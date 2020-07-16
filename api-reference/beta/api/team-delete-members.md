---
title: Удаление участников из группы
description: Удаление conversationMember из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ffce12f12288c7d184a5fd0a591ca6c48dac59c
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142271"
---
# <a name="delete-members"></a><span data-ttu-id="a4538-103">Удаление участников</span><span class="sxs-lookup"><span data-stu-id="a4538-103">Delete members</span></span>
<span data-ttu-id="a4538-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4538-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4538-105">Удаление нового [conversationMember](../resources/conversationmember.md) из [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a4538-105">Remove a new [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a4538-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4538-106">Permissions</span></span>
<span data-ttu-id="a4538-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4538-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4538-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4538-109">Permission type</span></span>|<span data-ttu-id="a4538-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4538-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4538-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4538-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a4538-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4538-112">TeamMember.ReadWrite.All</span></span>|
|<span data-ttu-id="a4538-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4538-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4538-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4538-114">Not supported.</span></span>    |
|<span data-ttu-id="a4538-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a4538-115">Application</span></span>| <span data-ttu-id="a4538-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4538-116">TeamMember.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4538-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4538-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{member-id}
```

## <a name="request-headers"></a><span data-ttu-id="a4538-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4538-118">Request headers</span></span>
|<span data-ttu-id="a4538-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a4538-119">Name</span></span>|<span data-ttu-id="a4538-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a4538-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a4538-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a4538-121">Authorization</span></span>|<span data-ttu-id="a4538-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4538-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4538-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4538-124">Request body</span></span>
<span data-ttu-id="a4538-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4538-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4538-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4538-126">Response</span></span>

<span data-ttu-id="a4538-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4538-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="a4538-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a4538-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a4538-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4538-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a4538-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4538-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/{teamsId}/members
```
# <a name="c"></a>[<span data-ttu-id="a4538-131">C#</span><span class="sxs-lookup"><span data-stu-id="a4538-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a4538-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4538-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a4538-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4538-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a4538-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4538-134">Response</span></span>
<span data-ttu-id="a4538-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a4538-135">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

