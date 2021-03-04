---
title: Список объектов SubscribedSku
description: Получение списка коммерческих подписок, приобретенных организацией.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a317ee834ffffde249d25cc238ef589f623c4f04
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443547"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="e4299-103">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="e4299-103">List subscribedSkus</span></span>

<span data-ttu-id="e4299-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4299-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4299-105">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="e4299-105">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4299-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4299-106">Permissions</span></span>
<span data-ttu-id="e4299-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e4299-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4299-109">Permission type</span></span>      | <span data-ttu-id="e4299-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4299-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4299-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4299-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e4299-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4299-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4299-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4299-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4299-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4299-114">Not supported.</span></span>    |
|<span data-ttu-id="e4299-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e4299-115">Application</span></span> | <span data-ttu-id="e4299-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4299-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4299-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4299-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e4299-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4299-118">Optional query parameters</span></span>

<span data-ttu-id="e4299-119">Этот метод не поддерживает [параметры запроса OData,](/graph//query-parameters) чтобы помочь настроить ответ `$filter` (не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="e4299-119">This method does not support the [OData query parameters](/graph//query-parameters) to help customize the response (`$filter` is not supported).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4299-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4299-120">Request headers</span></span>

| <span data-ttu-id="e4299-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e4299-121">Name</span></span>       | <span data-ttu-id="e4299-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e4299-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e4299-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4299-123">Authorization</span></span>  | <span data-ttu-id="e4299-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4299-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4299-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4299-126">Request body</span></span>
<span data-ttu-id="e4299-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4299-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4299-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4299-128">Response</span></span>

<span data-ttu-id="e4299-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4299-129">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4299-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e4299-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4299-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4299-131">Request</span></span>
<span data-ttu-id="e4299-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4299-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e4299-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4299-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="c"></a>[<span data-ttu-id="e4299-134">C#</span><span class="sxs-lookup"><span data-stu-id="e4299-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4299-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4299-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4299-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4299-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4299-137">Java</span><span class="sxs-lookup"><span data-stu-id="e4299-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e4299-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4299-138">Response</span></span>
<span data-ttu-id="e4299-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4299-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
  "value": [
    {
      "capabilityStatus": "capabilityStatus-value",
      "consumedUnits": 99,
      "prepaidUnits": {
        "enabled": 99,
        "suspended": 99,
        "warning": 99
      },
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


