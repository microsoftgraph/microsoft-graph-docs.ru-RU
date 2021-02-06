---
title: Get publishedResource
description: Извлечение свойств и связей объекта [publishedResource.](../resources/publishedresource.md)
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 6b0f84de5dfdcde391094e71dbcde451dc4fe3b0
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135536"
---
# <a name="get-publishedresource"></a><span data-ttu-id="40159-103">Get publishedResource</span><span class="sxs-lookup"><span data-stu-id="40159-103">Get publishedResource</span></span>

<span data-ttu-id="40159-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40159-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40159-105">Извлечение свойств и связей [объекта publishedResource.](../resources/publishedresource.md)</span><span class="sxs-lookup"><span data-stu-id="40159-105">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="40159-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="40159-106">Permissions</span></span>

<span data-ttu-id="40159-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40159-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40159-109">Permission type</span></span>                        | <span data-ttu-id="40159-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="40159-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="40159-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40159-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="40159-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40159-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="40159-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40159-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40159-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40159-114">Not supported.</span></span> |
| <span data-ttu-id="40159-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40159-115">Application</span></span>                            | <span data-ttu-id="40159-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40159-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="40159-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40159-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40159-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="40159-118">Optional query parameters</span></span>

<span data-ttu-id="40159-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="40159-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40159-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40159-120">Request headers</span></span>

| <span data-ttu-id="40159-121">Имя</span><span class="sxs-lookup"><span data-stu-id="40159-121">Name</span></span>      |<span data-ttu-id="40159-122">Описание</span><span class="sxs-lookup"><span data-stu-id="40159-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="40159-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40159-123">Authorization</span></span> | <span data-ttu-id="40159-124">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="40159-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="40159-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40159-125">Request body</span></span>

<span data-ttu-id="40159-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="40159-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40159-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="40159-127">Response</span></span>

<span data-ttu-id="40159-128">В случае успеха этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [publishedResource](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="40159-128">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40159-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="40159-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="40159-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="40159-130">Request</span></span>

<span data-ttu-id="40159-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40159-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="40159-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="40159-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="c"></a>[<span data-ttu-id="40159-133">C#</span><span class="sxs-lookup"><span data-stu-id="40159-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40159-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40159-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40159-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40159-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40159-136">Java</span><span class="sxs-lookup"><span data-stu-id="40159-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="40159-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="40159-137">Response</span></span>

<span data-ttu-id="40159-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="40159-138">The following is an example of the response.</span></span>

> <span data-ttu-id="40159-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="40159-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



