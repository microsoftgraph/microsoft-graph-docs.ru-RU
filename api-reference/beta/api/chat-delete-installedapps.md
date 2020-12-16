---
title: Удаление приложения в чате
description: Удалить (удалить) приложение, установленное в чате.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 212a033198a5bb1b6303b3d1a848ad32da4df5ab
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690109"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="d3286-103">Удаление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="d3286-103">Uninstall app in a chat</span></span>

<span data-ttu-id="d3286-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3286-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3286-105">Удаление [приложения](../resources/teamsapp.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="d3286-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="d3286-106">**Примечание**. Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp** будет удален из собрания.</span><span class="sxs-lookup"><span data-stu-id="d3286-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3286-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3286-107">Permissions</span></span>

<span data-ttu-id="d3286-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3286-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3286-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3286-110">Permission type</span></span>      | <span data-ttu-id="d3286-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3286-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3286-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3286-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3286-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="d3286-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="d3286-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3286-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3286-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3286-115">Not supported.</span></span>   |
|<span data-ttu-id="d3286-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3286-116">Application</span></span> | <span data-ttu-id="d3286-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="d3286-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3286-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3286-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="d3286-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3286-119">Response</span></span>

<span data-ttu-id="d3286-120">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d3286-120">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3286-121">Пример</span><span class="sxs-lookup"><span data-stu-id="d3286-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3286-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3286-122">Request</span></span>

<span data-ttu-id="d3286-123">В следующем примере удаляется приложение из указанного чата.</span><span class="sxs-lookup"><span data-stu-id="d3286-123">The following example uninstalls an app from the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3286-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3286-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="d3286-125">C#</span><span class="sxs-lookup"><span data-stu-id="d3286-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3286-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3286-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3286-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3286-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3286-128">Java</span><span class="sxs-lookup"><span data-stu-id="d3286-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3286-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3286-129">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat delete installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
