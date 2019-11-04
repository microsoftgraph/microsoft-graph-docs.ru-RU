---
title: Список Акцесспаккажекаталогс
description: Получение списка объектов Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a747f6620ca24c998be422bc8a2f2417988119b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936085"
---
# <a name="list-accesspackagecatalogs"></a><span data-ttu-id="82d16-103">Список Акцесспаккажекаталогс</span><span class="sxs-lookup"><span data-stu-id="82d16-103">List accessPackageCatalogs</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d16-104">Получение списка объектов [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="82d16-104">Retrieve a list of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="82d16-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82d16-105">Permissions</span></span>

<span data-ttu-id="82d16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82d16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82d16-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82d16-108">Permission type</span></span>                        | <span data-ttu-id="82d16-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82d16-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82d16-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82d16-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="82d16-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="82d16-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="82d16-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82d16-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d16-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d16-113">Not supported.</span></span> |
| <span data-ttu-id="82d16-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82d16-114">Application</span></span>                            | <span data-ttu-id="82d16-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82d16-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="82d16-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82d16-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82d16-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82d16-117">Optional query parameters</span></span>

<span data-ttu-id="82d16-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="82d16-118">This method supports some of the OData query parameters to help customize the response.</span></span>  <span data-ttu-id="82d16-119">Например, чтобы получить пакеты доступа в каждом каталоге, включите `$expand=accessPackages` в запрос.</span><span class="sxs-lookup"><span data-stu-id="82d16-119">For example, to retrieve the access packages in each catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="82d16-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="82d16-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82d16-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82d16-121">Request headers</span></span>

| <span data-ttu-id="82d16-122">Имя</span><span class="sxs-lookup"><span data-stu-id="82d16-122">Name</span></span>      |<span data-ttu-id="82d16-123">Описание</span><span class="sxs-lookup"><span data-stu-id="82d16-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82d16-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d16-124">Authorization</span></span> | <span data-ttu-id="82d16-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="82d16-125">Bearer \{token\}.</span></span> <span data-ttu-id="82d16-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="82d16-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82d16-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82d16-127">Request body</span></span>

<span data-ttu-id="82d16-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82d16-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82d16-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="82d16-129">Response</span></span>

<span data-ttu-id="82d16-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82d16-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82d16-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="82d16-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82d16-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="82d16-132">Request</span></span>

<span data-ttu-id="82d16-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82d16-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalogs"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
```

### <a name="response"></a><span data-ttu-id="82d16-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="82d16-134">Response</span></span>

<span data-ttu-id="82d16-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="82d16-135">The following is an example of the response.</span></span>

> <span data-ttu-id="82d16-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82d16-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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