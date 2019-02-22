---
title: Получение подписки
description: Получение свойств и связей подписки.
localization_priority: Normal
author: piotrci
ms.openlocfilehash: c73f01a65a2b81bfa34818f9a7a96f754501bd65
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163471"
---
# <a name="get-subscription"></a>Получение подписки

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей подписки.

## <a name="permissions"></a>Разрешения

В зависимости от ресурса и запрашиваемого типа разрешения (делегированного или приложения) разрешение, указанное в следующей таблице, является минимальным привилегированным требованием для вызова этого API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
|[contact](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
|[driveItem](../resources/driveitem.md) (личное хранилище OneDrive пользователя) | Не поддерживается | Files.ReadWrite | Не поддерживается |
|[driveItem](../resources/driveitem.md) (OneDrive для бизнеса) | Files.ReadWrite.All | Не поддерживается | Files.ReadWrite.All |
|[event](../resources/event.md) | Calendars.Read | Calendars.Read | Calendars.Read |
|[group](../resources/group.md) | Group.Read.All | Не поддерживается | Group.Read.All |
|[Групповая беседа](../resources/conversation.md) | Group.Read.All | Не поддерживается | Не поддерживается |
|[message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
|[Оповещение системы безопасности](../resources/alert.md) | SecurityEvents.ReadWrite.All | Не поддерживается | SecurityEvents.ReadWrite.All |
|[user](../resources/user.md) | User.Read.All | User.Read.All | User.Read.All |

> **Примечание:** Существуют дополнительные ограничения для подписок на OneDrive и элементы Outlook. Ограничения применяются к созданию и управлению подписками (процессами, обновлением и удалением подписок).

- В личном OneDrive вы можете подписаться на корневую папку или любую подпапку на этом диске. В OneDrive для бизнеса можно подписаться только на корневую папку. Уведомления отправляются для запрошенных типов изменений в подписанной папке, а также любых файлов, папок или других объектов driveItem в иерархии. Вы не можете подписаться на **диски** или экземпляры **driveItem** , которые не являются папками, например отдельными файлами.

- Делегированное разрешение в Outlook поддерживает подписку на элементы в папках только в почтовом ящике вошедшего пользователя. Это означает, например, вы не можете использовать делегированные календари разрешений. Read для подписки на события в почтовом ящике другого пользователя.
- Чтобы подписаться на уведомления об изменении контактов, событий или сообщений Outlook в _общих или делегированных_ папках, выполните следующие действия:

  - Используйте соответствующее разрешение приложения, чтобы подписаться на изменения элементов в папке или почтовом ящике _любого_ пользователя в клиенте.
  - Не используйте разрешения на общий доступ к Outlook (Contacts. Read. Shared, Calendars. Read. Shared, mail. Read. Shared и их аналоги для чтения и записи), так как они **не** поддерживают подписку на уведомления об изменении элементов в общих или делегированных папках.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя       | Тип | Описание|
|:-----------|:-----|:-----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscription](../resources/subscription.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions/{id}
```

##### <a name="response"></a>Ответ

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 252

{
  "id":"7f105c7d-2dc5-4530-97cd-4e7ae6534c07",
  "resource":"me/messages",
  "applicationId" : "string",
  "changeType":"created,updated",
  "clientState":"secretClientValue",
  "notificationUrl":"https://webhook.azurewebsites.net/api/send/myNotifyClient",
  "expirationDateTime":"2016-11-20T18:23:45.9356913Z",
  "creatorId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscription",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
