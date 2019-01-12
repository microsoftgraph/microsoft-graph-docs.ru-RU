---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bf9a8213b4beaf62208b4857584da981367b6fcd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941823"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="2867f-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="2867f-103">Get subscribedSku</span></span>
<span data-ttu-id="2867f-104">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="2867f-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="2867f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2867f-105">Permissions</span></span>
<span data-ttu-id="2867f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2867f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2867f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2867f-108">Permission type</span></span>      | <span data-ttu-id="2867f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2867f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2867f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2867f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2867f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2867f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2867f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2867f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2867f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2867f-113">Not supported.</span></span>    |
|<span data-ttu-id="2867f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2867f-114">Application</span></span> | <span data-ttu-id="2867f-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2867f-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2867f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2867f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2867f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2867f-117">Optional query parameters</span></span>
<span data-ttu-id="2867f-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="2867f-118">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2867f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2867f-119">Request headers</span></span>
| <span data-ttu-id="2867f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2867f-120">Name</span></span>       | <span data-ttu-id="2867f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2867f-121">Type</span></span> | <span data-ttu-id="2867f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2867f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2867f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2867f-123">Authorization</span></span>  | <span data-ttu-id="2867f-124">строка</span><span class="sxs-lookup"><span data-stu-id="2867f-124">string</span></span>  | <span data-ttu-id="2867f-p102">&lt;Токен&gt; носителя. *Обязательный*</span><span class="sxs-lookup"><span data-stu-id="2867f-p102">Bearer &lt;token&gt;. *Required*</span></span> |

## <a name="request-body"></a><span data-ttu-id="2867f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2867f-127">Request body</span></span>
<span data-ttu-id="2867f-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2867f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2867f-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2867f-129">Response</span></span>

<span data-ttu-id="2867f-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2867f-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2867f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2867f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2867f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2867f-132">Request</span></span>
<span data-ttu-id="2867f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2867f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="2867f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2867f-134">Response</span></span>
<span data-ttu-id="2867f-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2867f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
