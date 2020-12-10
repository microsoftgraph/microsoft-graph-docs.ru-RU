---
title: Удаление приложения в чате
description: Удалить (удалить) приложение, установленное в чате.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a463fd0c57f707c766367b2bd6e7abc326d35aa2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607626"
---
# <a name="uninstall-app-in-a-chat"></a><span data-ttu-id="00ca2-103">Удаление приложения в чате</span><span class="sxs-lookup"><span data-stu-id="00ca2-103">Uninstall app in a chat</span></span>

<span data-ttu-id="00ca2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00ca2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00ca2-105">Удаление [приложения](../resources/teamsapp.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="00ca2-105">Uninstall an [app](../resources/teamsapp.md) installed within a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="00ca2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00ca2-106">Permissions</span></span>

<span data-ttu-id="00ca2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00ca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ca2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00ca2-109">Permission type</span></span>      | <span data-ttu-id="00ca2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00ca2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00ca2-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00ca2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00ca2-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="00ca2-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="00ca2-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00ca2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00ca2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00ca2-114">Not supported.</span></span>   |
|<span data-ttu-id="00ca2-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="00ca2-115">Application</span></span> | <span data-ttu-id="00ca2-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="00ca2-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00ca2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00ca2-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
DELETE /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="response"></a><span data-ttu-id="00ca2-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ca2-118">Response</span></span>

<span data-ttu-id="00ca2-119">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="00ca2-119">If successful this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="00ca2-120">Пример</span><span class="sxs-lookup"><span data-stu-id="00ca2-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="00ca2-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="00ca2-121">Request</span></span>

<span data-ttu-id="00ca2-122">В следующем примере удаляется приложение из указанного чата.</span><span class="sxs-lookup"><span data-stu-id="00ca2-122">The following example uninstalls an app from the specified chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_installedApps_in_chat"
}-->

```http
DELETE https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=
```

### <a name="response"></a><span data-ttu-id="00ca2-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="00ca2-123">Response</span></span>

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
