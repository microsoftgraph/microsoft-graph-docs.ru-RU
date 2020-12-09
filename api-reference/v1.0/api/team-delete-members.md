---
title: Удаление участника из группы
description: Удаление conversationMember из группы.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 975b8f9c3f4ed75b90dd62be9d417a8941f9d510
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524649"
---
# <a name="remove-member-from-team"></a><span data-ttu-id="40ca1-103">Удаление участника из группы</span><span class="sxs-lookup"><span data-stu-id="40ca1-103">Remove member from team</span></span>
<span data-ttu-id="40ca1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40ca1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="40ca1-105">Удаление [conversationMember](../resources/conversationmember.md) из [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="40ca1-105">Remove a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="40ca1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40ca1-106">Permissions</span></span>
<span data-ttu-id="40ca1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40ca1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40ca1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40ca1-109">Permission type</span></span>|<span data-ttu-id="40ca1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40ca1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40ca1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40ca1-111">Delegated (work or school account)</span></span>| <span data-ttu-id="40ca1-112">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ca1-112">TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="40ca1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40ca1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40ca1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40ca1-114">Not supported.</span></span>    |
|<span data-ttu-id="40ca1-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="40ca1-115">Application</span></span>| <span data-ttu-id="40ca1-116">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40ca1-116">TeamMember.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="40ca1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40ca1-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /teams/{team-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="40ca1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40ca1-118">Request headers</span></span>
|<span data-ttu-id="40ca1-119">Имя</span><span class="sxs-lookup"><span data-stu-id="40ca1-119">Name</span></span>|<span data-ttu-id="40ca1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40ca1-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="40ca1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40ca1-121">Authorization</span></span>|<span data-ttu-id="40ca1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="40ca1-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="40ca1-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40ca1-124">Request body</span></span>
<span data-ttu-id="40ca1-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40ca1-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40ca1-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ca1-126">Response</span></span>

<span data-ttu-id="40ca1-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="40ca1-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="40ca1-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="40ca1-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40ca1-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="40ca1-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40ca1-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="40ca1-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_team"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="40ca1-131">C#</span><span class="sxs-lookup"><span data-stu-id="40ca1-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40ca1-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40ca1-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40ca1-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40ca1-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40ca1-134">Java</span><span class="sxs-lookup"><span data-stu-id="40ca1-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="40ca1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="40ca1-135">Response</span></span>
<span data-ttu-id="40ca1-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="40ca1-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="40ca1-137">См. также</span><span class="sxs-lookup"><span data-stu-id="40ca1-137">See also</span></span>

- [<span data-ttu-id="40ca1-138">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="40ca1-138">Remove member from channel</span></span>](channel-delete-members.md)
