---
title: Получение Публишедресаурце
description: Получение свойств и связей объекта [публишедресаурце](../resources/publishedresource.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ecfbaea8ff4e573326c2a591e85d2d0c90d4fa4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412371"
---
# <a name="get-publishedresource"></a><span data-ttu-id="5dc67-103">Получение Публишедресаурце</span><span class="sxs-lookup"><span data-stu-id="5dc67-103">Get publishedResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dc67-104">Получение свойств и связей объекта [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="5dc67-104">Retrieve the properties and relationships of [publishedResource](../resources/publishedresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5dc67-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5dc67-105">Permissions</span></span>

<span data-ttu-id="5dc67-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dc67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5dc67-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5dc67-108">Permission type</span></span>                        | <span data-ttu-id="5dc67-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5dc67-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="5dc67-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5dc67-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5dc67-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5dc67-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="5dc67-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5dc67-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dc67-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc67-113">Not supported.</span></span> |
| <span data-ttu-id="5dc67-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5dc67-114">Application</span></span>                            | <span data-ttu-id="5dc67-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5dc67-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5dc67-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5dc67-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5dc67-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5dc67-117">Optional query parameters</span></span>

<span data-ttu-id="5dc67-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc67-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5dc67-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5dc67-119">Request headers</span></span>

| <span data-ttu-id="5dc67-120">Имя</span><span class="sxs-lookup"><span data-stu-id="5dc67-120">Name</span></span>      |<span data-ttu-id="5dc67-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5dc67-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5dc67-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5dc67-122">Authorization</span></span> | <span data-ttu-id="5dc67-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="5dc67-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dc67-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5dc67-124">Request body</span></span>

<span data-ttu-id="5dc67-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5dc67-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5dc67-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dc67-126">Response</span></span>

<span data-ttu-id="5dc67-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и запрошенный объект [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc67-127">If successful, this method returns a `200 OK` response code and the requested [publishedResource](../resources/publishedresource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5dc67-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="5dc67-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5dc67-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="5dc67-129">Request</span></span>

<span data-ttu-id="5dc67-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5dc67-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5dc67-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dc67-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresource"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/aed0b780-965f-4149-85c5-a8c73e58b67d/?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5dc67-132">C#</span><span class="sxs-lookup"><span data-stu-id="5dc67-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dc67-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dc67-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5dc67-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="5dc67-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5dc67-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="5dc67-135">Response</span></span>

<span data-ttu-id="5dc67-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5dc67-136">The following is an example of the response.</span></span>

> <span data-ttu-id="5dc67-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5dc67-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
