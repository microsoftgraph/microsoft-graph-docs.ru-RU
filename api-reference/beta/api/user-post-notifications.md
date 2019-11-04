---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: c30df0bf19aeab48fab7655fd134dbc1cfe13195
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938164"
---
# <a name="create-and-send-a-notification"></a>Создание и отправление уведомления
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph. Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.  

## <a name="permissions"></a>Permissions
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

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено. В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской. 

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

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
