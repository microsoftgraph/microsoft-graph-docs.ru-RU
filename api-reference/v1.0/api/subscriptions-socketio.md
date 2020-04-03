---
author: daspek
ms.author: dspektor
title: Получение конечной точки WebSocket
localization_priority: Normal
ms.prod: sharepoint
description: Позволяет получать уведомления об изменении почти в режиме реального времени для диска с помощью socket.io.
doc_type: apiPageType
ms.openlocfilehash: 3249bba061257b4bae715734ab4e3ba348131c63
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109159"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="65cf8-103">Получение конечной точки WebSocket</span><span class="sxs-lookup"><span data-stu-id="65cf8-103">Get websocket endpoint</span></span>

<span data-ttu-id="65cf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65cf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65cf8-105">Позволяет получать уведомления об изменении почти в режиме реального времени для [диска][] и [списка][] с помощью [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="65cf8-105">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="65cf8-106">Socket.io — это популярная библиотека уведомлений для JavaScript, использующая WebSocket.</span><span class="sxs-lookup"><span data-stu-id="65cf8-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="65cf8-107">Дополнительные сведения см. в разделе [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="65cf8-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="65cf8-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65cf8-111">Permissions</span></span>

<span data-ttu-id="65cf8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65cf8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65cf8-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65cf8-114">Permission type</span></span>                        | <span data-ttu-id="65cf8-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65cf8-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="65cf8-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65cf8-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="65cf8-117">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="65cf8-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="65cf8-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65cf8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65cf8-119">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65cf8-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="65cf8-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65cf8-120">Application</span></span>                            | <span data-ttu-id="65cf8-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65cf8-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="65cf8-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65cf8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /lists/{list-id}/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="65cf8-123">Пример</span><span class="sxs-lookup"><span data-stu-id="65cf8-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="65cf8-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="65cf8-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="65cf8-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="65cf8-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="65cf8-126">C#</span><span class="sxs-lookup"><span data-stu-id="65cf8-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65cf8-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65cf8-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65cf8-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65cf8-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65cf8-129">Java</span><span class="sxs-lookup"><span data-stu-id="65cf8-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65cf8-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="65cf8-130">Response</span></span>

<span data-ttu-id="65cf8-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="65cf8-131">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="65cf8-132">`notificationUrl` Возвращаемый параметр является URL-адресом конечной точки Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="65cf8-132">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>

<span data-ttu-id="65cf8-133">В приведенном ниже примере показано, `notificationUrl` как использовать with Socket.IO в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="65cf8-133">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

```javascript
// this is the notificationUrl returned from this API
var notificationUrl = "https://f3hb0mpua.svc.ms/zbaehwg/callback?snthgk=1ff3-2345672zz831837523";

// 'io' comes from the socket.io client library
var socket = io(notificationUrl);

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
