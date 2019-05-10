---
title: Список объектов SubscribedSku
description: Получение списка коммерческих подписок, приобретенных организацией.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 641eb0306e2f12340c7d7740db347d36fb47b4a7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33603241"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="f8be6-103">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="f8be6-103">List subscribedSkus</span></span>
<span data-ttu-id="f8be6-104">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="f8be6-104">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8be6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f8be6-105">Permissions</span></span>
<span data-ttu-id="f8be6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8be6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f8be6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f8be6-108">Permission type</span></span>      | <span data-ttu-id="f8be6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f8be6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8be6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f8be6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f8be6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f8be6-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f8be6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f8be6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8be6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8be6-113">Not supported.</span></span>    |
|<span data-ttu-id="f8be6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f8be6-114">Application</span></span> | <span data-ttu-id="f8be6-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8be6-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8be6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f8be6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f8be6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f8be6-117">Optional query parameters</span></span>
<span data-ttu-id="f8be6-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="f8be6-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8be6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f8be6-119">Request headers</span></span>
| <span data-ttu-id="f8be6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f8be6-120">Name</span></span>       | <span data-ttu-id="f8be6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f8be6-121">Type</span></span> | <span data-ttu-id="f8be6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f8be6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f8be6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8be6-123">Authorization</span></span>  | <span data-ttu-id="f8be6-124">string</span><span class="sxs-lookup"><span data-stu-id="f8be6-124">string</span></span>  | <span data-ttu-id="f8be6-p102">&lt;Токен&gt; носителя. *Обязательный*</span><span class="sxs-lookup"><span data-stu-id="f8be6-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8be6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f8be6-127">Request body</span></span>
<span data-ttu-id="f8be6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f8be6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8be6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8be6-129">Response</span></span>

<span data-ttu-id="f8be6-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f8be6-130">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8be6-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f8be6-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8be6-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f8be6-132">Request</span></span>
<span data-ttu-id="f8be6-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f8be6-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
##### <a name="response"></a><span data-ttu-id="f8be6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f8be6-134">Response</span></span>
<span data-ttu-id="f8be6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f8be6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscribedSkus",
    "value": [
        {
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
                }
            ],
            "skuId": "c7df2760-2c81-4ef7-b578-5b5392b571df",
            "skuPartNumber": "ENTERPRISEPREMIUM",
            "appliesTo": "User"
        },
        {
            "capabilityStatus": "Suspended",
            "consumedUnits": 14,
            "id": "48a80680-7326-48cd-9935-b556b81d3a4e_d17b27af-3f49-4822-99f9-56a661538792",
            "prepaidUnits": {
                "enabled": 0,
                "suspended": 25,
                "warning": 0
            },
            "servicePlans": [
                {
                    "servicePlanId": "f9646fb2-e3b2-4309-95de-dc4833737456",
                    "servicePlanName": "CRMSTANDARD",
                    "provisioningStatus": "Disabled",
                    "appliesTo": "User"
                }
            ],
            "skuId": "d17b27af-3f49-4822-99f9-56a661538792",
            "skuPartNumber": "CRMSTANDARD",
            "appliesTo": "User"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f8be6-138">Образец кода SDK</span><span class="sxs-lookup"><span data-stu-id="f8be6-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f8be6-139">C#</span><span class="sxs-lookup"><span data-stu-id="f8be6-139">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscribedskus-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f8be6-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f8be6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscribedskus-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/subscribedsku-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/subscribedsku-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
