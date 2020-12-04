---
title: Отправка уведомлений о каналах активности пользователям в Microsoft Teams
description: Отправлять уведомления о каналах активности пользователям в Microsoft Teams с помощью приложений Teams и Microsoft Graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 698a5ed338906f8eed2d2611c8aba3b4f0b6f624
ms.sourcegitcommit: c419bb8901b7766af193196f80bc1d497643fcb2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/04/2020
ms.locfileid: "49572123"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a>Отправка уведомлений о каналах активности пользователям в Microsoft Teams

Канал активности Microsoft Teams позволяет пользователям рассматривать элементы, требующие внимания, уведомляя их об изменениях. Вы можете использовать API уведомления о каналах активности в Microsoft Graph, чтобы расширить эту функциональность для ваших приложений. Это позволит вашим приложениям предоставлять более широкие возможности и лучше привлекать пользователей, помогая поддерживать их в соответствии с изменениями в средствах и рабочих процессах, которые они используют.

## <a name="understanding-the-basics-of-activity-feed-notification"></a>Основные сведения об уведомлении канала активности

Уведомления канала активности в Microsoft Teams состоят из нескольких битов данных, которые отображаются вместе, как показано на следующем рисунке.

![Изображение, на котором показаны компоненты уведомления веб-канала активности](images/teams-activityfeednotifications/notificationtemplate.png)

К компонентам относятся:
- Субъект, который инициировал действие
- Значок, представляющий тип действия
- Причина, по которой субъект выполнил действие
- Предварительный просмотр текста
- Отметка времени
- Расположение действия

В следующем примере показано, как эти компоненты совместно предоставляют сведения об уведомлении. В этом примере отображается уведомление о пользователе, упомянутом в сообществе Yammer.

![Пример уведомления актифити Yammer](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a>Требования для использования API уведомления канала активности

API веб-каналов активности работают с [приложением Teams](/microsoftteams/platform/overview). Ниже приведены требования для отправки уведомлений о каналах активности:

- Манифест приложения Teams должен иметь идентификатор приложения Azure AD, добавленный в `webApplicationInfo` раздел. Дополнительные сведения см. в статье [схема манифеста](/microsoftteams/platform/resources/schema/manifest-schema).
- Типы действий должны быть объявлены в `activities` разделе. Дополнительные сведения см. в статье [схема манифеста](/microsoftteams/platform/resources/schema/manifest-schema).
- Приложение Teams должно быть установлено для получателя, либо для личного, либо для [группы](/graph/api/resources/team?preserve-view=true) или [чата](/graph/api/resources/chat?preserve-view=true) . Дополнительные [сведения см.](/graph/api/resources/teamsappinstallation?preserve-view=true)

### <a name="teams-app-manifest-changes"></a>Изменения в манифесте приложения Teams

В этом разделе описываются изменения, которые необходимо добавить в манифест приложения Teams. Обратите внимание, что необходимо использовать [манифест приложения Teams](/microsoftteams/platform/resources/schema/manifest-schema) `1.7` или более поздней версии.

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a>изменения в разделе webApplicationInfo

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|Параметр|Тип|Описание|
|:---|:---|:---|
|id|string|Идентификатор приложения Azure AD (идентификатор клиента).|
|resource|string|Ресурс, связанный с приложением Azure AD. Также называется URL-адресом ответа или перенаправлением на портале Azure.|

> **Примечание:** Вы можете получить сообщение об ошибке, если несколько приложений Teams в одной области (группа, чат или пользователь) используют одно и то же приложение Azure AD. Убедитесь, что вы используете уникальные приложения Azure AD.

#### <a name="activities-section-changes"></a>изменения в разделе "действия"

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
|type|string|Тип действия. Они должны быть уникальными в определенном манифесте.|
|description|string|Понятное для человека краткое описание. Он будет отображаться в клиенте Microsoft Teams.|
|темплатетекст|string|Текст шаблона для уведомления о действии. Вы можете объявить параметры с помощью инкапсуляции параметров в `{}` .|

>**Примечание:** `actor` — Это особый параметр, который всегда принимает имя вызывающего абонента. В случае делегированных вызовов `actor` — это имя пользователя. В вызовах, использующих только приложения, он принимает имя приложения Teams.

### <a name="installing-the-teams-app"></a>Установка приложения Teams

Приложения Teams могут быть установлены в команде, в чате или для пользователя лично и могут распространяться несколькими способами. Подробнее: [методы распространения приложений Teams](/microsoftteams/platform/concepts/deploy-and-publish/overview). Как правило, для целей разработки рекомендуется использовать загрузку [неопубликованных приложений](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) . После разработки можно выбрать правильный метод распространения в зависимости от того, хотите ли вы распределить их по одному клиенту или всем клиентам.

Вы также можете использовать API [установки приложений Teams](/graph/api/resources/teamsappinstallation?preserve-view=true) для управления установками приложений Teams.

## <a name="sending-activity-feed-notifications-to-users"></a>Отправка уведомлений о каналах активности пользователям

Поскольку приложение Teams можно установить для пользователя, в команде или в чате, уведомления можно отправлять в этих трех контекстах:

- [Отправка уведомления пользователю в чате](/graph/api/chat-sendactivitynotification)
- [Отправка уведомления пользователю команды](/graph/api/team-sendactivitynotification)
- [Отправка уведомления пользователю](/graph/api/userteamwork-sendactivitynotification)

Сведения о том, какие разделы поддерживаются для каждого сценария, можно найти в указанных API. Настраиваемые текстовые разделы поддерживаются для всех сценариев.

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a>Пример 1: уведомление пользователя о задаче, созданной в чате

В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате. В этом случае приложение Teams должно быть установлено в чате с идентификатором, `chatId` а пользователь `569363e2-4e49-4661-87f2-16f245c5d66a` также должен входить в чат.

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

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a>Пример 2: уведомление пользователя о задаче, созданной в команде

В этом примере показано, как можно отправить уведомление веб-канала активности для команды. В этом примере владелец команды уведомляется о новой созданной задаче, требующей внимания.

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

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a>Пример 3: уведомление пользователя о событии с помощью настраиваемого раздела

Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты команды или чата. Тем не менее, если вы хотите создать ссылку на аспект, который не является частью команды или не представлен в Microsoft Graph, или если вы хотите настроить это имя, вы можете задать для `topic` `text` него значение и передать его настраиваемое значение. Кроме того, `webUrl` является обязательным, если используется `topic` источник AS `text` .

В примере уведомления Yammer, показанном ранее, используется настраиваемый раздел, так как в Microsoft Graph ресурсы Yammer не поддерживаются.

> **Примечание:** `webUrl` должна начинаться с домена Microsoft Teams (например, teams.microsoft.com).

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
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
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

## <a name="customizing-how-the-notifications-alert-you"></a>Настройка оповещения о том, как вы

Пользователи Microsoft Teams могут настраивать уведомления, которые они видят в веб-канале, в виде баннера и т. д. Уведомления, созданные через API веб-каналов активности, также могут быть изменены. Пользователи могут выбрать способ уведомления с помощью параметров в Microsoft Teams. Приложения Teams отобразятся в списке, чтобы выбрать пользователя, как показано на следующем снимке экрана.

![Снимок экрана с параметрами уведомлений в Teams с выделенным настраиваемым параметром](images/teams-activityfeednotifications/notificationsettings.png)

Пользователи могут нажать кнопку **изменить** рядом с приложением и настроить уведомления, как показано в следующем примере. `description`Отображается поле в манифесте приложения Teams.

![Снимок экрана, на котором показаны уведомления, измененные на баннер и веб-канал для приложения Teams](images/teams-activityfeednotifications/applevelnotificationsettings.png)
