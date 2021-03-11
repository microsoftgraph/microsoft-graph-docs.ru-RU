---
author: learafa
title: Получить конечную точку websocket
description: Использование этих API в производственных приложениях не поддерживается.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e56a4174808a7b30ecf063c2b782e0be272c6046
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721462"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="d0b2e-103">Получить конечную точку websocket</span><span class="sxs-lookup"><span data-stu-id="d0b2e-103">Get websocket endpoint</span></span>

<span data-ttu-id="d0b2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="d0b2e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0b2e-106">Позволяет получать уведомления об изменениях в режиме [][] реального времени для диска и списка с помощью [socket.io.][] [][]</span><span class="sxs-lookup"><span data-stu-id="d0b2e-106">Allows you to receive near-real-time change notifications for a [drive][] and [list][] using [socket.io][].</span></span>
<span data-ttu-id="d0b2e-107">Socket.io — это популярная библиотека уведомлений для JavaScript, которая использует WebSockets.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-107">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="d0b2e-108">Подробнее см. в [socket.io.](https://socket.io)</span><span class="sxs-lookup"><span data-stu-id="d0b2e-108">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[list]: ../resources/list.md
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="d0b2e-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b2e-112">Permissions</span></span>

<span data-ttu-id="d0b2e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0b2e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0b2e-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0b2e-115">Permission type</span></span>                        | <span data-ttu-id="d0b2e-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0b2e-116">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="d0b2e-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0b2e-117">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0b2e-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b2e-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="d0b2e-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0b2e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0b2e-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0b2e-120">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="d0b2e-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0b2e-121">Application</span></span>                            | <span data-ttu-id="d0b2e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-122">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="d0b2e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0b2e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /drives/{driveId}/list/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="d0b2e-124">Пример</span><span class="sxs-lookup"><span data-stu-id="d0b2e-124">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0b2e-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0b2e-125">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d0b2e-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0b2e-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```msgraph-interactive
GET /me/drive/root/subscriptions/socketIo
```
# <a name="c"></a>[<span data-ttu-id="d0b2e-127">C#</span><span class="sxs-lookup"><span data-stu-id="d0b2e-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/drive-root-subscriptions-socketio-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0b2e-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0b2e-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/drive-root-subscriptions-socketio-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0b2e-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0b2e-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/drive-root-subscriptions-socketio-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0b2e-130">Java</span><span class="sxs-lookup"><span data-stu-id="d0b2e-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/drive-root-subscriptions-socketio-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0b2e-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0b2e-131">Response</span></span>

<span data-ttu-id="d0b2e-132">В случае успешного использования этот метод возвращает код отклика и объект подписки `200 OK` в тексте [](../resources/subscription.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-132">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="d0b2e-133">Возвращенный `notificationUrl` URL-адрес socket.io конечной точки.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-133">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="d0b2e-134">Чтобы использовать его с socket.io клиентом, разделите строку на `/callback?` маркер.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-134">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="d0b2e-135">Часть строки до этого — socket.io конечной точки, а часть строки после — непрозрачной строки запроса, которая должна быть передана `/callback?` библиотеке.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-135">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="d0b2e-136">В следующем примере показано, как использовать `notificationUrl` socket.io JavaScript.</span><span class="sxs-lookup"><span data-stu-id="d0b2e-136">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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


