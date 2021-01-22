---
title: Список accessPackageAssignments
description: Получить список объектов accesspackageassignment.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 605bc5bdfcafbf4c7aaae9903530bc5d067c748f
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934543"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="7244b-103">Список accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="7244b-103">List accessPackageAssignments</span></span>

<span data-ttu-id="7244b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7244b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7244b-105">В [средстве управления правами Azure AD](../resources/entitlementmanagement-root.md)извлекает список объектов [accessPackageAssignment.](../resources/accesspackageassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7244b-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span> <span data-ttu-id="7244b-106">Для администраторов всего каталога в итоговом списке содержатся все назначения, текущие и просроченные, которые вызывающий имеет доступ для чтения во всех каталогах и пакетах доступа.</span><span class="sxs-lookup"><span data-stu-id="7244b-106">For directory-wide administrators, the resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="7244b-107">Если вызываемая система находится от имени делегированного пользователя, которому назначены только делегированные административные роли каталога, запрос должен предоставить фильтр, чтобы указать определенный пакет доступа, `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` например:</span><span class="sxs-lookup"><span data-stu-id="7244b-107">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>


## <a name="permissions"></a><span data-ttu-id="7244b-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7244b-108">Permissions</span></span>

<span data-ttu-id="7244b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7244b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7244b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7244b-111">Permission type</span></span>                        | <span data-ttu-id="7244b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7244b-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7244b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7244b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7244b-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7244b-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7244b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7244b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7244b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7244b-116">Not supported.</span></span> |
| <span data-ttu-id="7244b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7244b-117">Application</span></span>                            | <span data-ttu-id="7244b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7244b-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7244b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7244b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7244b-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7244b-120">Optional query parameters</span></span>

<span data-ttu-id="7244b-121">Если вызываемая система находится от имени делегированного пользователя, которому назначены только делегированные административные роли каталога, запрос должен предоставить фильтр, чтобы указать определенный пакет доступа, `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` например:</span><span class="sxs-lookup"><span data-stu-id="7244b-121">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>  <span data-ttu-id="7244b-122">Этот метод также поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7244b-122">This method also supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7244b-123">Например, чтобы также вернуть целевую тему и пакет доступа, включаем `$expand=target,accessPackage` .</span><span class="sxs-lookup"><span data-stu-id="7244b-123">For example, to also return the target subject and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="7244b-124">Чтобы получить только доставленные назначения, можно включить `$filter=assignmentState eq 'Delivered'` запрос.</span><span class="sxs-lookup"><span data-stu-id="7244b-124">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="7244b-125">Чтобы получить только назначения для определенного пользователя, можно включить запрос с назначениями, нацеленными на ИД объекта этого пользователя: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="7244b-125">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="7244b-126">Чтобы получить только назначения для определенного пользователя и определенный пакет доступа, можно включить запрос с назначениями, нацеленными на этот пакет доступа, и ид объекта этого пользователя: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` .</span><span class="sxs-lookup"><span data-stu-id="7244b-126">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="7244b-127">Чтобы получить только назначения, полученные из определенной политики назначения пакета доступа, можно включить запрос для этой политики: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'` .</span><span class="sxs-lookup"><span data-stu-id="7244b-127">To retrieve only assignments resulting from a particular access package assignment policy, you can include a query for that policy: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'`.</span></span>

<span data-ttu-id="7244b-128">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7244b-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7244b-129">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7244b-129">Request headers</span></span>

| <span data-ttu-id="7244b-130">Имя</span><span class="sxs-lookup"><span data-stu-id="7244b-130">Name</span></span>      |<span data-ttu-id="7244b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7244b-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7244b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7244b-132">Authorization</span></span> | <span data-ttu-id="7244b-133">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="7244b-133">Bearer \{token\}.</span></span> <span data-ttu-id="7244b-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7244b-134">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7244b-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7244b-135">Request body</span></span>

<span data-ttu-id="7244b-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7244b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7244b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="7244b-137">Response</span></span>

<span data-ttu-id="7244b-138">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7244b-138">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7244b-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="7244b-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7244b-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="7244b-140">Request</span></span>

<span data-ttu-id="7244b-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7244b-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7244b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7244b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="7244b-143">C#</span><span class="sxs-lookup"><span data-stu-id="7244b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7244b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7244b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7244b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7244b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7244b-146">Java</span><span class="sxs-lookup"><span data-stu-id="7244b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7244b-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7244b-147">Response</span></span>

<span data-ttu-id="7244b-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7244b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="7244b-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7244b-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


