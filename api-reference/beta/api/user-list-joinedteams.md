---
title: Перечисление объектов joinedTeams
description: Загрузите группами Майкрософт, который пользователь является непосредственным членом группы.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 839b6531318ca9fc8abb3fd3544566622d02a78b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938204"
---
# <a name="list-joinedteams"></a><span data-ttu-id="e8be7-103">Перечисление объектов joinedTeams</span><span class="sxs-lookup"><span data-stu-id="e8be7-103">List joinedTeams</span></span>

> <span data-ttu-id="e8be7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8be7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8be7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8be7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8be7-106">Загрузите группами Майкрософт, который пользователь является непосредственным членом [групп](../resources/team.md) .</span><span class="sxs-lookup"><span data-stu-id="e8be7-106">Get the [teams](../resources/team.md) in Microsoft Teams that the user is a direct member of.</span></span>
 
## <a name="permissions"></a><span data-ttu-id="e8be7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8be7-107">Permissions</span></span>
<span data-ttu-id="e8be7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8be7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8be7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8be7-110">Permission type</span></span>      | <span data-ttu-id="e8be7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8be7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8be7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8be7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e8be7-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8be7-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="e8be7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8be7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8be7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8be7-115">Not supported.</span></span>    |
|<span data-ttu-id="e8be7-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8be7-116">Application</span></span> | <span data-ttu-id="e8be7-117">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8be7-117">User.Read.All, User.ReadWrite.All</span></span> |

> <span data-ttu-id="e8be7-118">На данный момент с разрешениями пользователя делегированной эта операция работает только для «me» пользователя.</span><span class="sxs-lookup"><span data-stu-id="e8be7-118">Currently, with user delegated permissions this operation only works for the 'me' user.</span></span> 
> <span data-ttu-id="e8be7-119">Имея разрешения приложения это работает для всех пользователей, указав идентификатор определенного пользователя. («обо мне» псевдоним не поддерживается с разрешениями приложения) Дополнительные сведения см [Известные проблемы](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span><span class="sxs-lookup"><span data-stu-id="e8be7-119">With application permissions, it works for all users by specifying  the specific user  id. ('me' alias is not supported with application permissions) For details, see [Known issues](/graph/known-issues#microsoft-teams-users-list-of-joined-teams-preview).</span></span>

## <a name="http-request"></a><span data-ttu-id="e8be7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8be7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/joinedTeams
or
GET /users/{id}/joinedTeams
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8be7-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e8be7-121">Optional query parameters</span></span>
<span data-ttu-id="e8be7-122">[Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) в настоящее время не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="e8be7-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8be7-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8be7-123">Request headers</span></span>
| <span data-ttu-id="e8be7-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e8be7-124">Header</span></span>       | <span data-ttu-id="e8be7-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e8be7-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8be7-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8be7-126">Authorization</span></span>  | <span data-ttu-id="e8be7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8be7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8be7-129">Accept</span><span class="sxs-lookup"><span data-stu-id="e8be7-129">Accept</span></span>  | <span data-ttu-id="e8be7-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e8be7-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8be7-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e8be7-131">Request body</span></span>
<span data-ttu-id="e8be7-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e8be7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8be7-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8be7-133">Response</span></span>

<span data-ttu-id="e8be7-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [group](../resources/group.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8be7-134">If successful, this method returns a `200 OK` response code and collection of [group](../resources/group.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8be7-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e8be7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8be7-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8be7-136">Request</span></span>
<span data-ttu-id="e8be7-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8be7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_joinedteams"
}-->
```http
GET https://graph.microsoft.com/beta/me/joinedTeams
```
##### <a name="response"></a><span data-ttu-id="e8be7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8be7-138">Response</span></span>
<span data-ttu-id="e8be7-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e8be7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="e8be7-142">См. также</span><span class="sxs-lookup"><span data-stu-id="e8be7-142">See also</span></span>
[<span data-ttu-id="e8be7-143">Список всех групп</span><span class="sxs-lookup"><span data-stu-id="e8be7-143">List all teams</span></span>](/graph/teams-list-all-teams)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List joinedTeams",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
