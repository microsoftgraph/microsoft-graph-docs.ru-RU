---
author: daspek
title: Получить конечную точку websocket
localization_priority: Normal
ms.prod: sharepoint
description: Позволяет получать уведомления об изменениях диска в режиме реального времени с помощью socket.io.
doc_type: apiPageType
ms.openlocfilehash: 2868ba963114bc78053c6098996b6cff597572d9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238444"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="69dc6-103">Получить конечную точку websocket</span><span class="sxs-lookup"><span data-stu-id="69dc6-103">Get websocket endpoint</span></span>

<span data-ttu-id="69dc6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69dc6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69dc6-105">Позволяет получать уведомления об изменениях диска и [][] списка в [][]режиме реального времени с помощью [socket.io.][]</span><span class="sxs-lookup"><span data-stu-id="69dc6-105">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="69dc6-106">Socket.io является популярной библиотекой уведомлений для JavaScript, которая использует WebSockets.</span><span class="sxs-lookup"><span data-stu-id="69dc6-106">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="69dc6-107">Дополнительные узнать см. [в socket.io.](https://socket.io)</span><span class="sxs-lookup"><span data-stu-id="69dc6-107">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="69dc6-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69dc6-111">Permissions</span></span>

<span data-ttu-id="69dc6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69dc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69dc6-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69dc6-114">Permission type</span></span>                        | <span data-ttu-id="69dc6-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69dc6-115">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="69dc6-116">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69dc6-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="69dc6-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69dc6-117">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="69dc6-118">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69dc6-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69dc6-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69dc6-119">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="69dc6-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69dc6-120">Application</span></span>                            | <span data-ttu-id="69dc6-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69dc6-121">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="69dc6-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69dc6-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /lists/{list-id}/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="69dc6-123">Пример</span><span class="sxs-lookup"><span data-stu-id="69dc6-123">Example</span></span>

### <a name="request"></a><span data-ttu-id="69dc6-124">Запрос</span><span class="sxs-lookup"><span data-stu-id="69dc6-124">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="69dc6-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="69dc6-125">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="69dc6-126">C#</span><span class="sxs-lookup"><span data-stu-id="69dc6-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69dc6-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69dc6-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="69dc6-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="69dc6-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69dc6-129">Java</span><span class="sxs-lookup"><span data-stu-id="69dc6-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69dc6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="69dc6-130">Response</span></span>

<span data-ttu-id="69dc6-131">В случае успеха этот метод возвращает код отклика и `200 OK` объект [подписки](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="69dc6-131">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="69dc6-132">Возвращается `notificationUrl` URL-адрес socket.io конечной точки.</span><span class="sxs-lookup"><span data-stu-id="69dc6-132">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>

<span data-ttu-id="69dc6-133">В следующем примере показано, как использовать `notificationUrl` socket.io в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="69dc6-133">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

