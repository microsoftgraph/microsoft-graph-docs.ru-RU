---
title: Удаление приложения в чате
description: Удалить (удалить) приложение, установленное в чате.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 954567f3d899f432922edb2c1c618814282043c4
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658585"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="3e7fd-103">Удаление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="3e7fd-103">Uninstall app in a chat</span></span>

<span data-ttu-id="3e7fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e7fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e7fd-105">Удаление [приложения](../resources/teamsapp.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="3e7fd-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="3e7fd-106">**Примечание**. Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp** будет удален из собрания.</span><span class="sxs-lookup"><span data-stu-id="3e7fd-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get removed from the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e7fd-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7fd-107">Permissions</span></span>

<span data-ttu-id="3e7fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7fd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7fd-110">Permission type</span></span>      | <span data-ttu-id="3e7fd-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3e7fd-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e7fd-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="3e7fd-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="3e7fd-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e7fd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7fd-115">Not supported.</span></span>   |
|<span data-ttu-id="3e7fd-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="3e7fd-116">Application</span></span> | <span data-ttu-id="3e7fd-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="3e7fd-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e7fd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7fd-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="3e7fd-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7fd-119">Response</span></span>

<span data-ttu-id="3e7fd-120">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3e7fd-120">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3e7fd-121">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7fd-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e7fd-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7fd-122">Request</span></span>

<span data-ttu-id="3e7fd-123">В следующем примере удаляется приложение из указанного чата.</span><span class="sxs-lookup"><span data-stu-id="3e7fd-123">The following example uninstalls an app from the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a><span data-ttu-id="3e7fd-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7fd-124">Response</span></span>

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
