---
title: Создание подписки
description: Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.
ms.openlocfilehash: f524213871f8a9216ad7f7ec8da4ffb521a4a2aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082318"
---
# <a name="create-subscription"></a>Создание подписки

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Подписывается прослушиватель для получения уведомлений при изменении данных в Microsoft Graph ресурсов.

## <a name="permissions"></a>Permissions

Создание подписки на требует разрешения на чтение ресурса, для которого приложение будет получать уведомления. Например, чтобы получать уведомления о сообщениях, ваше приложение должно `Mail.Read` разрешений. В таблице ниже перечислены рекомендуемые разрешения, которые требуются для каждого ресурса. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип ресурса или элемент        | Разрешение          |
|-----------------------------|---------------------|
| Contacts                    | Contacts.Read       |
| Беседы               | Group.Read.All      |
| События                      | Calendars.Read      |
| Сообщения                    | Mail.Read           |
| Groups                      | Group.Read.All      |
| Users                       | User.Read.All       |
| Диск (хранилище OneDrive пользователя)    | Files.ReadWrite.     |
| На дисках (содержимое общих SharePoint и диски) | Files.ReadWrite.All |
| Предупреждение системы безопасности              | SecurityEvents.ReadWrite.All |

> **Примечание:** Конечная точка /beta позволяет разрешения приложения для большинства ресурсов. Беседы в группу и OneDrive элементов корневой диск с разрешениями приложения не поддерживаются.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /subscriptions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201 Created` и объект [subscription](../resources/subscription.md) в теле отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

В тексте запроса укажите представление объекта [подписки](../resources/subscription.md) с JSON.
`clientState` Поле является необязательным.

Этот пример запроса создает подписки для уведомлений о новых сообщений, полученных в настоящее время входа пользователя.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{
   "changeType": "created,updated",
   "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
   "resource": "me/mailFolders('Inbox')/messages",
   "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
   "clientState": "secretClientValue"
}
```

Ниже приведены допустимые значения для свойства ресурса:

| Тип ресурса | Примеры |
|:------ |:----- |
|Почта|me/mailfolders('inbox')/messages<br />me/messages|
|Контакты|me/contacts|
|Календари|me/events|
|Users|users|
|Groups|группы|
|Conversations|groups('*{id}*')/conversations|
|Drives|me/drive/root|
|Предупреждение системы безопасности|Оповещение системы безопасности /? $filter = состояние eq «Создать»|

##### <a name="response"></a>Ответ

Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 252

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
  "id": "7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource": "me/mailFolders('Inbox')/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType": "created,updated",
  "clientState": "secretClientValue",
  "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime": "2016-11-20T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
}
```

## <a name="notification-endpoint-validation"></a>Проверка конечной точки уведомлений

Конечная точка уведомления подписки (указанного в `notificationUrl` свойство) должен быть способен отвечать на запрос проверки, как описано в [Настройка уведомлений для изменения в данные пользователя](/graph/webhooks#notification-endpoint-validation). Если не удается выполнить проверку, запрос на создание подписки возвращает ошибку 400 Ошибочный запрос.

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
