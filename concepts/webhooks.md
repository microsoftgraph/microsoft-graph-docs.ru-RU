---
title: Настройка уведомлений об изменениях в пользовательских данных
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: bfd2ddff5fe87ccabd2c0d7a935ba429c67bda09
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038508"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>Настройка уведомлений об изменениях в пользовательских данных

The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.

Когда Microsoft Graph принимает запрос на подписку, он передает уведомления об изменениях URL-адресу, указанному в подписке. Затем приложение действует в соответствии с бизнес-логикой. Например, оно получает дополнительные данные, обновляет кэш и представления, а также выполняет другие действия.


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [Руководство: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

По умолчанию уведомления об изменениях не включают данные ресурсов, кроме `id`. Если приложению требуются данные ресурса, оно может вызвать API Microsoft Graph, чтобы получить ресурс полностью. В этой статье ресурс **User** используется в качестве примера для работы с уведомлениями об изменениях.

Приложение также может подписаться на уведомления об изменениях, включающие данные ресурсов, чтобы избежать необходимости дополнительного вызова API для доступа к данным. В этом случае приложению необходимо реализовать дополнительный код для обработки требований таких уведомлений, в частности, ответа на уведомления о жизненном цикле подписки, проверки подлинности уведомлений и расшифровки данных ресурсов. Другие типы ресурсов также будут поддерживать этот тип уведомлений в дальнейшем. Дополнительные сведения о работе с такими уведомлениями см. в статье [Настройка уведомлений об изменениях, включающих данные ресурсов (предварительная версия)](webhooks-with-resource-data.md).

## <a name="supported-resources"></a>Поддерживаемые ресурсы

С помощью API Microsoft Graph приложение может подписаться на изменения для следующих ресурсов:

- [Сообщение][] Outlook
- [Событие][] Outlook
- Личный [контакт][] Outlook
- [user][]
- [group][]
- [Беседа][] группы (майкрософт) 365
- Контент внутри иерархии _любой папки_ [driveItem][] на персональном хранилище OneDrive пользователя
- Контент внутри иерархии _корневой папки_ [driveItem][] на персональном хранилище OneDrive для бизнеса
- [Оповещение][] безопасности
- [Каллрекорд][] Teams
- Teams [chatMessage][] (предварительная версия)

Например, вы можете создать подписку на определенную папку Outlook, например, папку Входящие: `me/mailFolders('inbox')/messages`

Или на ресурс верхнего уровня:,, `/me/messages` `/me/contacts` ,, `/me/events` `users` `groups` или`/communications/callRecords`

либо на определенный экземпляр ресурса: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`;

либо на личное хранилище OneDrive пользователя: `/drives/{id}/root`
`/drives/{id}/root/subfolder`.

либо на корневую папку диска SharePoint/OneDrive для бизнеса: `/drive/root`

либо на новое оповещение [API безопасности](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`

### <a name="azure-ad-resource-limitations"></a>Ограничения ресурсов Azure AD

К ресурсам Azure AD (пользователи, группы) применяются определенные ограничения. В случае их превышения возникают ошибки.

> **Примечание**. Эти ограничения не применяются к ресурсам служб, не относящихся к Azure AD. Например, приложение может создать больше дополнительных подписок на ресурсы `message` или `event`, поддерживаемые службой Exchange Online в составе Microsoft Graph.

- Квоты максимальной подписки:

  - Для каждого приложения (для всех клиентов): 50 000 всего подписок
  - Для каждого клиента (для всех приложений в совокупности): 1000 всего подписок для всех приложений
  - На сочетание приложения и клиента: 100 подписок всего

При превышении какого-либо ограничения попытки создать подписку приведут к возникновению [ошибки](errors.md)  -  `403 Forbidden` . Свойство `message` указывает, какое ограничение превышено.

- Клиенты Azure AD B2C не поддерживаются.

- Уведомление чангфе для пользовательских сущностей не поддерживается для личных учетных записей Майкрософт.

- В подписках пользователей и групп существует [известная проблема](known-issues.md#change-notifications).

### <a name="outlook-resource-limitations"></a>Ограничения ресурсов Outlook

Если вы используете *имя участника-пользователя* на пути к ресурсу при оформлении подписки на ресурсы Outlook, например **сообщения**, **события** или **контакты**, запрос на подписку может быть не выполнен, если это имя содержит апостроф.  Используйте ИД GUID пользователей вместо имен участников-пользователей, чтобы избежать этой проблемы. Например, вместо пути к ресурсу:

`/users/sh.o'neal@contoso.com/messages`

Используйте: 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a>Время существования подписки

Время существования подписок ограничено. Приложениям необходимо обновлять подписки до истечения срока их действия. В противном случае им потребуется создавать новые подписки. Список значений, представляющих собой максимально допустимый срок действия, см. в разделе [Максимальный период подписки для каждого из типов ресурсов](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).

Кроме того, приложения могут отменять подписку в любое время, чтобы остановить получение уведомлений об изменениях.

## <a name="managing-subscriptions"></a>Управление подписками

Клиенты могут создавать, продлевать и удалять подписки.

### <a name="creating-a-subscription"></a>Создание подписки

Creating a subscription is the first step to start receiving change notifications for a resource. The subscription process is as follows:

1. Клиент отправляет запрос (POST) на подписку для определенного ресурса.

1. Microsoft Graph проверяет запрос.

    - Если запрос является допустимым, Microsoft Graph отправляет маркер проверки на URL-адрес уведомлений.
    - В противном случае Microsoft Graph возвращает сообщение об ошибке с кодом и подробными сведениями.

1. Клиент отправляет маркер проверки в Microsoft Graph.

1. Клиент получает ответ от Microsoft Graph.

Клиент должен хранить идентификатор подписки, чтобы сопоставить уведомления об изменениях с подпиской.

#### <a name="subscription-request-example"></a>Пример запроса на подписку

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

Необходимы свойства `changeType`, `notificationUrl`, `resource` и `expirationDateTime`. Определения и значения свойств представлены в [описании типа ресурса подписки](/graph/api/resources/subscription?view=graph-rest-1.0).

Свойство `resource` указывает ресурс, для которого будут отслеживаться изменения. Например, вы можете создать подписку на определенную почтовую папку: `me/mailFolders('inbox')/messages` или сделать это от имени пользователя с согласия администратора: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.

Хотя `clientState` это не обязательно, необходимо включить его в соответствии с рекомендуемым процессом обработки уведомлений об изменениях. Задание этого свойства позволяет подтвердить, что уведомления об изменениях, получаемые от службы Microsoft Graph, вы можете подтвердить. По этой причине значение свойства должно оставаться секретным и быть известно только приложению и службе Microsoft Graph.

В случае успешного выполнения Microsoft Graph возвращает код `201 Created` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика.

#### <a name="notification-endpoint-validation"></a>Проверка конечной точки уведомлений

Прежде чем создавать подписку, Microsoft Graph проверяет конечную точку уведомлений в `notificationUrl` запросе на свойство подписки. Проверка происходит следующим образом:

1. Microsoft Graph отправляет запрос POST на URL-адрес уведомлений:

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **Важно!** Так как `validationToken` — это параметр запроса, он должен декодироваться клиентом согласно правилам кодирования HTTP. Если клиент не декодирует маркер и использует закодированное значение на следующем шаге (ответ), конечная точка не пройдет проверку. Кроме того, клиент должен рассматривать значение маркера как непрозрачное, так как формат маркера может измениться в будущем без уведомления.

1. В течение 10 секунд клиент должен предоставить ответ со следующими характеристиками:

    - Код состояния 200 (OK).
    - Необходимый тип контента — `text/plain`.
    - Текст должен содержать маркер проверки, предоставленный Microsoft Graph.

Клиент должен удалить маркер проверки после того, как укажет его в отклике.

Кроме того, можно использовать [коллекцию Microsoft Graph Postman](use-postman.md), чтобы убедиться в правильности реализации запроса проверки в вашей конечной точке. Запрос **Проверка подписки** в папке **Прочее** предоставляет модульные тесты, проверяющие отклик вашей конечной точки.  

![результаты теста отклика проверки](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a>Возобновление подписки

Клиент может продлить подписку, указав срок действия до трех дней с момента отправки запроса. Свойство `expirationDateTime` является обязательным.

#### <a name="subscription-renewal-example"></a>Пример возобновления подписки

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

В случае успешного выполнения Microsoft Graph возвращает код `200 OK` и объект [подписки](/graph/api/resources/subscription?view=graph-rest-1.0) в теле отклика. Объект подписки включает новое значение `expirationDateTime`.

### <a name="deleting-a-subscription"></a>Удаление подписки

Клиент может прекратить получать уведомления об изменениях, удалив подписку с помощью ее идентификатора.

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

В случае успешного выполнения Microsoft Graph возвращает код `204 No Content`.

## <a name="change-notifications"></a>Уведомления об изменениях

Если клиент выполняет подписку на изменения ресурса, Microsoft Graph отправляет `POST` запрос на URL-адрес уведомлений при каждом изменении ресурса. Он отправляет уведомления только для тех изменений типа, которые указаны в подписке, например `created` .

> **Примечание:** Если клиент имеет несколько подписок, контролирующих один и тот же URL-адрес уведомления, Microsoft Graph может отправлять несколько уведомлений об изменениях, соответствующих разным подпискам, каждый из которых отображает соответствующий идентификатор подписки. Нет гарантии, что все уведомления об изменениях в `POST` запросе принадлежат одной подписке.

### <a name="change-notification-example"></a>Пример уведомления об изменении

В этом разделе представлен пример уведомления для создания сообщения. Когда пользователь получает электронное письмо, Microsoft Graph отправляет уведомление об изменении, как показано в следующем примере.
Обратите внимание, что уведомление представлено в коллекции, представленной в `value` поле. Сведения о полезных данных уведомления можно найти в [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection) . 

При возникновении большого количества изменений Microsoft Graph может отправлять несколько уведомлений, соответствующих разным подпискам в одном `POST` запросе.

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a>Обработка уведомления об изменении

Процесс должен обрабатывать каждое уведомление об изменении, которое он получает. Ниже приведены минимальные задачи, которые приложение должно выполнить для обработки уведомления об изменении.

1. Отправьте код состояния `202 - Accepted` в ответе, предназначенном Microsoft Graph. Если Microsoft Graph не получает код класса 2xx, он попытается опубликовать уведомление об изменении несколько раз в течение 4 часов; После этого уведомление об изменении будет удалено и не будет доставлено.

    > **Примечание:** Отправьте код состояния сразу же после `202 - Accepted` получения уведомления об изменении, даже перед проверкой его подлинности. Вы просто подтверждаете получение уведомления об изменении и предотвратите ненужные попытки. Текущее значение времени ожидания — 30 секунд, но это время может быть сокращено в будущем для оптимизации производительности службы. Если URL-адрес уведомления не отвечает в течение 30 секунд для более чем 10% запросов от Microsoft Graph за 10 минут, все следующие уведомления будут задержаны и повторены в течение 4 часов. Если URL-адрес уведомления не отвечает в течение 30 секунд за более 20% запросов от Microsoft Graph за 10 минут, будут удалены все следующие уведомления.

1. Проверьте свойство `clientState`. Оно должно соответствовать значению, отправленному с запросом на создание подписки.

    > **Примечание:** Если это не так, вы не должны считать это действительное уведомление об изменении. Возможно, что уведомление об изменении не получено из Microsoft Graph и может быть отправлено фальшивым субъектом. Кроме того, следует проверить, откуда поступило уведомление об изменении, и предпринять соответствующие действия.

1. Обновляйте приложение в соответствии с бизнес-логикой.

Повторите эти действия для других уведомлений об изменении в запросе.

## <a name="code-samples"></a>Примеры кода

Указанные ниже примеры кода доступны на сайте GitHub.

- [Обучающий модуль по Microsoft Graph: использование уведомлений об изменениях и отслеживание изменений с помощью Microsoft Graph](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [Пример веб-перехватчиков Microsoft Graph для Node.js](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [Пример веб-перехватчиков Microsoft Graph для ASP.NET Core](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [Пример веб-перехватчиков Microsoft Graph для Java Spring](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a>Конфигурация брандмауэра

При необходимости можно настроить брандмауэр, защищающий URL-адрес уведомлений, чтобы разрешить входящие подключения только из Microsoft Graph. Это позволяет уменьшить риск недопустимых уведомлений об изменениях, отправляемых на URL-адрес уведомлений. Эти недопустимые уведомления об изменении могут пытаться активировать реализованную пользовательскую логику. Полный список IP-адресов, используемых Microsoft Graph для доставки уведомлений об изменениях, приведен в разделе [дополнительные конечные точки для microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).

> **Примечание:** Указанные IP-адреса, используемые для доставки уведомлений об изменениях, можно обновить в любое время без уведомления.

## <a name="see-also"></a>См. также

- [Тип ресурса subscription](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Получение подписки](/graph/api/subscription-get?view=graph-rest-1.0)
- [Создание подписки](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- Тип ресурса [чанженотификатион](/graph/api/resources/changenotification?view=graph-rest-beta)
- Тип ресурса [чанженотификатионколлектион](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)
- [Руководство по изменениям уведомлений и отслеживания изменений](/learn/modules/msgraph-changenotifications-trackchanges)
- [Уведомления в жизненном цикле (Предварительная версия)](/graph/concepts/webhooks-outlook-authz.md)

[contact]: /graph/api/resources/contact?view=graph-rest-1.0
[conversation]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
