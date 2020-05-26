---
title: Обновление подписки
description: Возобновление подписки путем увеличения срока действия.
localization_priority: Normal
author: baywet
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 7611ed3b52861066fe7fbc666895c99cb7bc9003
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353268"
---
# <a name="update-subscription"></a>Обновление подписки

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Возобновление подписки путем увеличения срока действия.

Срок действия подписок истечет через период времени, который зависит от типа ресурса. Чтобы избежать отсутствия уведомлений об изменениях, приложение должно правильно обновить свои подписки до истечения срока их действия. В этой [статье приведены сведения](../resources/subscription.md) о максимальной длине подписки для каждого типа ресурсов.

## <a name="permissions"></a>Разрешения

В зависимости от ресурса и типа требующегося разрешения (делегированное или для приложения) разрешение, указанное в приведенной ниже таблице, является наименее привилегированным разрешением, необходимым для вызова этого API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
|[callRecord](../resources/callrecords-callrecord.md) | Не поддерживается | Не поддерживается | CallRecords.Read.All  |
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя) | Не поддерживается | Files.ReadWrite | Не поддерживается |
|[driveItem](../resources/driveitem.md) (OneDrive для бизнеса) | Files.ReadWrite.All | Не поддерживается | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Не поддерживается | Group.Read.All |
|[group conversation](../resources/conversation.md) | Group.Read.All | Не поддерживается | Не поддерживается |
|[list](../resources/list.md) | Sites.ReadWrite.All | Не поддерживается | Sites.ReadWrite.All |
|[message](../resources/message.md) | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |
|[security alert](../resources/alert.md) | SecurityEvents.ReadWrite.All | Не поддерживается | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Примечание.** Существуют дополнительные ограничения для подписок на элементы OneDrive и Outlook. Ограничения применяются для создания, а также управления подписками (получение, обновление и удаление подписок).

- В личном хранилище OneDrive можно подписаться на корневую папку или любую вложенную папку в этом хранилище. В OneDrive для бизнеса можно подписаться только на корневую папку. Уведомления об изменениях отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии. Нельзя подписаться на экземпляры **drive** или **driveItem**, не являющиеся папками, например на отдельные файлы.

- В Outlook делегированные разрешения поддерживают подписку на элементы в папках только в почтовом ящике пользователя, вошедшего в систему. Это означает, например, что нельзя использовать делегированное разрешение Calendars.Read, чтобы подписаться на события в почтовом ящике другого пользователя.
- Чтобы подписаться на уведомления об изменениях контактов Outlook, событий или сообщений в _общих или делегированных_ папках:

  - Используйте соответствующее разрешение приложения для подписки на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.
  - Не используйте разрешения Outlook на общий доступ (Contacts.Read.Shared, Calendars.Read.Shared, Mail.Read.Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменениях элементов в общих или делегированных папках.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PATCH /subscriptions/{id}
```

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.

Сведения о том, как возвращаются ошибки, приведены в разделе [ошибочные ответы][error-response].

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}-->

```http
PATCH https://graph.microsoft.com/beta/subscriptions/{id}
Content-type: application/json

{
   "expirationDateTime":"2016-11-22T18:23:45.9356913Z"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-subscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-subscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-subscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-22T18:23:45.9356913Z",
  "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
  "latestSupportedTlsVersion": "v1_2"
}
```

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Update subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
