---
title: Удаление приложения в чате
description: Удалить (удалить) приложение, установленное в чате.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 014ef8e056ca117bd1680cb5b0be0595f20d8571
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50770074"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="da781-103">Удаление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="da781-103">Uninstall app in a chat</span></span>

<span data-ttu-id="da781-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da781-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da781-105">Удаление [приложения](../resources/teamsapp.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="da781-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="da781-106">**Примечание**. Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp** будет удален из собрания.</span><span class="sxs-lookup"><span data-stu-id="da781-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="da781-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da781-107">Permissions</span></span>

<span data-ttu-id="da781-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da781-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da781-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da781-110">Permission type</span></span>      | <span data-ttu-id="da781-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da781-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da781-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da781-112">Delegated (work or school account)</span></span> | <span data-ttu-id="da781-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="da781-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="da781-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da781-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da781-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da781-115">Not supported.</span></span>   |
|<span data-ttu-id="da781-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="da781-116">Application</span></span> | <span data-ttu-id="da781-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="da781-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="da781-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da781-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="da781-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da781-119">Request headers</span></span>
|<span data-ttu-id="da781-120">Имя</span><span class="sxs-lookup"><span data-stu-id="da781-120">Name</span></span>|<span data-ttu-id="da781-121">Описание</span><span class="sxs-lookup"><span data-stu-id="da781-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="da781-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da781-122">Authorization</span></span>|<span data-ttu-id="da781-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da781-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="da781-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da781-125">Request body</span></span>
<span data-ttu-id="da781-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da781-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da781-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="da781-127">Response</span></span>

<span data-ttu-id="da781-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="da781-128">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="da781-129">Пример</span><span class="sxs-lookup"><span data-stu-id="da781-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="da781-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="da781-130">Request</span></span>

<span data-ttu-id="da781-131">В следующем примере удаляется приложение из указанного чата.</span><span class="sxs-lookup"><span data-stu-id="da781-131">The following example uninstalls an app from the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="da781-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="da781-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```
# <a name="c"></a>[<span data-ttu-id="da781-133">C#</span><span class="sxs-lookup"><span data-stu-id="da781-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da781-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da781-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da781-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da781-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da781-136">Java</span><span class="sxs-lookup"><span data-stu-id="da781-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="da781-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="da781-137">Response</span></span>

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
