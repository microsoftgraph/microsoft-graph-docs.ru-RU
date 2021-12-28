---
title: Создание и отправка уведомлений (неподготовленных)
description: Создание и отправка уведомления, нацеленного на пользователя через Microsoft Graph.
ms.localizationpriority: medium
ms.prod: notifications
doc_type: apiPageType
author: merzink
ms.openlocfilehash: 33346ef8a625b08652c3b11d8ac9e4e3b17e6060
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/27/2021
ms.locfileid: "61608915"
---
# <a name="create-and-send-a-notification-deprecated"></a>Создание и отправка уведомлений (неподготовленных)

Пространство имен: microsoft.graph

> [!IMPORTANT]
> API Graph уведомлений Майкрософт обесценилось и прекратит возвращать данные к концу января 2022 г. Дополнительные сведения см. в [Microsoft Azure центрах](/azure/notification-hubs) [](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/) уведомлений в этом блоге.

Создание и отправка уведомления, нацеленного на пользователя через Microsoft Graph. Уведомление хранится в магазине каналов Graph Microsoft и отправляется всем клиентам приложений на всех конечных точках устройства, на которые подписан пользователь.  

## <a name="permissions"></a>Разрешения
Служба приложений не требует дополнительных разрешений на публикацию уведомлений целевому пользователю.  

> [!IMPORTANT]
> Если вместо этого вы решите размещать уведомления от имени пользователя с помощью делегирования разрешений, для вызова этого API требуется одно из следующих разрешений. Мы не рекомендуем этот вариант для создания уведомлений. Если вы хотите узнать больше, в том числе о выборе разрешений, см. [в руб. Разрешения.](/graph/permissions-reference)

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
|Авторизация | Загона авторизации используется для пропуска учетных данных вызываемой стороны. Bearer {token}. Обязательный. |
|X-UNS-ID | UserNotificationSubscriptionId, возвращаемая службой уведомлений Microsoft Graph после создания подписки, используется для целевого использования определенного пользователя. Обязательный параметр. |
|Content-Type | application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляют представление JSON объекта [уведомлений.](../resources/projectrome-notification.md)

## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа, который указывает, что уведомление было успешно создано `201 Created` и сохранено. Впоследствии уведомление будет раздуно во все указанные конечные точки с действительной подпиской. 

В следующей таблице перечислены возможные коды ошибок и ответов, которые можно вернуть.

|Код ошибки             | Descrition                              |
|:-----------------------------------|:----------------------------------------------------------|
|HttpStatusCode.BadRequest           | Body — это массив (несколько уведомлений не поддерживаются).|
|HttpStatusCode.BadRequest           | Body не соответствует контракту для API.               |
|HttpStatusCode.Forbidden            | Вызываемая в списке заблокирована.                          |
|HttpStatusCode.MethodNotAllowed     | Используемый метод HTTP не поддерживается.                     |
|HttpStatusCode.BadRequest           | В запросе присутствуют неподдержные заглавные. Два загона не поддерживаются:<br/><br/>If-Modified-Since<br/>If-Range |                    
|HttpStatusCode.UnsupportedMediaType | Заглавное содержимое-кодирования присутствует и имеет значения алгоритма сжатия, кроме `Deflate` или `Gzip` .  |
|HttpStatusCode.BadRequest           | Недействительный полезной нагрузки.                                           |
|HttpStatusCode.Forbidden            | Вызываемая не уполномочена действовать от имени пользователя или отправлять уведомление пользователю.                         |
|HttpStatusCode.Unauthorized         |    Тело запроса содержит недействительные типы данных о действиях.        |
|HttpStatusCode.OK                   |     Действие успешно создано.                            |
|HttpStatusCode.NotAcceptable        |    Запрос был регулирование или сервер занят.    |


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
Ниже приводится пример соответствующего ответа.

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


