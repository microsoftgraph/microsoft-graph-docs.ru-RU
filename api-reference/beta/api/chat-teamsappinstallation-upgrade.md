---
title: 'teamsAppInstallation: обновление'
description: Обновление приложения, установленного в чате, и его синхронизация с текущей версией, доступной в каталоге приложений клиента.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c6e012008fc85d3b114ee422ed7eebd67dba6349
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971072"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="e7bdd-103">teamsAppInstallation: обновление</span><span class="sxs-lookup"><span data-stu-id="e7bdd-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="e7bdd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7bdd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7bdd-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="e7bdd-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="e7bdd-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp**, установленный для собрания, будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="e7bdd-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then effectively, the **teamsApp** installed in the meeting will get upgraded.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7bdd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e7bdd-107">Permissions</span></span>

<span data-ttu-id="e7bdd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7bdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7bdd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e7bdd-110">Permission type</span></span>      | <span data-ttu-id="e7bdd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e7bdd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7bdd-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e7bdd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e7bdd-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="e7bdd-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="e7bdd-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e7bdd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7bdd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7bdd-115">Not supported.</span></span>   |
|<span data-ttu-id="e7bdd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e7bdd-116">Application</span></span> | <span data-ttu-id="e7bdd-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="e7bdd-117">Chat.Manage.Chat\*, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="e7bdd-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="e7bdd-118">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="e7bdd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e7bdd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="e7bdd-120">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7bdd-120">Response</span></span>

<span data-ttu-id="e7bdd-121">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e7bdd-121">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e7bdd-122">Пример</span><span class="sxs-lookup"><span data-stu-id="e7bdd-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7bdd-123">Запрос</span><span class="sxs-lookup"><span data-stu-id="e7bdd-123">Request</span></span>

<span data-ttu-id="e7bdd-124">В следующем примере обновляется приложение, установленное в чате.</span><span class="sxs-lookup"><span data-stu-id="e7bdd-124">The following example upgrades an app installed in a chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="e7bdd-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="e7bdd-125">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```
# <a name="c"></a>[<span data-ttu-id="e7bdd-126">C#</span><span class="sxs-lookup"><span data-stu-id="e7bdd-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e7bdd-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7bdd-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e7bdd-128">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e7bdd-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e7bdd-129">Java</span><span class="sxs-lookup"><span data-stu-id="e7bdd-129">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e7bdd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="e7bdd-130">Response</span></span>

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
