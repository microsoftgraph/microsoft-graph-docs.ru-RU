---
title: Удаление участников из группы
description: Удаление Конверсатионмембер из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2dc5359684f0b4d73f08551ea720dc095f482337
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091447"
---
# <a name="delete-members"></a><span data-ttu-id="c0c0e-103">Удаление элементов</span><span class="sxs-lookup"><span data-stu-id="c0c0e-103">Delete members</span></span>
<span data-ttu-id="c0c0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0c0e-105">Удаление нового [конверсатионмембер](../resources/conversationmember.md) из [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c0c0e-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c0c0e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c0e-106">Permissions</span></span>
<span data-ttu-id="c0c0e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c0c0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c0e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c0e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0c0e-109">Permission type</span></span>|<span data-ttu-id="c0c0e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c0e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c0c0e-112">Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c0c0e-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="c0c0e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0c0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c0e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-114">Not supported.</span></span>    |
|<span data-ttu-id="c0c0e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0c0e-115">Application</span></span>| <span data-ttu-id="c0c0e-116">Теаммембер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c0c0e-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c0e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0c0e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{member-id}
```

## <a name="request-headers"></a><span data-ttu-id="c0c0e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0c0e-118">Request headers</span></span>
|<span data-ttu-id="c0c0e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c0c0e-119">Name</span></span>|<span data-ttu-id="c0c0e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0c0e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c0c0e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0c0e-121">Authorization</span></span>|<span data-ttu-id="c0c0e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-122">Bearer {token}.</span></span> <span data-ttu-id="c0c0e-123">Required.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-123">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c0e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c0c0e-124">Request body</span></span>
<span data-ttu-id="c0c0e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c0e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c0e-126">Response</span></span>

<span data-ttu-id="c0c0e-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c0c0e-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="c0c0e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c0c0e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0c0e-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c0c0e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c0e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="c0c0e-131">C#</span><span class="sxs-lookup"><span data-stu-id="c0c0e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0c0e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0c0e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0c0e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0c0e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="c0c0e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0c0e-134">Response</span></span>
<span data-ttu-id="c0c0e-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0c0e-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

