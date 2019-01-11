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
# <a name="get-websocket-endpoint"></a><span data-ttu-id="ceb9c-103">Получение конечной точки websocket</span><span class="sxs-lookup"><span data-stu-id="ceb9c-103">Get websocket endpoint</span></span>

> <span data-ttu-id="ceb9c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span>
<span data-ttu-id="ceb9c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ceb9c-106">Позволяет получать уведомления об изменении рядом с режиме реального времени для [диска][] с помощью [socket.io][].</span><span class="sxs-lookup"><span data-stu-id="ceb9c-106">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="ceb9c-107">Socket.IO — это библиотека популярные уведомления для JavaScript, который использует WebSockets.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="ceb9c-108">Чтобы получить дополнительные сведения, обратитесь к разделу [socket.io](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="ceb9c-108">To learn more, see [socket.io](https://socket.io).</span></span>

[диск]: ../resources/drive.md
[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="ceb9c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb9c-111">Permissions</span></span>

<span data-ttu-id="ceb9c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ceb9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ceb9c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ceb9c-114">Permission type</span></span>                        | <span data-ttu-id="ceb9c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ceb9c-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="ceb9c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ceb9c-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="ceb9c-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb9c-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="ceb9c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ceb9c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ceb9c-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ceb9c-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="ceb9c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ceb9c-120">Application</span></span>                            | <span data-ttu-id="ceb9c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="ceb9c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ceb9c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="ceb9c-123">Пример</span><span class="sxs-lookup"><span data-stu-id="ceb9c-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="ceb9c-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="ceb9c-124">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="ceb9c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ceb9c-125">Response</span></span>

<span data-ttu-id="ceb9c-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [подписки](../resources/subscription.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-126">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="ceb9c-127">`notificationUrl` Возвращаемые — это URL-адрес конечной точки socket.io.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-127">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="ceb9c-128">Чтобы использовать его с помощью клиента socket.io, разделение строки на `/callback?` маркеров.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-128">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="ceb9c-129">Часть строки до `/callback?` — это URL-адрес конечной точки socket.io и часть строки после представляет собой строку непрозрачный запроса, которое должно быть задано в библиотеку.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-129">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="ceb9c-130">Следующий пример демонстрирует использование `notificationUrl` с socket.io в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="ceb9c-130">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
