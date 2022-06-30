---
title: Отправка уведомлений веб-канала действий пользователям в Microsoft Teams
description: Используйте API-интерфейсы уведомлений веб-канала действий Microsoft Teams в Microsoft Graph, чтобы поддерживать пользователей в курсе изменений в средствах и рабочих процессах, которые они используют.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: 7c0ab65bd6d79c662dd37ab8cbb2e14e3bcc2c70
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555956"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>Отправка уведомлений веб-канала действий пользователям в Microsoft Teams

Веб-канал действий Microsoft Teams позволяет пользователям рассматривать элементы, которые требуют внимания, уведомляя их об изменениях. Вы можете использовать API-интерфейсы уведомлений веб-канала действий в Microsoft Graph, чтобы расширить эту функцию для приложений. Это позволяет приложениям предоставлять более широкие возможности и лучше привлекать пользователей, помогая поддерживать их в актуальном состоянии с учетом изменений в используемых ими средствах и рабочих процессах.

## <a name="understand-the-basics-of-activity-feed-notification"></a>Основные сведения об уведомлении веб-канала действий

Уведомления веб-канала действий в Microsoft Teams состоят из нескольких битов информации, которые отображаются вместе, как показано на следующем рисунке.

![Изображение, показывающее компоненты уведомления веб-канала действий](images/teams-activityfeednotifications/notificationtemplate.png)

К компонентам относятся:
- Субъект, иницивший действие
- Значок, представляющий тип действия
- Причина, по которой субъект выполнил действие
- Предварительный просмотр текста
- Метка времени
- Место действия

В следующем примере показано, как эти компоненты вместе предоставляют сведения об уведомлении. В этом примере показано уведомление о пользователе, упомянутом в сообществе Yammer.

![Пример уведомления о действиях Yammer](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>Требования для использования API-интерфейсов уведомлений веб-канала действий

API-интерфейсы веб-канала действий работают с [приложением Teams](/microsoftteams/platform/overview). Ниже приведены требования для отправки уведомлений веб-канала действий.

- В манифесте приложения Teams должен быть Azure AD идентификатор приложения, добавленный в `webApplicationInfo` раздел. Дополнительные сведения см [. в схеме манифеста](/microsoftteams/platform/resources/schema/manifest-schema).
- Типы действий должны быть объявлены в разделе `activities` . Дополнительные сведения см [. в схеме манифеста](/microsoftteams/platform/resources/schema/manifest-schema).
- Приложение Teams должно быть установлено для получателя либо лично, либо в команде [или](/graph/api/resources/team) чате, [в который он](/graph/api/resources/chat) входит. Дополнительные сведения см. в статье [об установке приложения Teams](/graph/api/resources/teamsappinstallation).

### <a name="teams-app-manifest-changes"></a>Изменения манифеста приложения Teams

В этом разделе описываются изменения, которые необходимо добавить в манифест приложения Teams. Обратите внимание, что необходимо использовать [версию манифеста](/microsoftteams/platform/resources/schema/manifest-schema) `1.7` приложения Teams или более поздней версии.

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
```

#### <a name="webapplicationinfo-section-changes"></a>Изменения раздела webApplicationInfo

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|Параметр|Тип|Описание|
|:---|:---|:---|
|id|string|Azure AD приложения (идентификатор клиента).|
|resource|string|Ресурс, связанный с Azure AD приложения. Также называется URL-адресом ответа или перенаправления на портале Azure.|

> [!NOTE]
> Может возникнуть ошибка, если несколько приложений Teams в одной области (команда, чат или пользователь) используют одно Azure AD приложения. Убедитесь, что вы используете уникальные Azure AD приложения.

#### <a name="activities-section-changes"></a>Изменения раздела действий

```json
"activities":
{
  "activityTypes": [
    {
      "type": "taskCreated",
      "description": "Task Created Activity",
      "templateText": "{actor} created task {taskId} for you"
    },
    {
      "type": "approvalRequired",
      "description": "Deployment requires your approval",
      "templateText": "{actor} created a new deployment {deploymentId}"
    }
  ]
}
```

|Параметр|Тип|Описание|
|:---|:---|:---|
|type|string|Тип действия. Он должен быть уникальным в определенном манифесте.|
|description|string|Краткое описание, доступное для чтения. Он будет отображаться в клиенте Microsoft Teams.|
|templateText|string|Текст шаблона для уведомления о действии. Параметры можно объявить, инкапсулирование параметров в `{}`.|

> [!NOTE]
> `actor` — это специальный параметр, который всегда принимает имя вызывающего объекта. В делегированных вызовах `actor` — это имя пользователя. В вызовах, доступных только для приложений, он принимает имя приложения Teams.

### <a name="install-the-teams-app"></a>Установка приложения Teams

Приложения Teams можно устанавливать в команде, чате или лично для пользователя и распространять несколькими способами. Дополнительные сведения см. в разделе [о методах распространения приложений Teams](/microsoftteams/platform/concepts/deploy-and-publish/overview). Как правило, [загрузка неопубликованных](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) приложений предпочтительна для целей разработки. После разработки вы можете выбрать правильный метод распространения в зависимости от того, хотите ли вы распространить его между одним клиентом или всеми клиентами.

Вы также можете использовать [API установки приложений Teams](/graph/api/resources/teamsappinstallation) для управления установками приложений Teams.

## <a name="send-activity-feed-notifications-to-users"></a>Отправка уведомлений веб-канала действий пользователям

Так как приложение Teams можно установить для пользователя, в команде или в чате, уведомления также можно отправлять в следующих трех контекстах:

- [Отправка уведомления пользователю в чате](/graph/api/chat-sendactivitynotification)
- [Отправка уведомления пользователю в команде](/graph/api/team-sendactivitynotification)
- [Отправка уведомления пользователю](/graph/api/userteamwork-sendactivitynotification)

Кроме того, уведомления могут отправляться массово до 100 пользователей одновременно:

* [Массовая отправка уведомлений нескольким пользователям](/graph/api/teamwork-sendactivitynotificationtorecipients)

Дополнительные сведения о том, какие разделы поддерживаются для каждого сценария, см. в конкретных API. Пользовательские текстовые разделы поддерживаются во всех сценариях.

> [!NOTE]
> Значок действия основан на контексте, в который выполняется запрос. Если запрос выполняется с делегированными разрешениями, фотография пользователя отображается как аватар, а значок приложения Teams — как значок действия. В контексте только для приложений значок приложения Teams используется в качестве аватара, а значок действия опущен.

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Пример 1. Уведомление пользователя о задаче, созданной в чате

В этом примере показано, как отправить уведомление веб-канала действий для новой задачи, созданной в чате. В этом случае приложение Teams должно быть `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` установлено в чате с идентификатором, а пользователь также должен быть частью чата.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a>Пример 2. Уведомление пользователя о задаче, созданной в команде

В этом примере показано, как отправить уведомление о веб-канале действий для команды. В этом примере владелец команды уведомляет о созданной задаче, которая требует внимания.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>Пример 3. Уведомление пользователя о событии с помощью пользовательского раздела

Как показано в предыдущих примерах, вы можете связать различные аспекты команды или чата. Однако если вы хотите связать с аспектом, который не является частью команды или не представлен Microsoft Graph, или если вы хотите настроить имя, `topic` `text` можно задать источник и передать для него пользовательское значение. Кроме того, `webUrl` при использовании источника `topic` `text`в качестве .

В приведенном выше примере уведомления Yammer используется пользовательский раздел, так как ресурсы Yammer не поддерживаются Microsoft Graph.

> [!NOTE]
> `webUrl` должен начинаться с домена Microsoft Teams (например, teams.microsoft.com).

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-an-event"></a>Пример 4. Уведомление участников команды о событии

В этом примере показано, как отправить уведомление о веб-канале действий всем участникам команды. В этом примере участники команды уведомляют о новом событии. 

> [!NOTE]
> Возможность отправки уведомлений всем участникам команды в настоящее время доступна только в бета-версии.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db"
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-an-event"></a>Пример 5. Уведомление участников канала о событии

В этом примере показано, как отправить уведомление о веб-канале действий всем участникам канала. В этом примере участники канала уведомляют о новом событии. 

> [!NOTE]
> Возможность отправки уведомлений всем участникам канала в настоящее время доступна только в бета-версии.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db",
        "channelId": "19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2"
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-6-notify-the-chat-members-about-an-event"></a>Пример 6. Уведомление участников чата о событии

В этом примере показано, как отправить уведомление о веб-канале действий всем участникам чата. В этом примере участники чата уведомляют о новом событии. 

> [!NOTE]
> Возможность отправлять уведомления всем участникам чата в настоящее время доступна только в бета-версии.

#### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"
    }
}
```

#### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-7-notify-multiple-users-about-pending-finance-approval-requests"></a>Пример 7. Уведомление нескольких пользователей об ожидающих запросах на утверждение финансовых данных

В следующем примере показано, как массово отправлять уведомления в веб-канале действий нескольким пользователям. В этом примере несколько заинтересованных лиц уведомляют об ожидающих запросах на утверждение финансовых данных.

> [!NOTE]
> Возможность массовой отправки уведомлений нескольким пользователям в настоящее время доступна только в бета-версии.

#### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
  "name": "teamwork_sendactivitynotificationtorecipients"
}
-->

``` http
POST https://graph.microsoft.com/beta/teamwork/sendActivityNotificationToRecipients
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipients": [
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "ab88234e-0874-477c-9638-d144296ed04f"
        },
        {
            "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
            "userId": "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
        }
    ],
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```

#### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": false
}
-->

``` http
HTTP/1.1 202 Accepted
```

## <a name="customize-how-the-notifications-alert-you"></a>Настройка оповещений об уведомлениях

Пользователи Microsoft Teams могут настраивать уведомления, которые они видят в веб-канале, в виде баннера и т. д. Уведомления, созданные с помощью API-интерфейсов веб-канала действий, также можно настроить. Пользователи могут выбрать способ уведомления с помощью параметров в Microsoft Teams. Приложения Teams будут отображаться в списке для выбора пользователем, как показано на следующем снимке экрана.

![Снимок экрана: параметры уведомлений в Teams с выделенным параметром "Пользовательский"](images/teams-activityfeednotifications/notificationsettings.png)

Пользователи могут **нажать** кнопку "Изменить" рядом с приложением и настроить уведомления, как показано в следующем примере. Отобразится `description` поле в манифесте приложения Teams.

![Снимок экрана: уведомления, настроенные на баннер и веб-канал для приложения Teams](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a>Вопросы и ответы

### <a name="who-needs-to-install-the-teams-app"></a>Кому нужно установить приложение Teams?

У целевого пользователя должно быть установлено приложение Teams, которое отправляет уведомления.

### <a name="can-a-user-send-notifications-to-themselves"></a>Может ли пользователь отправлять уведомления себе?

Нет, пользователь не может отправлять уведомления себе. В этом сценарии используйте разрешения приложения.

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a>Может ли приложение Teams управлять тем, как уведомления отображаются пользователю?

Нет, изменять параметры уведомлений могут только пользователи.

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a>Приложение установлено; Почему я не вижу параметры уведомлений в учетной записи пользователя?

Параметры будут отображаться после отправки первого уведомления приложением Teams. Это сокращает количество параметров, которые видят пользователи.

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a>Я начал получать ошибку 409 (конфликт); Как устранить проблему?

`Conflict`Ошибки в основном возникают, когда несколько приложений Teams, установленных в одной области (команда, чат, пользователь и т. д.), имеют одинаковый Azure AD appId `webApplicationInfo` в разделе манифеста. В этом случае вы получите ошибку, например `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`. Убедитесь, что вы используете уникальные Azure AD для уникальных приложений Teams. Обратите внимание, что одно и то же приложение Teams можно установить в нескольких областях (например, команда и пользователь).

## <a name="see-also"></a>См. также

- [Рекомендации по использованию уведомлений веб-канала действий Microsoft Teams](teams-activity-feed-notifications-best-practices.md)
- [Разработка уведомлений веб-канала действий для Microsoft Teams](/microsoftteams/platform/concepts/design/activity-feed-notifications?tabs=mobile)
- [Обзор API Microsoft Teams](teams-concept-overview.md)
