---
title: Get publishedResource
description: Извлечение свойств и связей объекта [publishedResource.](../resources/publishedresource.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 00b3242dbef55afe0f01571fabac848aa8e391db
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055185"
---
# <a name="get-publishedresource"></a><span data-ttu-id="54b6c-103">Get publishedResource</span><span class="sxs-lookup"><span data-stu-id="54b6c-103">Get publishedResource</span></span>

<span data-ttu-id="54b6c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54b6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b6c-105">Извлечение свойств и связей [объекта publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="54b6c-105">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54b6c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54b6c-106">Permissions</span></span>

<span data-ttu-id="54b6c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54b6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54b6c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54b6c-109">Permission type</span></span>                        | <span data-ttu-id="54b6c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54b6c-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="54b6c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54b6c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54b6c-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54b6c-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="54b6c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54b6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54b6c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54b6c-114">Not supported.</span></span> |
| <span data-ttu-id="54b6c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54b6c-115">Application</span></span>                            | <span data-ttu-id="54b6c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54b6c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="54b6c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54b6c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54b6c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="54b6c-118">Optional query parameters</span></span>

<span data-ttu-id="54b6c-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="54b6c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="54b6c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54b6c-120">Request headers</span></span>

| <span data-ttu-id="54b6c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="54b6c-121">Name</span></span>      |<span data-ttu-id="54b6c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="54b6c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54b6c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54b6c-123">Authorization</span></span> | <span data-ttu-id="54b6c-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="54b6c-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="54b6c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54b6c-125">Request body</span></span>

<span data-ttu-id="54b6c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54b6c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54b6c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b6c-127">Response</span></span>

<span data-ttu-id="54b6c-128">В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [publishedResource](../resources/publishedresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="54b6c-128">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54b6c-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="54b6c-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54b6c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="54b6c-130">Request</span></span>

<span data-ttu-id="54b6c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54b6c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54b6c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="54b6c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="54b6c-133">C#</span><span class="sxs-lookup"><span data-stu-id="54b6c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54b6c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54b6c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54b6c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54b6c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54b6c-136">Java</span><span class="sxs-lookup"><span data-stu-id="54b6c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54b6c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="54b6c-137">Response</span></span>

<span data-ttu-id="54b6c-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54b6c-138">The following is an example of the response.</span></span>

> <span data-ttu-id="54b6c-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54b6c-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "publishingType": "provisioning",
    "displayName": "Demo provisioning",
    "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
    "resourceName": "domain1.contoso.com",
    "agentGroups": [
        {
            "id": "2d55ed41-1619-4848-92bb-0576d3038682",
            "displayName": "Group 1"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



