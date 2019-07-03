---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c08884a68cce7f7f85275324d23b7948654e2dd1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446194"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="cae88-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="cae88-103">Get subscribedSku</span></span>
<span data-ttu-id="cae88-104">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="cae88-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="cae88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae88-105">Permissions</span></span>
<span data-ttu-id="cae88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cae88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae88-108">Permission type</span></span>      | <span data-ttu-id="cae88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae88-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cae88-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cae88-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cae88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae88-113">Not supported.</span></span>    |
|<span data-ttu-id="cae88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae88-114">Application</span></span> | <span data-ttu-id="cae88-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae88-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cae88-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cae88-117">Optional query parameters</span></span>
<span data-ttu-id="cae88-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="cae88-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cae88-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae88-119">Request headers</span></span>
| <span data-ttu-id="cae88-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cae88-120">Name</span></span>       | <span data-ttu-id="cae88-121">Тип</span><span class="sxs-lookup"><span data-stu-id="cae88-121">Type</span></span> | <span data-ttu-id="cae88-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cae88-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cae88-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cae88-123">Authorization</span></span>  | <span data-ttu-id="cae88-124">string</span><span class="sxs-lookup"><span data-stu-id="cae88-124">string</span></span>  | <span data-ttu-id="cae88-p102">&lt;Токен&gt; носителя. *Обязательный*</span><span class="sxs-lookup"><span data-stu-id="cae88-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae88-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae88-127">Request body</span></span>
<span data-ttu-id="cae88-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae88-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae88-129">Response</span></span>

<span data-ttu-id="cae88-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cae88-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cae88-131">Пример</span><span class="sxs-lookup"><span data-stu-id="cae88-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae88-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae88-132">Request</span></span>
<span data-ttu-id="cae88-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae88-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cae88-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae88-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cae88-135">C#</span><span class="sxs-lookup"><span data-stu-id="cae88-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cae88-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="cae88-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cae88-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cae88-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cae88-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae88-138">Response</span></span>
<span data-ttu-id="cae88-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cae88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus/$entity",
    "capabilityStatus": "Enabled",
    "consumedUnits": 14,
    "id": "48a80680-7326-48cd-9935-b556b81d3a4e_c7df2760-2c81-4ef7-b578-5b5392b571df",
    "prepaidUnits": {
        "enabled": 25,
        "suspended": 0,
        "warning": 0
    },
    "servicePlans": [
        {
            "servicePlanId": "8c098270-9dd4-4350-9b30-ba4703f3b36b",
            "servicePlanName": "ADALLOM_S_O365",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        },
        {
            "servicePlanId": "9f431833-0334-42de-a7dc-70aa40db46db",
            "servicePlanName": "LOCKBOX_ENTERPRISE",
            "provisioningStatus": "Success",
            "appliesTo": "User"
        }
    ],
    "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
    "skuPartNumber": "ENTERPRISEPREMIUM",
    "appliesTo": "User"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
