---
title: Список accessPackageCatalogs
description: Извлечение списка объектов accessPackageCatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c4f4d959792e657f79d0242a52944da505a41695
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439550"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="28b93-103">Список accessPackageCatalogs</span><span class="sxs-lookup"><span data-stu-id="28b93-103">List accessPackageCatalogs</span></span>

<span data-ttu-id="28b93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28b93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28b93-105">Извлечение списка [объектов accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="28b93-105">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="28b93-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28b93-106">Permissions</span></span>

<span data-ttu-id="28b93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28b93-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28b93-109">Permission type</span></span>                        | <span data-ttu-id="28b93-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28b93-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="28b93-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28b93-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28b93-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b93-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="28b93-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28b93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28b93-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28b93-114">Not supported.</span></span> |
| <span data-ttu-id="28b93-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="28b93-115">Application</span></span>                            | <span data-ttu-id="28b93-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28b93-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="28b93-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28b93-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="28b93-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="28b93-118">Optional query parameters</span></span>

<span data-ttu-id="28b93-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="28b93-119">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="28b93-120">Например, чтобы получить пакеты доступа в каждом каталоге, включайте `$expand=accessPackages` в запрос.</span><span class="sxs-lookup"><span data-stu-id="28b93-120">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="28b93-121">Чтобы найти каталоги пакетов доступа с определенным именем, включайте фильтр, `$filter=contains(tolower(displayName),'staff')` например, в запрос.</span><span class="sxs-lookup"><span data-stu-id="28b93-121">To search for access package catalogs with a particular name, include a filter such as `$filter=contains(tolower(displayName),'staff')` in the query.</span></span>  <span data-ttu-id="28b93-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="28b93-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="28b93-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28b93-123">Request headers</span></span>

| <span data-ttu-id="28b93-124">Имя</span><span class="sxs-lookup"><span data-stu-id="28b93-124">Name</span></span>      |<span data-ttu-id="28b93-125">Описание</span><span class="sxs-lookup"><span data-stu-id="28b93-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28b93-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="28b93-126">Authorization</span></span> | <span data-ttu-id="28b93-127">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="28b93-127">Bearer \{token\}.</span></span> <span data-ttu-id="28b93-128">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="28b93-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28b93-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28b93-129">Request body</span></span>

<span data-ttu-id="28b93-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28b93-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28b93-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="28b93-131">Response</span></span>

<span data-ttu-id="28b93-132">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageCatalog](../resources/accesspackagecatalog.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="28b93-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="28b93-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="28b93-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="28b93-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="28b93-134">Request</span></span>

<span data-ttu-id="28b93-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28b93-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28b93-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="28b93-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="c"></a>[<span data-ttu-id="28b93-137">C#</span><span class="sxs-lookup"><span data-stu-id="28b93-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28b93-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28b93-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28b93-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28b93-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28b93-140">Java</span><span class="sxs-lookup"><span data-stu-id="28b93-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagecatalogs-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28b93-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="28b93-141">Response</span></span>

<span data-ttu-id="28b93-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28b93-142">The following is an example of the response.</span></span>

> <span data-ttu-id="28b93-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="28b93-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package catalog",
      "displayName":"Access package catalog for testing",
      "isExternallyVisible":false,
      "catalogType":"UserManaged",
      "catalogStatus":"Published",
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageCatalogs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


