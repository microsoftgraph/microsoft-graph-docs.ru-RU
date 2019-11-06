---
title: Список Акцесспаккажекаталогс
description: Получение списка объектов Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d1d8aaf8a0138195e737cdd26f288f7aca8ba3e5
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994256"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="98ab6-103">Список Акцесспаккажекаталогс</span><span class="sxs-lookup"><span data-stu-id="98ab6-103">List accessPackageCatalogs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98ab6-104">Получение списка объектов [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="98ab6-104">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="98ab6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98ab6-105">Permissions</span></span>

<span data-ttu-id="98ab6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98ab6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="98ab6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98ab6-108">Permission type</span></span>                        | <span data-ttu-id="98ab6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98ab6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="98ab6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98ab6-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="98ab6-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98ab6-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="98ab6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98ab6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98ab6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98ab6-113">Not supported.</span></span> |
| <span data-ttu-id="98ab6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98ab6-114">Application</span></span>                            | <span data-ttu-id="98ab6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98ab6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="98ab6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98ab6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="98ab6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98ab6-117">Optional query parameters</span></span>

<span data-ttu-id="98ab6-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="98ab6-118">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="98ab6-119">Например, чтобы получить пакеты доступа в каждом каталоге, включите `$expand=accessPackages` в запрос.</span><span class="sxs-lookup"><span data-stu-id="98ab6-119">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="98ab6-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="98ab6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="98ab6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98ab6-121">Request headers</span></span>

| <span data-ttu-id="98ab6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="98ab6-122">Name</span></span>      |<span data-ttu-id="98ab6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="98ab6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="98ab6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="98ab6-124">Authorization</span></span> | <span data-ttu-id="98ab6-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="98ab6-125">Bearer \{token\}.</span></span> <span data-ttu-id="98ab6-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="98ab6-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="98ab6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98ab6-127">Request body</span></span>

<span data-ttu-id="98ab6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98ab6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98ab6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="98ab6-129">Response</span></span>

<span data-ttu-id="98ab6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="98ab6-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="98ab6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="98ab6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="98ab6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="98ab6-132">Request</span></span>

<span data-ttu-id="98ab6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98ab6-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="98ab6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="98ab6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="98ab6-135">C#</span><span class="sxs-lookup"><span data-stu-id="98ab6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98ab6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98ab6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="98ab6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98ab6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="98ab6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="98ab6-138">Response</span></span>

<span data-ttu-id="98ab6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98ab6-139">The following is an example of the response.</span></span>

> <span data-ttu-id="98ab6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98ab6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
