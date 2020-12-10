---
title: 'teamsAppInstallation: обновление'
description: Обновление приложения, установленного в чате, и его синхронизация с текущей версией, доступной в каталоге приложений клиента.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f3c68d21a5af7cb724bf0990e3af216ce54a28b4
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607589"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="c2905-103">teamsAppInstallation: обновление</span><span class="sxs-lookup"><span data-stu-id="c2905-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="c2905-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2905-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2905-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="c2905-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2905-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2905-106">Permissions</span></span>

<span data-ttu-id="c2905-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2905-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2905-109">Permission type</span></span>      | <span data-ttu-id="c2905-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2905-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2905-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2905-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2905-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="c2905-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="c2905-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2905-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2905-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2905-114">Not supported.</span></span>   |
|<span data-ttu-id="c2905-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2905-115">Application</span></span> | <span data-ttu-id="c2905-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="c2905-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2905-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2905-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="c2905-118">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2905-118">Response</span></span>

<span data-ttu-id="c2905-119">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2905-119">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2905-120">Пример</span><span class="sxs-lookup"><span data-stu-id="c2905-120">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2905-121">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2905-121">Request</span></span>

<span data-ttu-id="c2905-122">В следующем примере обновляется приложение, установленное в чате.</span><span class="sxs-lookup"><span data-stu-id="c2905-122">The following example upgrades an app installed in a chat.</span></span>
<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```

### <a name="response"></a><span data-ttu-id="c2905-123">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2905-123">Response</span></span>

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
