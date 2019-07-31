---
title: Перечисление объектов joinedTeams
description: Получение команд в Microsoft Teams, непосредственным участником которых является пользователь.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3124f72b30a9ca82efe7f2583a6afc766bed1718
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931487"
---
# <a name="list-joinedteams"></a><span data-ttu-id="96a11-103">Перечисление объектов joinedTeams</span><span class="sxs-lookup"><span data-stu-id="96a11-103">List joinedTeams</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96a11-104">Получение [команд](../resources/team.md) в Microsoft Teams, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="96a11-104">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="96a11-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="96a11-105">Permissions</span></span>
<span data-ttu-id="96a11-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96a11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96a11-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="96a11-108">Permission type</span></span>      | <span data-ttu-id="96a11-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="96a11-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96a11-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="96a11-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96a11-111">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a11-111">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="96a11-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="96a11-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96a11-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96a11-113">Not supported.</span></span>    |
|<span data-ttu-id="96a11-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="96a11-114">Application</span></span> | <span data-ttu-id="96a11-115">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96a11-115">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="96a11-116">В настоящее время при использовании делегированных разрешений эта операция поддерживается только для пользователя "Я".</span><span class="sxs-lookup"><span data-stu-id="96a11-116">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="96a11-117">При использовании разрешений для приложений она поддерживается для всех пользователей путем указания определенного идентификатора пользователя. (Псевдоним "Я" не поддерживается при использовании разрешений для приложений). Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span><span class="sxs-lookup"><span data-stu-id="96a11-117">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="96a11-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="96a11-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96a11-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="96a11-119">Optional query parameters</span></span>
<span data-ttu-id="96a11-120">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="96a11-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96a11-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="96a11-121">Request headers</span></span>
| <span data-ttu-id="96a11-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="96a11-122">Header</span></span>       | <span data-ttu-id="96a11-123">Значение</span><span class="sxs-lookup"><span data-stu-id="96a11-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96a11-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="96a11-124">Authorization</span></span>  | <span data-ttu-id="96a11-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="96a11-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96a11-127">Accept</span><span class="sxs-lookup"><span data-stu-id="96a11-127">Accept</span></span>  | <span data-ttu-id="96a11-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96a11-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96a11-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="96a11-129">Request body</span></span>
<span data-ttu-id="96a11-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="96a11-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96a11-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="96a11-131">Response</span></span>

<span data-ttu-id="96a11-132">При успешном выполнении этот метод возвращает `200 OK`код ответа и коллекцию объектов [team](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="96a11-132">If successful, this method returns a `200 OK` response code and collection of [group](../resources/team.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96a11-133">Пример</span><span class="sxs-lookup"><span data-stu-id="96a11-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96a11-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="96a11-134">Request</span></span>
<span data-ttu-id="96a11-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="96a11-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="96a11-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="96a11-136">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="96a11-137">C#</span><span class="sxs-lookup"><span data-stu-id="96a11-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="96a11-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96a11-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="96a11-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96a11-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="96a11-140">Java</span><span class="sxs-lookup"><span data-stu-id="96a11-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-joinedteams-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96a11-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="96a11-141">Response</span></span>
<span data-ttu-id="96a11-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="96a11-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="96a11-145">См. также</span><span class="sxs-lookup"><span data-stu-id="96a11-145">See also</span></span>
[<span data-ttu-id="96a11-146">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="96a11-146">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
