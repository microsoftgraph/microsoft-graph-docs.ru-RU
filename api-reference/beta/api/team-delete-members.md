---
title: Удаление участников из группы
description: Удаление conversationMember из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d76456123f3d60428feb213b0ef8901b03db3fa1
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124137"
---
# <a name="delete-members"></a><span data-ttu-id="8eacd-103">Удаление участников</span><span class="sxs-lookup"><span data-stu-id="8eacd-103">Delete members</span></span>
<span data-ttu-id="8eacd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eacd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8eacd-105">Удаление нового [conversationMember](../resources/conversationmember.md) из [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="8eacd-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eacd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8eacd-106">Permissions</span></span>
<span data-ttu-id="8eacd-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8eacd-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8eacd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eacd-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eacd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8eacd-109">Permission type</span></span>|<span data-ttu-id="8eacd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8eacd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eacd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8eacd-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8eacd-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eacd-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="8eacd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8eacd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8eacd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8eacd-114">Not supported.</span></span>    |
|<span data-ttu-id="8eacd-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8eacd-115">Application</span></span>| <span data-ttu-id="8eacd-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eacd-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eacd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8eacd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{member-id}
```

## <a name="request-headers"></a><span data-ttu-id="8eacd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8eacd-118">Request headers</span></span>
|<span data-ttu-id="8eacd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8eacd-119">Name</span></span>|<span data-ttu-id="8eacd-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8eacd-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8eacd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8eacd-121">Authorization</span></span>|<span data-ttu-id="8eacd-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8eacd-122">Bearer {token}.</span></span> <span data-ttu-id="8eacd-123">Required.</span><span class="sxs-lookup"><span data-stu-id="8eacd-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eacd-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8eacd-124">Request body</span></span>
<span data-ttu-id="8eacd-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8eacd-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8eacd-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eacd-126">Response</span></span>

<span data-ttu-id="8eacd-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8eacd-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="8eacd-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="8eacd-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8eacd-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8eacd-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8eacd-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="8eacd-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="8eacd-131">C#</span><span class="sxs-lookup"><span data-stu-id="8eacd-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8eacd-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8eacd-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8eacd-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8eacd-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="8eacd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="8eacd-134">Response</span></span>
<span data-ttu-id="8eacd-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8eacd-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

