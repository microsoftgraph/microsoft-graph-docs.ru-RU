---
title: Получение участника команды
description: Получение участника команды.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d4cd3f0b9bed2ba469659fb415ba484c030b5417
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781032"
---
# <a name="get-member-of-team"></a><span data-ttu-id="0a3ef-103">Получение участника команды</span><span class="sxs-lookup"><span data-stu-id="0a3ef-103">Get member of team</span></span>

<span data-ttu-id="0a3ef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a3ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a3ef-105">Получение [conversationMember](../resources/conversationmember.md) из [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0a3ef-105">Get a [conversationMember](../resources/conversationmember.md) from a [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a3ef-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3ef-106">Permissions</span></span>

<span data-ttu-id="0a3ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a3ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a3ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0a3ef-109">Permission Type</span></span>|<span data-ttu-id="0a3ef-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0a3ef-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0a3ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0a3ef-111">Delegated (work or school account)</span></span>| <span data-ttu-id="0a3ef-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3ef-112">TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |
|<span data-ttu-id="0a3ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0a3ef-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a3ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-114">Not supported.</span></span>    |
|<span data-ttu-id="0a3ef-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0a3ef-115">Application</span></span>| <span data-ttu-id="0a3ef-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a3ef-116">TeamMember.Read.Group\*, TeamMember.Read.All, TeamMember.ReadWrite.All</span></span> |

> <span data-ttu-id="0a3ef-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="0a3ef-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="0a3ef-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0a3ef-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0a3ef-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0a3ef-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0a3ef-120">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
GET /teams/{team-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a3ef-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0a3ef-121">Optional query parameters</span></span>

<span data-ttu-id="0a3ef-122">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a3ef-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0a3ef-123">Request headers</span></span>

| <span data-ttu-id="0a3ef-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0a3ef-124">Header</span></span>       | <span data-ttu-id="0a3ef-125">Значение</span><span class="sxs-lookup"><span data-stu-id="0a3ef-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a3ef-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0a3ef-126">Authorization</span></span>  | <span data-ttu-id="0a3ef-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a3ef-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0a3ef-129">Request body</span></span>

<span data-ttu-id="0a3ef-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a3ef-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3ef-131">Response</span></span>

<span data-ttu-id="0a3ef-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a3ef-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0a3ef-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a3ef-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0a3ef-134">Request</span></span>

<span data-ttu-id="0a3ef-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a3ef-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a3ef-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-get_member"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```
# <a name="c"></a>[<span data-ttu-id="0a3ef-137">C#</span><span class="sxs-lookup"><span data-stu-id="0a3ef-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-get-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a3ef-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a3ef-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-get-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a3ef-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a3ef-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-get-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a3ef-140">Java</span><span class="sxs-lookup"><span data-stu-id="0a3ef-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-get-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a3ef-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0a3ef-141">Response</span></span>

<span data-ttu-id="0a3ef-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-142">Here is an example of the response.</span></span>

><span data-ttu-id="0a3ef-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0a3ef-143">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/members/microsoft.graph.aadUserConversationMember/$entity",
   "@odata.type":"#microsoft.graph.aadUserConversationMember",
   "id":"/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=",
   "roles":[
      "owner"
   ],
   "displayName":"John Doe",
   "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
   "email":null
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "get_team_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a><span data-ttu-id="0a3ef-144">Дополнительные материалы</span><span class="sxs-lookup"><span data-stu-id="0a3ef-144">See also</span></span>

- [<span data-ttu-id="0a3ef-145">Получение участника канала</span><span class="sxs-lookup"><span data-stu-id="0a3ef-145">Get member of channel</span></span>](channel-get-members.md)

