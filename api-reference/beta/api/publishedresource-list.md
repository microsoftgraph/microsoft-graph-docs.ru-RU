---
title: Список Публишедресаурцес
description: Получение списка объектов Публишедресаурце.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 102c541c8ffce01ae16b83340dd2e61f8fd74f5b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309244"
---
# <a name="list-publishedresources"></a><span data-ttu-id="efb9a-103">Список Публишедресаурцес</span><span class="sxs-lookup"><span data-stu-id="efb9a-103">List publishedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="efb9a-104">Получение списка объектов [публишедресаурце](../resources/publishedresource.md) .</span><span class="sxs-lookup"><span data-stu-id="efb9a-104">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="efb9a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="efb9a-105">Permissions</span></span>

<span data-ttu-id="efb9a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="efb9a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="efb9a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="efb9a-108">Permission type</span></span>                        | <span data-ttu-id="efb9a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="efb9a-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="efb9a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="efb9a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="efb9a-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="efb9a-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="efb9a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="efb9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="efb9a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb9a-113">Not supported.</span></span> |
| <span data-ttu-id="efb9a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="efb9a-114">Application</span></span>                            | <span data-ttu-id="efb9a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efb9a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="efb9a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="efb9a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="efb9a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="efb9a-117">Optional query parameters</span></span>

<span data-ttu-id="efb9a-118">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="efb9a-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="efb9a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="efb9a-119">Request headers</span></span>

| <span data-ttu-id="efb9a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="efb9a-120">Name</span></span>      |<span data-ttu-id="efb9a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="efb9a-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="efb9a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="efb9a-122">Authorization</span></span> | <span data-ttu-id="efb9a-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="efb9a-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="efb9a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="efb9a-124">Request body</span></span>

<span data-ttu-id="efb9a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="efb9a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="efb9a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb9a-126">Response</span></span>

<span data-ttu-id="efb9a-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="efb9a-127">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="efb9a-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="efb9a-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="efb9a-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="efb9a-129">Request</span></span>

<span data-ttu-id="efb9a-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="efb9a-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="efb9a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="efb9a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="efb9a-132">C#</span><span class="sxs-lookup"><span data-stu-id="efb9a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-publishedresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="efb9a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="efb9a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-publishedresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="efb9a-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="efb9a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-publishedresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="efb9a-135">Java</span><span class="sxs-lookup"><span data-stu-id="efb9a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-publishedresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="efb9a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="efb9a-136">Response</span></span>

<span data-ttu-id="efb9a-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="efb9a-137">The following is an example of the response.</span></span>

> <span data-ttu-id="efb9a-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="efb9a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
