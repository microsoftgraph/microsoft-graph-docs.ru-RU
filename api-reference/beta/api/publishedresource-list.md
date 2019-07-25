---
title: Список Публишедресаурцес
description: Получение списка объектов Публишедресаурце.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0bc2dc4ad763bd3cdb45d072f3d95847c17007b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875084"
---
# <a name="list-publishedresources"></a><span data-ttu-id="db665-103">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="db665-103">List publishedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db665-104">Получение списка объектов [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="db665-104">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="db665-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db665-105">Permissions</span></span>

<span data-ttu-id="db665-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db665-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db665-108">Permission type</span></span>                        | <span data-ttu-id="db665-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db665-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="db665-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db665-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="db665-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="db665-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="db665-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db665-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db665-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db665-113">Not supported.</span></span> |
| <span data-ttu-id="db665-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db665-114">Application</span></span>                            | <span data-ttu-id="db665-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db665-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db665-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db665-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="db665-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="db665-117">Optional query parameters</span></span>

<span data-ttu-id="db665-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="db665-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="db665-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db665-119">Request headers</span></span>

| <span data-ttu-id="db665-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db665-120">Name</span></span>      |<span data-ttu-id="db665-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db665-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="db665-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db665-122">Authorization</span></span> | <span data-ttu-id="db665-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="db665-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="db665-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="db665-124">Request body</span></span>

<span data-ttu-id="db665-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db665-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db665-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="db665-126">Response</span></span>

<span data-ttu-id="db665-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="db665-127">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db665-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="db665-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db665-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="db665-129">Request</span></span>

<span data-ttu-id="db665-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db665-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="db665-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="db665-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db665-132">C#</span><span class="sxs-lookup"><span data-stu-id="db665-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db665-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="db665-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db665-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="db665-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="db665-135">Java</span><span class="sxs-lookup"><span data-stu-id="db665-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db665-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="db665-136">Response</span></span>

<span data-ttu-id="db665-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db665-137">The following is an example of the response.</span></span>

> <span data-ttu-id="db665-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="db665-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List publishedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
