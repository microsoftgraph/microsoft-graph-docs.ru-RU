---
title: Перечисление объектов joinedTeams
description: Получение команд в Microsoft Teams, непосредственным участником которых является пользователь.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 648b0a6edd8f5e24665a6829e0f30ff10453d23b
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459503"
---
# <a name="list-joinedteams"></a><span data-ttu-id="8d09b-103">Перечисление объектов joinedTeams</span><span class="sxs-lookup"><span data-stu-id="8d09b-103">List joinedTeams</span></span>

<span data-ttu-id="8d09b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d09b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d09b-105">Получение [команд](../resources/team.md) в Microsoft Teams, непосредственным участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="8d09b-105">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="8d09b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d09b-106">Permissions</span></span>
<span data-ttu-id="8d09b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d09b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d09b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d09b-109">Permission type</span></span>      | <span data-ttu-id="8d09b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d09b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d09b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d09b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8d09b-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d09b-112">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="8d09b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d09b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d09b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d09b-114">Not supported.</span></span>    |
|<span data-ttu-id="8d09b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d09b-115">Application</span></span> | <span data-ttu-id="8d09b-116">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d09b-116">Team.ReadBasic.All, TeamSettings.Read.All, TeamSettings.ReadWrite.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="8d09b-117">В настоящее время при использовании делегированных разрешений эта операция поддерживается только для пользователя "Я".</span><span class="sxs-lookup"><span data-stu-id="8d09b-117">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="8d09b-118">При использовании разрешений для приложений она поддерживается для всех пользователей путем указания определенного идентификатора пользователя. (Псевдоним "Я" не поддерживается при использовании разрешений для приложений). Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span><span class="sxs-lookup"><span data-stu-id="8d09b-118">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="8d09b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d09b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8d09b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8d09b-120">Optional query parameters</span></span>
<span data-ttu-id="8d09b-121">[Параметры запроса OData](/graph/query-parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8d09b-121">The [OData Query Parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d09b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d09b-122">Request headers</span></span>
| <span data-ttu-id="8d09b-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d09b-123">Header</span></span>       | <span data-ttu-id="8d09b-124">Значение</span><span class="sxs-lookup"><span data-stu-id="8d09b-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d09b-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d09b-125">Authorization</span></span>  | <span data-ttu-id="8d09b-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d09b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8d09b-128">Accept</span><span class="sxs-lookup"><span data-stu-id="8d09b-128">Accept</span></span>  | <span data-ttu-id="8d09b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="8d09b-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d09b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d09b-130">Request body</span></span>
<span data-ttu-id="8d09b-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d09b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d09b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d09b-132">Response</span></span>

<span data-ttu-id="8d09b-133">При успешном выполнении этот метод возвращает `200 OK`код ответа и коллекцию объектов [team](../resources/team.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8d09b-133">If successful, this method returns a `200 OK` response code and collection of [team](../resources/team.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d09b-134">Пример</span><span class="sxs-lookup"><span data-stu-id="8d09b-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d09b-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d09b-135">Request</span></span>
<span data-ttu-id="8d09b-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d09b-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d09b-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d09b-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/joinedTeams
```
# <a name="c"></a>[<span data-ttu-id="8d09b-138">C#</span><span class="sxs-lookup"><span data-stu-id="8d09b-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-joinedteams-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8d09b-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d09b-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-joinedteams-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8d09b-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d09b-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-joinedteams-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8d09b-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d09b-141">Response</span></span>
<span data-ttu-id="8d09b-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="8d09b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="8d09b-145">См. также</span><span class="sxs-lookup"><span data-stu-id="8d09b-145">See also</span></span>
[<span data-ttu-id="8d09b-146">Перечисление всех команд</span><span class="sxs-lookup"><span data-stu-id="8d09b-146">List all teams</span></span>](/graph/teams-list-all-teams)

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
