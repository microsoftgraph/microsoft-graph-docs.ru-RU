---
title: Перечисление объектов joinedTeams
description: Получение команд в Microsoft Teams, непосредственным участником которых является пользователь.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 597274fdd37f93c16d6d5f73e19bff79b207b223
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601813"
---
# <a name="list-joinedteams"></a><span data-ttu-id="84016-103">Перечисление объектов joinedTeams</span><span class="sxs-lookup"><span data-stu-id="84016-103">List joinedTeams</span></span>



<span data-ttu-id="84016-104">Получение [команд](../resources/team.md) в Microsoft Teams, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="84016-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="84016-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84016-105">Permissions</span></span>
<span data-ttu-id="84016-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84016-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84016-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84016-108">Permission type</span></span>      | <span data-ttu-id="84016-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84016-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84016-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84016-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84016-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84016-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="84016-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84016-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84016-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84016-113">Not supported.</span></span>    |
|<span data-ttu-id="84016-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84016-114">Application</span></span> | <span data-ttu-id="84016-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84016-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="84016-116">При использовании делегированных разрешений эта операция поддерживается только для пользователя "Я".</span><span class="sxs-lookup"><span data-stu-id="84016-116">With user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="84016-117">При использовании разрешений для приложений она поддерживается для всех пользователей путем указания определенного идентификатора пользователя. (Псевдоним "Я" не поддерживается при использовании разрешений для приложений.)</span><span class="sxs-lookup"><span data-stu-id="84016-117">With application permissions, it works for all users by specifying  the specific user id. ('me' alias is not supported with application permissions)</span></span>

## <a name="http-request"></a><span data-ttu-id="84016-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84016-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84016-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84016-119">Optional query parameters</span></span>
<span data-ttu-id="84016-120">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="84016-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84016-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84016-121">Request headers</span></span>
| <span data-ttu-id="84016-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="84016-122">Header</span></span>       | <span data-ttu-id="84016-123">Значение</span><span class="sxs-lookup"><span data-stu-id="84016-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="84016-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84016-124">Authorization</span></span>  | <span data-ttu-id="84016-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84016-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="84016-127">Accept</span><span class="sxs-lookup"><span data-stu-id="84016-127">Accept</span></span>  | <span data-ttu-id="84016-128">application/json</span><span class="sxs-lookup"><span data-stu-id="84016-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84016-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84016-129">Request body</span></span>
<span data-ttu-id="84016-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="84016-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84016-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="84016-131">Response</span></span>

<span data-ttu-id="84016-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="84016-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="84016-133">Пример</span><span class="sxs-lookup"><span data-stu-id="84016-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="84016-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="84016-134">Request</span></span>
<span data-ttu-id="84016-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="84016-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="84016-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="84016-136">Response</span></span>
<span data-ttu-id="84016-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="84016-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84016-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84016-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84016-141">C#</span><span class="sxs-lookup"><span data-stu-id="84016-141">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_joinedteams-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84016-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84016-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_joinedteams-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a><span data-ttu-id="84016-143">Дополнительные ресурсы</span><span class="sxs-lookup"><span data-stu-id="84016-143">See also</span></span>
[<span data-ttu-id="84016-144">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="84016-144">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-joinedteams.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
