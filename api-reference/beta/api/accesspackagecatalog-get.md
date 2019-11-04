---
title: Получение Акцесспаккажекаталог
description: Получение свойств и связей объекта акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3c12ba6922e3252c91cd456e17ad162be7a3e40
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936089"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="76ca6-103">Получение Акцесспаккажекаталог</span><span class="sxs-lookup"><span data-stu-id="76ca6-103">Get accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76ca6-104">Получение свойств и связей объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="76ca6-104">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="76ca6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76ca6-105">Permissions</span></span>

<span data-ttu-id="76ca6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76ca6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76ca6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76ca6-108">Permission type</span></span>                        | <span data-ttu-id="76ca6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76ca6-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76ca6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76ca6-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="76ca6-111">Ентитлементманажемент. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="76ca6-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="76ca6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76ca6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76ca6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ca6-113">Not supported.</span></span> |
| <span data-ttu-id="76ca6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76ca6-114">Application</span></span>                            | <span data-ttu-id="76ca6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76ca6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="76ca6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76ca6-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76ca6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="76ca6-117">Optional query parameters</span></span>

<span data-ttu-id="76ca6-118">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="76ca6-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="76ca6-119">Например, чтобы получить пакеты Access в каталоге, включите `$expand=accessPackages` в запрос.</span><span class="sxs-lookup"><span data-stu-id="76ca6-119">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="76ca6-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="76ca6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="76ca6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76ca6-121">Request headers</span></span>

| <span data-ttu-id="76ca6-122">Имя</span><span class="sxs-lookup"><span data-stu-id="76ca6-122">Name</span></span>      |<span data-ttu-id="76ca6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="76ca6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76ca6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="76ca6-124">Authorization</span></span> | <span data-ttu-id="76ca6-125">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="76ca6-125">Bearer \{token\}.</span></span> <span data-ttu-id="76ca6-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="76ca6-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76ca6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76ca6-127">Request body</span></span>

<span data-ttu-id="76ca6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76ca6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76ca6-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="76ca6-129">Response</span></span>

<span data-ttu-id="76ca6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76ca6-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76ca6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="76ca6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76ca6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="76ca6-132">Request</span></span>

<span data-ttu-id="76ca6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76ca6-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

### <a name="response"></a><span data-ttu-id="76ca6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="76ca6-134">Response</span></span>

<span data-ttu-id="76ca6-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="76ca6-135">The following is an example of the response.</span></span>

> <span data-ttu-id="76ca6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76ca6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
