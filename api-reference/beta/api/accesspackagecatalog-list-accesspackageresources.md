---
title: Список accessPackageResources
description: Извлечение списка объектов accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a148144c416d91ed43d1eedcbc800b779dc2800a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439557"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="4a32f-103">Список accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="4a32f-103">List accessPackageResources</span></span>

<span data-ttu-id="4a32f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a32f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a32f-105">Извлечение списка [объектов accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="4a32f-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="4a32f-106">Чтобы попросить добавить или удалить [accessPackageResource,](../resources/accesspackageresource.md)используйте [создание accessPackageResourceRequest.](accesspackageresourcerequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="4a32f-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a32f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a32f-107">Permissions</span></span>

<span data-ttu-id="4a32f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a32f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a32f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a32f-110">Permission type</span></span>                        | <span data-ttu-id="4a32f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a32f-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4a32f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a32f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a32f-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a32f-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4a32f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a32f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a32f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a32f-115">Not supported.</span></span> |
| <span data-ttu-id="4a32f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4a32f-116">Application</span></span>                            | <span data-ttu-id="4a32f-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a32f-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a32f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a32f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a32f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4a32f-119">Optional query parameters</span></span>

<span data-ttu-id="4a32f-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4a32f-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4a32f-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4a32f-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a32f-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a32f-122">Request headers</span></span>

| <span data-ttu-id="4a32f-123">Имя</span><span class="sxs-lookup"><span data-stu-id="4a32f-123">Name</span></span>      |<span data-ttu-id="4a32f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="4a32f-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a32f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a32f-125">Authorization</span></span> | <span data-ttu-id="4a32f-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="4a32f-126">Bearer \{token\}.</span></span> <span data-ttu-id="4a32f-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="4a32f-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a32f-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a32f-128">Request body</span></span>

<span data-ttu-id="4a32f-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a32f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a32f-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a32f-130">Response</span></span>

<span data-ttu-id="4a32f-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResource](../resources/accesspackageresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a32f-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4a32f-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="4a32f-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4a32f-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a32f-133">Request</span></span>

<span data-ttu-id="4a32f-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a32f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a32f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a32f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="4a32f-136">C#</span><span class="sxs-lookup"><span data-stu-id="4a32f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a32f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a32f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a32f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a32f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a32f-139">Java</span><span class="sxs-lookup"><span data-stu-id="4a32f-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a32f-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a32f-140">Response</span></span>

<span data-ttu-id="4a32f-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a32f-141">The following is an example of the response.</span></span>

> <span data-ttu-id="4a32f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a32f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


