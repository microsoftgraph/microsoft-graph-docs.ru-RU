---
author: learafa
ms.author: learafa
title: Получение конечной точки WebSocket
description: Использование этих API в производственных приложениях не поддерживается.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 067fc455a0a122761c45ac1078712ea04b68845c
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109192"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="dc903-103">Получение конечной точки WebSocket</span><span class="sxs-lookup"><span data-stu-id="dc903-103">Get websocket endpoint</span></span>

<span data-ttu-id="dc903-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc903-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="dc903-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc903-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc903-106">Позволяет получать уведомления об изменении почти в режиме реального времени для [диска][] и [списка][] с помощью [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="dc903-106">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="dc903-107">Socket.io — это популярная библиотека уведомлений для JavaScript, использующая WebSocket.</span><span class="sxs-lookup"><span data-stu-id="dc903-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="dc903-108">Дополнительные сведения см. в разделе [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="dc903-108">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="dc903-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc903-112">Permissions</span></span>

<span data-ttu-id="dc903-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc903-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc903-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc903-115">Permission type</span></span>                        | <span data-ttu-id="dc903-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc903-116">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="dc903-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc903-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc903-118">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="dc903-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="dc903-119">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc903-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc903-120">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dc903-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="dc903-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc903-121">Application</span></span>                            | <span data-ttu-id="dc903-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc903-122">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="dc903-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc903-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /lists/{list-id}/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="dc903-124">Пример</span><span class="sxs-lookup"><span data-stu-id="dc903-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc903-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc903-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dc903-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc903-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="dc903-127">C#</span><span class="sxs-lookup"><span data-stu-id="dc903-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc903-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc903-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc903-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc903-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dc903-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc903-130">Response</span></span>

<span data-ttu-id="dc903-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc903-131">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="dc903-132">`notificationUrl` Возвращаемый параметр является URL-адресом конечной точки Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="dc903-132">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="dc903-133">Чтобы использовать его с клиентом socket.io, разделите строку на `/callback?` маркере.</span><span class="sxs-lookup"><span data-stu-id="dc903-133">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="dc903-134">Часть строки Before `/callback?` является URL-адресом конечной точки Socket.IO, а часть строки After — непрозрачной строкой запроса, которую необходимо присвоить библиотеке.</span><span class="sxs-lookup"><span data-stu-id="dc903-134">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="dc903-135">В приведенном ниже примере показано, `notificationUrl` как использовать with Socket.IO в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="dc903-135">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
  ]
}-->
