---
title: Получение конечной точки WebSocket
description: Использование этих API в производственных приложениях не поддерживается.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03dbaf8522005c2bb0c038c8ba885becc41f72dc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591823"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="7c399-103">Получение конечной точки WebSocket</span><span class="sxs-lookup"><span data-stu-id="7c399-103">Get websocket endpoint</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="7c399-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c399-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7c399-105">Позволяет получать уведомления об изменении почти в режиме реального времени для [диска][] с помощью [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="7c399-105">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="7c399-106">Socket.io — это популярная библиотека уведомлений для JavaScript, использующая WebSocket.</span><span class="sxs-lookup"><span data-stu-id="7c399-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="7c399-107">Дополнительные сведения см. в разделе [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="7c399-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="7c399-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7c399-110">Permissions</span></span>

<span data-ttu-id="7c399-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c399-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c399-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7c399-113">Permission type</span></span>                        | <span data-ttu-id="7c399-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7c399-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="7c399-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7c399-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c399-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="7c399-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="7c399-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7c399-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c399-118">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="7c399-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="7c399-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7c399-119">Application</span></span>                            | <span data-ttu-id="7c399-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c399-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="7c399-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7c399-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="7c399-122">Пример</span><span class="sxs-lookup"><span data-stu-id="7c399-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c399-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="7c399-123">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="7c399-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="7c399-124">Response</span></span>

<span data-ttu-id="7c399-125">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7c399-125">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7c399-126">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7c399-126">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7c399-127">Языках</span><span class="sxs-lookup"><span data-stu-id="7c399-127">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7c399-128">Язык</span><span class="sxs-lookup"><span data-stu-id="7c399-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/drive_root_subscriptions_socketIo-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="7c399-129">`notificationUrl` Возвращаемый параметр является URL-адресом конечной точки Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="7c399-129">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="7c399-130">Чтобы использовать его с клиентом socket.io, разделите строку на `/callback?` маркере.</span><span class="sxs-lookup"><span data-stu-id="7c399-130">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="7c399-131">Часть строки Before `/callback?` является URL-адресом конечной точки Socket.IO, а часть строки After — непрозрачной строкой запроса, которую необходимо присвоить библиотеке.</span><span class="sxs-lookup"><span data-stu-id="7c399-131">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="7c399-132">В приведенном ниже примере показано, `notificationUrl` как использовать with Socket.IO в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="7c399-132">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveItem-subscriptions-socketio.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
