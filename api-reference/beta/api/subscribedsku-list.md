---
title: Список объектов SubscribedSku
description: Получение списка коммерческих подписок, приобретенных организацией.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6bf83162dc1d25180c009814d9135780b02c970
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35453546"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="a80e9-103">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="a80e9-103">List subscribedSkus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a80e9-104">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="a80e9-104">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="a80e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a80e9-105">Permissions</span></span>
<span data-ttu-id="a80e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a80e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a80e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a80e9-108">Permission type</span></span>      | <span data-ttu-id="a80e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a80e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a80e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a80e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a80e9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a80e9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a80e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a80e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a80e9-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a80e9-113">Not supported.</span></span>    |
|<span data-ttu-id="a80e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a80e9-114">Application</span></span> | <span data-ttu-id="a80e9-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a80e9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a80e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a80e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a80e9-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a80e9-117">Optional query parameters</span></span>
<span data-ttu-id="a80e9-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a80e9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a80e9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a80e9-119">Request headers</span></span>
| <span data-ttu-id="a80e9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a80e9-120">Name</span></span>       | <span data-ttu-id="a80e9-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a80e9-121">Type</span></span> | <span data-ttu-id="a80e9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a80e9-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a80e9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a80e9-123">Authorization</span></span>  | <span data-ttu-id="a80e9-124">string</span><span class="sxs-lookup"><span data-stu-id="a80e9-124">string</span></span>  | <span data-ttu-id="a80e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a80e9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a80e9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a80e9-127">Request body</span></span>
<span data-ttu-id="a80e9-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a80e9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a80e9-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a80e9-129">Response</span></span>

<span data-ttu-id="a80e9-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a80e9-130">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a80e9-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a80e9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a80e9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a80e9-132">Request</span></span>
<span data-ttu-id="a80e9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a80e9-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a80e9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a80e9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a80e9-135">C#</span><span class="sxs-lookup"><span data-stu-id="a80e9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a80e9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="a80e9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a80e9-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a80e9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a80e9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a80e9-138">Response</span></span>
<span data-ttu-id="a80e9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a80e9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
