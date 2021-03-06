---
title: Список объектов appRoleAssignment, предоставленных для пользователя
description: Получение списка назначений ролей приложений, предоставленных для пользователя.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 43f1119f83d0865319462e7ffb65c263eb67f06f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433528"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="15194-103">Список объектов appRoleAssignment, предоставленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="15194-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="15194-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15194-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15194-105">Получение списка [appRoleAssignment](../resources/approleassignment.md), предоставленного пользователю.</span><span class="sxs-lookup"><span data-stu-id="15194-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="15194-106">Эта операция также возвращает роли приложений, назначенные группам, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="15194-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="15194-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="15194-107">Permissions</span></span>

<span data-ttu-id="15194-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15194-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15194-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15194-110">Permission type</span></span>      | <span data-ttu-id="15194-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15194-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15194-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15194-112">Delegated (work or school account)</span></span> | <span data-ttu-id="15194-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="15194-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="15194-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15194-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15194-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15194-115">Not supported.</span></span>    |
|<span data-ttu-id="15194-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="15194-116">Application</span></span> | <span data-ttu-id="15194-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15194-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15194-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15194-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="15194-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="15194-119">Optional query parameters</span></span>

<span data-ttu-id="15194-120">Этот метод поддерживает [параметры запросов OData](/graph/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="15194-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="15194-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="15194-121">Request headers</span></span>

| <span data-ttu-id="15194-122">Имя</span><span class="sxs-lookup"><span data-stu-id="15194-122">Name</span></span>           | <span data-ttu-id="15194-123">Описание</span><span class="sxs-lookup"><span data-stu-id="15194-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="15194-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15194-124">Authorization</span></span>  | <span data-ttu-id="15194-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15194-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="15194-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="15194-127">Request body</span></span>

<span data-ttu-id="15194-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="15194-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15194-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="15194-129">Response</span></span>

<span data-ttu-id="15194-130">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [appRoleAssignment](../resources/approleassignment.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="15194-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15194-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="15194-131">Examples</span></span>

### <a name="example-1-list-approleassignments-granted-to-a-user"></a><span data-ttu-id="15194-132">Пример 1. Список объектов appRoleAssignment, предоставленных для пользователя</span><span class="sxs-lookup"><span data-stu-id="15194-132">Example 1: List appRoleAssignments granted to a user</span></span>

#### <a name="request"></a><span data-ttu-id="15194-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="15194-133">Request</span></span>

<span data-ttu-id="15194-134">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="15194-134">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="15194-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="15194-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="15194-136">C#</span><span class="sxs-lookup"><span data-stu-id="15194-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15194-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15194-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15194-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15194-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15194-139">Java</span><span class="sxs-lookup"><span data-stu-id="15194-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="15194-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="15194-140">Response</span></span>

<span data-ttu-id="15194-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15194-141">The following is an example of the response.</span></span> 

><span data-ttu-id="15194-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15194-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "Alex Wilber",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

### <a name="example-2-list-approleassignments-granted-to-a-user-filtered-by-resourceid"></a><span data-ttu-id="15194-144">Пример 2. Список объектов appRoleAssignment, предоставленных для пользователя и отфильтрованных по resourceId</span><span class="sxs-lookup"><span data-stu-id="15194-144">Example 2: List appRoleAssignments granted to a user, filtered by resourceId</span></span>

#### <a name="request"></a><span data-ttu-id="15194-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="15194-145">Request</span></span>

<span data-ttu-id="15194-146">В приведенном примере показано, как запросить извлечение ролей приложения, назначенных пользователю, отфильтровав их по `resourceId`, который является типом GUID</span><span class="sxs-lookup"><span data-stu-id="15194-146">Here is an example of the request to retrieve the app roles that have been assigned to a user, filtering by a `resourceId`, which is a GUID type.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments_filterby_resourceId"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments?$filter=resourceId eq 8e881353-1735-45af-af21-ee1344582a4d
```

#### <a name="response"></a><span data-ttu-id="15194-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="15194-147">Response</span></span>

<span data-ttu-id="15194-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="15194-148">The following is an example of the response.</span></span> 

><span data-ttu-id="15194-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="15194-149">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


