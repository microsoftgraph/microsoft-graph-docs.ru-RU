---
title: Список объектов SubscribedSku
description: Получение списка коммерческих подписок, приобретенных организацией.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e5f6753f4712a2b7d90031fa78ae38e60e5e1425
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890580"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="4c137-103">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="4c137-103">List subscribedSkus</span></span>

<span data-ttu-id="4c137-104">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="4c137-104">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c137-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c137-105">Permissions</span></span>
<span data-ttu-id="4c137-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4c137-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c137-108">Permission type</span></span>      | <span data-ttu-id="4c137-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c137-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c137-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c137-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c137-111">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4c137-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c137-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c137-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c137-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c137-113">Not supported.</span></span>    |
|<span data-ttu-id="4c137-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4c137-114">Application</span></span> | <span data-ttu-id="4c137-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c137-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c137-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c137-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c137-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c137-117">Optional query parameters</span></span>
<span data-ttu-id="4c137-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="4c137-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c137-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c137-119">Request headers</span></span>

| <span data-ttu-id="4c137-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4c137-120">Name</span></span>       | <span data-ttu-id="4c137-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4c137-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="4c137-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c137-122">Authorization</span></span>  | <span data-ttu-id="4c137-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c137-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c137-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c137-125">Request body</span></span>
<span data-ttu-id="4c137-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c137-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c137-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c137-127">Response</span></span>

<span data-ttu-id="4c137-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c137-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c137-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4c137-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c137-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c137-130">Request</span></span>
<span data-ttu-id="4c137-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c137-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c137-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c137-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c137-133">C#</span><span class="sxs-lookup"><span data-stu-id="4c137-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c137-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c137-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c137-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c137-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c137-136">Java</span><span class="sxs-lookup"><span data-stu-id="4c137-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedskus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c137-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c137-137">Response</span></span>
<span data-ttu-id="4c137-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c137-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscribedSkus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
