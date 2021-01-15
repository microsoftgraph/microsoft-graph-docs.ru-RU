---
title: Удаление участника из группы
description: Удаление conversationMember из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97e6b940abd02e409531f9872393583320f88eba
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49873012"
---
# <a name="remove-member-from-team"></a><span data-ttu-id="80475-103">Удаление участника из группы</span><span class="sxs-lookup"><span data-stu-id="80475-103">Remove member from team</span></span>
<span data-ttu-id="80475-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80475-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80475-105">Удаление [conversationMember](../resources/conversationmember.md) из [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="80475-105">Remove a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="80475-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="80475-106">Permissions</span></span>
<span data-ttu-id="80475-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80475-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80475-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="80475-109">Permission type</span></span>|<span data-ttu-id="80475-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="80475-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80475-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="80475-111">Delegated (work or school account)</span></span>| <span data-ttu-id="80475-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80475-112">TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="80475-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="80475-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80475-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="80475-114">Not supported.</span></span>    |
|<span data-ttu-id="80475-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="80475-115">Application</span></span>| <span data-ttu-id="80475-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80475-116">TeamMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80475-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="80475-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="80475-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="80475-118">Request headers</span></span>
|<span data-ttu-id="80475-119">Имя</span><span class="sxs-lookup"><span data-stu-id="80475-119">Name</span></span>|<span data-ttu-id="80475-120">Описание</span><span class="sxs-lookup"><span data-stu-id="80475-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="80475-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="80475-121">Authorization</span></span>|<span data-ttu-id="80475-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="80475-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="80475-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="80475-124">Request body</span></span>
<span data-ttu-id="80475-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="80475-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="80475-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="80475-126">Response</span></span>

<span data-ttu-id="80475-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80475-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="80475-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="80475-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="80475-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="80475-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="80475-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="80475-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="80475-131">C#</span><span class="sxs-lookup"><span data-stu-id="80475-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80475-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80475-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80475-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80475-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80475-134">Java</span><span class="sxs-lookup"><span data-stu-id="80475-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="80475-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="80475-135">Response</span></span>
<span data-ttu-id="80475-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="80475-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="80475-137">См. также</span><span class="sxs-lookup"><span data-stu-id="80475-137">See also</span></span>

- [<span data-ttu-id="80475-138">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="80475-138">Remove member from channel</span></span>](channel-delete-members.md)

