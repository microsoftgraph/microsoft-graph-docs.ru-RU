---
title: Получение Акцесспаккажекаталог
description: Получение свойств и связей объекта акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b13becb36bbcc9fb4eb579f1997c66ae7262fe2b
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345480"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="823f2-103">Получение Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="823f2-103">Get accessPackageCatalog</span></span>

<span data-ttu-id="823f2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="823f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="823f2-105">Получение свойств и связей объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="823f2-105">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="823f2-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="823f2-106">Permissions</span></span>

<span data-ttu-id="823f2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="823f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="823f2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="823f2-109">Permission type</span></span>                        | <span data-ttu-id="823f2-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="823f2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="823f2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="823f2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="823f2-112">Ентитлементманажемент. Read. ALL, Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="823f2-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="823f2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="823f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="823f2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="823f2-114">Not supported.</span></span> |
| <span data-ttu-id="823f2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="823f2-115">Application</span></span>                            | <span data-ttu-id="823f2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="823f2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="823f2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="823f2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="823f2-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="823f2-118">Optional query parameters</span></span>

<span data-ttu-id="823f2-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="823f2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="823f2-120">Например, чтобы получить пакеты Access в каталоге, включите `$expand=accessPackages` в запрос.</span><span class="sxs-lookup"><span data-stu-id="823f2-120">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="823f2-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="823f2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="823f2-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="823f2-122">Request headers</span></span>

| <span data-ttu-id="823f2-123">Имя</span><span class="sxs-lookup"><span data-stu-id="823f2-123">Name</span></span>      |<span data-ttu-id="823f2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="823f2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="823f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="823f2-125">Authorization</span></span> | <span data-ttu-id="823f2-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="823f2-126">Bearer \{token\}.</span></span> <span data-ttu-id="823f2-127">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="823f2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="823f2-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="823f2-128">Request body</span></span>

<span data-ttu-id="823f2-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="823f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="823f2-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="823f2-130">Response</span></span>

<span data-ttu-id="823f2-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="823f2-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="823f2-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="823f2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="823f2-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="823f2-133">Request</span></span>

<span data-ttu-id="823f2-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="823f2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="823f2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="823f2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```
# <a name="c"></a>[<span data-ttu-id="823f2-136">C#</span><span class="sxs-lookup"><span data-stu-id="823f2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="823f2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="823f2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="823f2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="823f2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="823f2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="823f2-139">Response</span></span>

<span data-ttu-id="823f2-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="823f2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="823f2-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="823f2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
