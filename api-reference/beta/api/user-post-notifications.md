---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 8eb35ea0ade2e7d471674d8d064ba0ac38b361cc
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996270"
---
# <a name="create-and-send-a-notification"></a>Создание и отправление уведомления
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph. Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.  

## <a name="permissions"></a>Разрешения
Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.  

> [!IMPORTANT]
> Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений. Мы не рекомендуем использовать этот параметр для отправки уведомлений, но если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notifications.ReadWrite.CreatedByApp    |
|Делегированные (личная учетная запись Майкрософт) | Notifications.ReadWrite.CreatedByApp    |
| Для приложений                           | Не поддерживается. |


## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Заголовки запросов
|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string |Заголовок Authorization используется для передачи учетных данных вызывающей стороны. Bearer {Token}. Обязательный элемент. |
|X – УНС — ID | string |Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки на стороне клиента, и используется для назначения определенного пользователя. Обязательный параметр. |
|Content-Type| application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено. В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской. 

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_notification_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/me/notifications
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "appNotificationId": "appNotificationID-value",
    "expirationDateTime": "datetime-value",
    "targetPolicy": {
      "platformTypes": [
        "platformTypes-value"
        ]
      }, 
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-notification-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notification"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "notification": {
    "targetHostName": "targetHostName-value",
    "expirationDateTime": "datetime-value",
    "payload": {
      "rawContent": "rawContent-value",
      "visualContent": {
        "title": "title-value",
        "body": "body-value"
      }
    },
    "displayTimeToLive": 99,
    "priority": "priority-value",
    "groupName": "groupName-value"
  }
}
```
