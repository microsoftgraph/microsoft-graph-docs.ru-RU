---
author: daspek
ms.author: dspektor
title: Получение конечной точки WebSocket
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 4d4577ea69c65d6ce003af96b0d96b55fe178fb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562757"
---
# <a name="get-websocket-endpoint"></a><span data-ttu-id="550bc-102">Получение конечной точки WebSocket</span><span class="sxs-lookup"><span data-stu-id="550bc-102">Get websocket endpoint</span></span>

<span data-ttu-id="550bc-103">Позволяет получать уведомления об изменении почти в режиме реального времени для [диска][] с помощью [Socket.IO][].</span><span class="sxs-lookup"><span data-stu-id="550bc-103">Allows you to receive near-real-time change notifications for a [drive][] using [socket.io][].</span></span>
<span data-ttu-id="550bc-104">Socket.io — это популярная библиотека уведомлений для JavaScript, использующая WebSocket.</span><span class="sxs-lookup"><span data-stu-id="550bc-104">Socket.io is a popular notifications library for JavaScript that utilizes WebSockets.</span></span> <span data-ttu-id="550bc-105">Дополнительные сведения см. в разделе [Socket.IO](https://socket.io).</span><span class="sxs-lookup"><span data-stu-id="550bc-105">To learn more, see [socket.io](https://socket.io).</span></span>

[drive]: ../resources/drive.md
[Socket.IO]: https://socket.io/
[socket.io]: https://socket.io/

## <a name="permissions"></a><span data-ttu-id="550bc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="550bc-108">Permissions</span></span>

<span data-ttu-id="550bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="550bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="550bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="550bc-111">Permission type</span></span>                        | <span data-ttu-id="550bc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="550bc-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="550bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="550bc-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="550bc-114">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL, sites. ReadWrite. ALL.</span><span class="sxs-lookup"><span data-stu-id="550bc-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="550bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="550bc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="550bc-116">Files. Read, Files. ReadWrite, Files. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="550bc-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="550bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="550bc-117">Application</span></span>                            | <span data-ttu-id="550bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550bc-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="550bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="550bc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive/root/subscriptions/socketIo
GET /drives/{driveId}/root/subscriptions/socketIo
GET /groups/{groupId}/drive/root/subscriptions/socketIo
GET /sites/{siteId}/lists/{listId}/drive/root/subscriptions/socketIo
```

## <a name="example"></a><span data-ttu-id="550bc-120">Пример</span><span class="sxs-lookup"><span data-stu-id="550bc-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="550bc-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="550bc-121">Request</span></span>

<!-- { "blockType": "request", "name": "drive_root_subscriptions_socketIo" } -->
```http
GET /me/drive/root/subscriptions/socketIo
```

### <a name="response"></a><span data-ttu-id="550bc-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="550bc-122">Response</span></span>

<span data-ttu-id="550bc-123">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Subscription](../resources/subscription.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="550bc-123">If successful, this method returns a `200 OK` response code and a [subscription](../resources/subscription.md) object in the response body.</span></span>

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

<span data-ttu-id="550bc-124">`notificationUrl` Возвращаемый параметр является URL-адресом конечной точки Socket.IO.</span><span class="sxs-lookup"><span data-stu-id="550bc-124">The `notificationUrl` returned is a socket.io endpoint URL.</span></span>
<span data-ttu-id="550bc-125">Чтобы использовать его с клиентом socket.io, разделите строку на `/callback?` маркере.</span><span class="sxs-lookup"><span data-stu-id="550bc-125">To use it with a socket.io client, split the string on the `/callback?` token.</span></span>
<span data-ttu-id="550bc-126">Часть строки Before `/callback?` является URL-адресом конечной точки Socket.IO, а часть строки After — непрозрачной строкой запроса, которую необходимо присвоить библиотеке.</span><span class="sxs-lookup"><span data-stu-id="550bc-126">The part of the string before `/callback?` is the socket.io endpoint URL and the part of the string after is an opaque query string that must be given to the libary.</span></span>

<span data-ttu-id="550bc-127">В приведенном ниже примере показано, `notificationUrl` как использовать with Socket.IO в JavaScript.</span><span class="sxs-lookup"><span data-stu-id="550bc-127">The following example shows how to use the `notificationUrl` with socket.io in JavaScript.</span></span>

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

