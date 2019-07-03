---
author: daspek
ms.author: dspektor
title: Получение конечной точки WebSocket
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 56a932010801963b4e95bd0009fef0c982c89893
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446040"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="2d10c-102">Получение конечной точки WebSocket</span><span class="sxs-lookup"><span data-stu-id="2d10c-102">Get websocket endpoint</span></span>

<span data-ttu-id="2d10c-103">Позволяет получать уведомления об изменении почти в режиме реального времени для [диска][] с помощью [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="2d10c-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="2d10c-104">Socket.io — это популярная библиотека уведомлений для JavaScript, использующая WebSocket.</span><span class="sxs-lookup"><span data-stu-id="2d10c-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="2d10c-105">Дополнительные сведения см. в разделе [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="2d10c-105">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="2d10c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d10c-108">Permissions</span></span>

<span data-ttu-id="2d10c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d10c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2d10c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d10c-111">Permission type</span></span>                        | <span data-ttu-id="2d10c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d10c-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="2d10c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d10c-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="2d10c-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="2d10c-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="2d10c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d10c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d10c-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2d10c-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="2d10c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d10c-117">Application</span></span>                            | <span data-ttu-id="2d10c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2d10c-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="2d10c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d10c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="2d10c-120">Пример</span><span class="sxs-lookup"><span data-stu-id="2d10c-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d10c-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d10c-121">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2d10c-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d10c-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2d10c-123">C#</span><span class="sxs-lookup"><span data-stu-id="2d10c-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2d10c-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="2d10c-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2d10c-125">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2d10c-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2d10c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d10c-126">Response</span></span>

<span data-ttu-id="2d10c-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2d10c-127">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="2d10c-128">`notificationUrl` Возвращаемый параметр является URL-адресом конечной точки Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="2d10c-128">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="2d10c-129">Чтобы использовать его с клиентом socket.io, разделите строку на `/callback?` маркере.</span><span class="sxs-lookup"><span data-stu-id="2d10c-129">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="2d10c-130">Часть строки Before `/callback?` является URL-адресом конечной точки Socket.IO, а часть строки After — непрозрачной строкой запроса, которую необходимо присвоить библиотеке.</span><span class="sxs-lookup"><span data-stu-id="2d10c-130">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="2d10c-131">В приведенном ниже примере показано, `notificationUrl` как использовать with Socket.IO в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="2d10c-131">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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
