---
title: 'teamsAppInstallation: обновление'
description: Обновление приложения, установленного в чате, и его синхронизация с текущей версией, доступной в каталоге приложений клиента.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9da26926b9e41c7c4897744d9cb062a36003af4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776125"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="90b35-103">teamsAppInstallation: обновление</span><span class="sxs-lookup"><span data-stu-id="90b35-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="90b35-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90b35-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90b35-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="90b35-105">Upgrade an [app installation](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="90b35-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp**, установленный для собрания, будет обновлен.</span><span class="sxs-lookup"><span data-stu-id="90b35-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then effectively, the **teamsApp** installed in the meeting will get upgraded.</span></span>

## <a name="permissions"></a><span data-ttu-id="90b35-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90b35-107">Permissions</span></span>

<span data-ttu-id="90b35-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90b35-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90b35-110">Permission type</span></span>      | <span data-ttu-id="90b35-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90b35-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90b35-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90b35-112">Delegated (work or school account)</span></span> | <span data-ttu-id="90b35-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="90b35-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="90b35-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90b35-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90b35-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90b35-115">Not supported.</span></span>   |
|<span data-ttu-id="90b35-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="90b35-116">Application</span></span> | <span data-ttu-id="90b35-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="90b35-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90b35-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90b35-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /chats/{chat-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="response"></a><span data-ttu-id="90b35-119">Отклик</span><span class="sxs-lookup"><span data-stu-id="90b35-119">Response</span></span>

<span data-ttu-id="90b35-120">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="90b35-120">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="90b35-121">Пример</span><span class="sxs-lookup"><span data-stu-id="90b35-121">Example</span></span>

### <a name="request"></a><span data-ttu-id="90b35-122">Запрос</span><span class="sxs-lookup"><span data-stu-id="90b35-122">Request</span></span>

<span data-ttu-id="90b35-123">В следующем примере обновляется приложение, установленное в чате.</span><span class="sxs-lookup"><span data-stu-id="90b35-123">The following example upgrades an app installed in a chat.</span></span>

<!-- {
  "blockType": "request",
  "name": "upgrade_installedApps_in_chat"
}-->

```http
POST https://graph.microsoft.com/v1.0/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps/NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=/upgrade
```


### <a name="response"></a><span data-ttu-id="90b35-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="90b35-124">Response</span></span>

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
