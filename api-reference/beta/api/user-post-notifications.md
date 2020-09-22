---
title: Создание и отправление уведомления
description: Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph.
localization_priority: Normal
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 7296a136a4d2bab38eaf8ef25790019abc05bf6b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064523"
---
# <a name="create-and-send-a-notification"></a>Создание и отправление уведомления

Пространство имен: Microsoft. Graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание и отправка уведомления, предназначенного для пользователя с помощью Microsoft Graph. Уведомление хранится в хранилище каналов уведомлений Microsoft Graph и отправляется всем клиентам приложений во всех конечных точках устройств, в которых пользователь вошел в систему.  

## <a name="permissions"></a>Разрешения
Служба приложения не требует дополнительных разрешений для отправки уведомлений целевому пользователю.  

> [!IMPORTANT]
> Если вы решите отправлять уведомления от имени пользователя через делегированные разрешения, то для вызова этого API требуется одно из следующих разрешений. Мы не рекомендуем использовать этот параметр для создания уведомлений. Если вы хотите узнать больше, в том числе как выбирать разрешения, ознакомьтесь с разделом [разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Notifications.ReadWrite.CreatedByApp    |
|Делегированные (личная учетная запись Майкрософт) | Notifications.ReadWrite.CreatedByApp    |
|Для приложений | Не поддерживается.|



## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/notifications/
```
## <a name="request-headers"></a>Заголовки запросов
|Имя | Описание|
|:----|:-----------|
|Авторизация | Заголовок Authorization используется для передачи учетных данных вызывающей стороны. Bearer {Token}. Обязательно. |
|X – УНС — ID | Усернотификатионсубскриптионид, возвращенный службой уведомлений Microsoft Graph после создания подписки, и используется для назначения определенного пользователя. Обязательный параметр. |
|Content-Type | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [уведомления](../resources/projectrome-notification.md) в формате JSON.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика, указывающий, что уведомление было успешно создано и сохранено. В дальнейшем уведомление будет развертывание которого выполняется на все указанные конечные точки с действующей подпиской. 

В следующей таблице перечислены возможные коды ошибок и ответов, которые могут быть возвращены.

|Код ошибки             | дескритион                             |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode. Бадрекуест           | Body является массивом (несколько уведомлений не поддерживаются).|
|HttpStatusCode. Бадрекуест           | Текст не отвечает контракту для API.               |
|HttpStatusCode. запрещено            | Абонент находится в списке заблокированных.                          |
|HttpStatusCode. Месодноталловед     | Используемый метод HTTP не поддерживается.                     |
|HttpStatusCode. Бадрекуест           | В запросе присутствуют Неподдерживаемые заголовки. Два заголовка не поддерживаются:<br/><br/>If — Modified — с<br/>Если — Range |                    
|HttpStatusCode. Унсуппортедмедиатипе | Заголовок Content-Encoding присутствует и имеет значения алгоритма сжатия, отличные от `Deflate` OR `Gzip` .  |
|HttpStatusCode. Бадрекуест           | Недопустимые полезные данные.                                           |
|HttpStatusCode. запрещено            | Абонент не имеет прав на действия от имени пользователя или отправлять уведомление пользователю.                         |
|HttpStatusCode. несанкционированный         |  Текст запроса содержит недопустимые типы данных о действиях.        |
|HttpStatusCode. ОК                   |  Действие успешно создано.                            |
|HttpStatusCode. Нотакцептабле        |  Запрос был отрегулирован или сервер занят.    |


## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

```http
POST https://graph.microsoft.com/beta/me/notifications/
Content-type: application/json

{
    "targetHostName": "graphnotifications.sample.windows.com",
    "appNotificationId": "testDirectToastNotification",
    "expirationDateTime": "2019-10-30T23:59:00.000Z",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    },
    "targetPolicy": {
        "platformTypes": [
    "windows",
    "ios",
    "android"
        ]
    },
    "priority": "High",
    "groupName": "TestGroup",
    "displayTimeToLive": "60"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример соответствующего ответа.

```http
HTTP/1.1 201
client-request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781
content-length: 356
content-type: application/json
location: https://graph.microsoft.com/beta/me/activities/119081f2-f19d-4fa8-817c-7e01092c0f7d
request-id: 71e62feb-8d72-4912-8b2c-4cee9d89e781

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('graphnotify%40contoso.com')/notifications/$entity",
    "displayTimeToLive": 59,
    "expirationDateTime": "2019-10-28T22:05:36.25Z",
    "groupName": "TestGroup",
    "id": "119081f2-f19d-4fa8-817c-7e01092c0f7d",
    "priority": "High",
    "payload": {
        "visualContent": {
            "title": "Hello World!",
            "body": "Notifications are Great!"
        }
    }
}
```


