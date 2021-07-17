---
title: Список accessPackageResources
description: Извлечение списка объектов accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3aaeddef635a80bb8a54d3680281b8b9edae98ae
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466952"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="b25f9-103">Список accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="b25f9-103">List accessPackageResources</span></span>

<span data-ttu-id="b25f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b25f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b25f9-105">Извлечение списка [объектов accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="b25f9-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="b25f9-106">Чтобы попросить добавить или удалить [accessPackageResource,](../resources/accesspackageresource.md)используйте [создание accessPackageResourceRequest.](accesspackageresourcerequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="b25f9-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b25f9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b25f9-107">Permissions</span></span>

<span data-ttu-id="b25f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b25f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b25f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b25f9-110">Permission type</span></span>                        | <span data-ttu-id="b25f9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b25f9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b25f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b25f9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b25f9-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25f9-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b25f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b25f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b25f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b25f9-115">Not supported.</span></span> |
| <span data-ttu-id="b25f9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b25f9-116">Application</span></span>                            | <span data-ttu-id="b25f9-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b25f9-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b25f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b25f9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b25f9-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b25f9-119">Optional query parameters</span></span>

<span data-ttu-id="b25f9-120">Этот метод поддерживает параметры запросов OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b25f9-120">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="b25f9-121">Например, чтобы получить области и среды пакета доступа для каждого ресурса, включайте `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` в запрос.</span><span class="sxs-lookup"><span data-stu-id="b25f9-121">For example, to retrieve the access package resource scopes and environments for each resource, include `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment` in the query.</span></span> <span data-ttu-id="b25f9-122">Чтобы получить доступные роли ресурса, включай `$expand=accessPackageResourceRoles` .</span><span class="sxs-lookup"><span data-stu-id="b25f9-122">To retrieve the available roles of a resource, include `$expand=accessPackageResourceRoles`.</span></span> <span data-ttu-id="b25f9-123">Чтобы получить только ресурсы для приложений, а не групп или сайтов, включайте `$filter=resourceType eq 'Application'` запрос.</span><span class="sxs-lookup"><span data-stu-id="b25f9-123">To retrieve only resources for applications and not groups or sites, include `$filter=resourceType eq 'Application'` in the query.</span></span> <span data-ttu-id="b25f9-124">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b25f9-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b25f9-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b25f9-125">Request headers</span></span>

| <span data-ttu-id="b25f9-126">Имя</span><span class="sxs-lookup"><span data-stu-id="b25f9-126">Name</span></span>      |<span data-ttu-id="b25f9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b25f9-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b25f9-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="b25f9-128">Authorization</span></span> | <span data-ttu-id="b25f9-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b25f9-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b25f9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b25f9-131">Request body</span></span>

<span data-ttu-id="b25f9-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b25f9-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b25f9-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25f9-133">Response</span></span>

<span data-ttu-id="b25f9-134">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResource](../resources/accesspackageresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b25f9-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b25f9-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="b25f9-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b25f9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b25f9-136">Request</span></span>

<span data-ttu-id="b25f9-137">Ниже приводится пример запроса с помощью фильтра для выбора ресурсов определенного типа и возврата областей ресурсов `$expand` каждого ресурса.</span><span class="sxs-lookup"><span data-stu-id="b25f9-137">The following is an example of the request, using a filter to select resources of a particular type and `$expand` to return resource scopes of each resource.</span></span>

# <a name="http"></a>[<span data-ttu-id="b25f9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="b25f9-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources?$filter=resourceType eq 'Application'&$expand=accessPackageResourceScopes
```
# <a name="c"></a>[<span data-ttu-id="b25f9-139">C#</span><span class="sxs-lookup"><span data-stu-id="b25f9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b25f9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b25f9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b25f9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b25f9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b25f9-142">Java</span><span class="sxs-lookup"><span data-stu-id="b25f9-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b25f9-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25f9-143">Response</span></span>

<span data-ttu-id="b25f9-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b25f9-144">The following is an example of the response.</span></span>

> <span data-ttu-id="b25f9-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b25f9-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
      "accessPackageResourceScopes": [
         {
            "id": "452d78a7-69a5-482d-a82f-859a5169c55e",
            "displayName": "Root",
            "description": "Root Scope",
            "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e",
            "originSystem": "AadApplication",
            "isRootScope": true
         }
      ]
    }
  ]
}
```

https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/e71fafe7-9ccb-4c5a-a7b3-77ec35e83e3c/accessPackageResources

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


