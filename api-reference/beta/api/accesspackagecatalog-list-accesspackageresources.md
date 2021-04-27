---
title: Список accessPackageResources
description: Извлечение списка объектов accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be2ad10b946574ca48b93ada1d7833262f127059
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048563"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="7d205-103">Список accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="7d205-103">List accessPackageResources</span></span>

<span data-ttu-id="7d205-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d205-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d205-105">Извлечение списка [объектов accessPackageResource](../resources/accesspackageresource.md) в [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="7d205-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="7d205-106">Чтобы попросить добавить или удалить [accessPackageResource,](../resources/accesspackageresource.md)используйте [создание accessPackageResourceRequest.](accesspackageresourcerequest-post.md)</span><span class="sxs-lookup"><span data-stu-id="7d205-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7d205-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7d205-107">Permissions</span></span>

<span data-ttu-id="7d205-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d205-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d205-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d205-110">Permission type</span></span>                        | <span data-ttu-id="7d205-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d205-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7d205-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d205-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d205-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d205-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7d205-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d205-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d205-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d205-115">Not supported.</span></span> |
| <span data-ttu-id="7d205-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7d205-116">Application</span></span>                            | <span data-ttu-id="7d205-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d205-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d205-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d205-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7d205-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7d205-119">Optional query parameters</span></span>

<span data-ttu-id="7d205-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="7d205-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7d205-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="7d205-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7d205-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d205-122">Request headers</span></span>

| <span data-ttu-id="7d205-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7d205-123">Name</span></span>      |<span data-ttu-id="7d205-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7d205-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d205-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7d205-125">Authorization</span></span> | <span data-ttu-id="7d205-p104">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7d205-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d205-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d205-128">Request body</span></span>

<span data-ttu-id="7d205-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7d205-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d205-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d205-130">Response</span></span>

<span data-ttu-id="7d205-131">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [accessPackageResource](../resources/accesspackageresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="7d205-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d205-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7d205-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7d205-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d205-133">Request</span></span>

<span data-ttu-id="7d205-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d205-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7d205-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d205-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="7d205-136">C#</span><span class="sxs-lookup"><span data-stu-id="7d205-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d205-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d205-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d205-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d205-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7d205-139">Java</span><span class="sxs-lookup"><span data-stu-id="7d205-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7d205-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d205-140">Response</span></span>

<span data-ttu-id="7d205-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7d205-141">The following is an example of the response.</span></span>

> <span data-ttu-id="7d205-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="7d205-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


