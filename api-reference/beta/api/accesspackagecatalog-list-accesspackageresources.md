---
title: Список accessPackageResources
description: Получить список объектов accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3dc8d28d66f96508270101aa465079ee0ca19d70
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934550"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="598bf-103">Список accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="598bf-103">List accessPackageResources</span></span>

<span data-ttu-id="598bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="598bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="598bf-105">Получить список объектов [accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog.](../resources/accesspackagecatalog.md)</span><span class="sxs-lookup"><span data-stu-id="598bf-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="598bf-106">Чтобы запросить добавление или удаление [accessPackageResource,](../resources/accesspackageresource.md)используйте [создание accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="598bf-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="598bf-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="598bf-107">Permissions</span></span>

<span data-ttu-id="598bf-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="598bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="598bf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="598bf-110">Permission type</span></span>                        | <span data-ttu-id="598bf-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="598bf-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="598bf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="598bf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="598bf-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598bf-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="598bf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="598bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="598bf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="598bf-115">Not supported.</span></span> |
| <span data-ttu-id="598bf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="598bf-116">Application</span></span>                            | <span data-ttu-id="598bf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="598bf-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="598bf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="598bf-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="598bf-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="598bf-119">Optional query parameters</span></span>

<span data-ttu-id="598bf-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="598bf-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="598bf-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="598bf-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="598bf-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="598bf-122">Request headers</span></span>

| <span data-ttu-id="598bf-123">Имя</span><span class="sxs-lookup"><span data-stu-id="598bf-123">Name</span></span>      |<span data-ttu-id="598bf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="598bf-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="598bf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="598bf-125">Authorization</span></span> | <span data-ttu-id="598bf-126">Носитель \{токен\}.</span><span class="sxs-lookup"><span data-stu-id="598bf-126">Bearer \{token\}.</span></span> <span data-ttu-id="598bf-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="598bf-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="598bf-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="598bf-128">Request body</span></span>

<span data-ttu-id="598bf-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="598bf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="598bf-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="598bf-130">Response</span></span>

<span data-ttu-id="598bf-131">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResource](../resources/accesspackageresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="598bf-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="598bf-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="598bf-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="598bf-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="598bf-133">Request</span></span>

<span data-ttu-id="598bf-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="598bf-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="598bf-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="598bf-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="598bf-136">C#</span><span class="sxs-lookup"><span data-stu-id="598bf-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="598bf-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="598bf-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="598bf-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="598bf-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="598bf-139">Java</span><span class="sxs-lookup"><span data-stu-id="598bf-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="598bf-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="598bf-140">Response</span></span>

<span data-ttu-id="598bf-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="598bf-141">The following is an example of the response.</span></span>

> <span data-ttu-id="598bf-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="598bf-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


