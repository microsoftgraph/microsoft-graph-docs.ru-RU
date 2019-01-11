---
title: Получение конечной точки websocket
description: Использование этих API в производственных приложениях не поддерживается.
localization_priority: Normal
ms.openlocfilehash: a981a4d02d2e40fec0cb2bca397c7b7794d36867
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859796"
---
# <a name="get-websocket-endpoint"></a>Получение конечной точки websocket

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.
Использование этих API в производственных приложениях не поддерживается.

Позволяет получать уведомления об изменении рядом с режиме реального времени для [диска][] с помощью [socket.io][].
Socket.IO — это библиотека популярные уведомления для JavaScript, который использует WebSockets. Чтобы получить дополнительные сведения, обратитесь к разделу [socket.io](https://socket.io).

[диск]: ../resources/drive.md
[Socket.IO]: https://socket.io/

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий)
|:---------------------------------------|:-------------------------------------------
| Делегированные (рабочая или учебная учетная запись)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Делегированные (личная учетная запись Майкрософт) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Для приложений                            | Не поддерживается.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a>Ответ

Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [подписки](../resources/subscription.md) в теле ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "opaqueId-fj3hd7yf283jfk193726nvc2w3i2diemdu8",
  "notificationUrl": "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523"
}
```

`notificationUrl` Возвращаемые — это URL-адрес конечной точки socket.io.
Чтобы использовать его с помощью клиента socket.io, разделение строки на `/callback?` маркеров.
Часть строки до `/callback?` — это URL-адрес конечной точки socket.io и часть строки после представляет собой строку непрозрачный запроса, которое должно быть задано в библиотеку.

Следующий пример демонстрирует использование `notificationUrl` с socket.io в JavaScript.

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// after the split, split[0] will be everything leading up to '/callback?' and split[1] will be everything after.
var split = notificationUrl.split("/callback?");

// 'io' comes from the socket.io client library
var socket = io(split[0], { query: split[1] });

// these examples log to the console.
// your app would provide its own callbacks
socket.on("connect", ()=>console.log("Connected!"));
socket.on("notification", (data)=>console.log("Notification!", data));
```

<!-- {
  "type": "#page.annotation"
}-->
