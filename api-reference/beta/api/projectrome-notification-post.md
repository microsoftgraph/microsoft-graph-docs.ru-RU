---
title: Создание и отправка уведомления
description: 'Создание и отправка уведомления, предназначенные для пользователей через Microsoft Graph. Уведомление, сохраненных в Microsoft Graph уведомление, веб-канала хранилища и отправляется всем клиентам приложения на всех конечных точках устройства, которые пользователь входит в систему.  '
localization_priority: Normal
ms.openlocfilehash: 67906aa56ace21d9d03cfe47c17acda38d8c680f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843901"
---
# <a name="create-and-send-a-notification"></a>Создание и отправка уведомления
> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Создание и отправка уведомления, предназначенные для пользователей через Microsoft Graph. Уведомление, сохраненных в Microsoft Graph уведомление, веб-канала хранилища и отправляется всем клиентам приложения на всех конечных точках устройства, которые пользователь входит в систему.  
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notifications.ReadWrite.CreatedByApp    |
|Делегированные (личная учетная запись Майкрософт) | Notifications.ReadWrite.CreatedByApp    |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Заголовки запросов
|Имя | Тип | Описание|
|:----|:-----|:-----------|
|Authorization | string |Заголовок authorization используется для передачи учетных данных вызывающей стороны. Носителя {маркер}. Обязательный. |
## <a name="request-body"></a>Тело запроса
В тексте запроса укажите представление JSON объекта [уведомлений](../resources/projectrome-notification.md) .

## <a name="response"></a>Ответ
Успешно завершена, этот метод возвращает `201 Created` код ответа, которое указывает, что уведомления было успешно создаются и сохраняются. 
## <a name="example"></a>Пример
#### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2018-08-29T23:51:33.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
        "windows",
        "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "23"
}
```

#### <a name="response"></a>Ответ
Ниже приведен пример ответа.

```http
HTTP/1.1 201
Content-Type: application/json
location: https://graph.microsoft.com/beta/me/notifications/518c4fb1-c565-4d67-95c4-bcc3eb8eda1b

{
    "@odata.context": "https://graph.microsoft.com/test872018/$metadata#users('graphNotificationsUser%40contoso.com')/notifications/$entity",
    "appNotificationId": "testDirectToastNotification",
    "displayTimeToLive": 23,
    "expirationDateTime": "2018-08-24T12:31:53.858Z",
    "groupName": "TestGroup",
    "id": "cd5c5e6a-99ce-470a-9982-c47635e73620",
    "priority": "1",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


