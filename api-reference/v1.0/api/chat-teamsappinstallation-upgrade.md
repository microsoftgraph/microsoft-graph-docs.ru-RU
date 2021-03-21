---
title: 'teamsAppInstallation: обновление'
description: Обновление приложения, установленного в чате, и его синхронизация с текущей версией, доступной в каталоге приложений клиента.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e193fd03cc83c0e60f137e8610dfa647fbbb3c8c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960034"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="50613-103">teamsAppInstallation: обновление</span><span class="sxs-lookup"><span data-stu-id="50613-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="50613-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50613-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="50613-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="50613-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="50613-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp**, установленный для собрания, будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="50613-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then effectively, the **teamsApp** installed in the meeting will get upgraded.</span></span>

## <a name="permissions"></a><span data-ttu-id="50613-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50613-107">Permissions</span></span>

<span data-ttu-id="50613-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50613-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50613-110">Permission type</span></span>      | <span data-ttu-id="50613-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50613-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50613-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50613-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50613-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="50613-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="50613-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50613-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50613-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50613-115">Not supported.</span></span>   |
|<span data-ttu-id="50613-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="50613-116">Application</span></span> | <span data-ttu-id="50613-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="50613-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50613-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50613-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="50613-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="50613-119">Response</span></span>

<span data-ttu-id="50613-120">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50613-120">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50613-121">Пример</span><span class="sxs-lookup"><span data-stu-id="50613-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="50613-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="50613-122">Request</span></span>

<span data-ttu-id="50613-123">В следующем примере обновляется приложение, установленное в чате.</span><span class="sxs-lookup"><span data-stu-id="50613-123">The following example upgrades an app installed in a chat.</span></span>


# <a name="http"></a>[<span data-ttu-id="50613-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="50613-124">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```
# <a name="c"></a>[<span data-ttu-id="50613-125">C#</span><span class="sxs-lookup"><span data-stu-id="50613-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="50613-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50613-126">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="50613-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="50613-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="50613-128">Java</span><span class="sxs-lookup"><span data-stu-id="50613-128">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="50613-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="50613-129">Response</span></span>

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
  "description": "Chat update installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
