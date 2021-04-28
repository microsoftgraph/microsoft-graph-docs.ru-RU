---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0493d8ccf201739d1d59d06933a75d27d5b0c08d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050299"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="329da-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="329da-103">Get subscribedSku</span></span>

<span data-ttu-id="329da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="329da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="329da-105">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="329da-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="329da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="329da-106">Permissions</span></span>
<span data-ttu-id="329da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="329da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="329da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="329da-109">Permission type</span></span>      | <span data-ttu-id="329da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="329da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="329da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="329da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="329da-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="329da-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="329da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="329da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="329da-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="329da-114">Not supported.</span></span>    |
|<span data-ttu-id="329da-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="329da-115">Application</span></span> | <span data-ttu-id="329da-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="329da-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="329da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="329da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="329da-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="329da-118">Optional query parameters</span></span>
<span data-ttu-id="329da-119">Этот метод **не** поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика (например, $filter не поддерживается).</span><span class="sxs-lookup"><span data-stu-id="329da-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="329da-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="329da-120">Request headers</span></span>

| <span data-ttu-id="329da-121">Имя</span><span class="sxs-lookup"><span data-stu-id="329da-121">Name</span></span>       | <span data-ttu-id="329da-122">Описание</span><span class="sxs-lookup"><span data-stu-id="329da-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="329da-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="329da-123">Authorization</span></span>  | <span data-ttu-id="329da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="329da-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="329da-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="329da-126">Request body</span></span>
<span data-ttu-id="329da-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="329da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="329da-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="329da-128">Response</span></span>

<span data-ttu-id="329da-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="329da-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="329da-130">Пример</span><span class="sxs-lookup"><span data-stu-id="329da-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="329da-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="329da-131">Request</span></span>
<span data-ttu-id="329da-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="329da-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="329da-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="329da-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="329da-134">C#</span><span class="sxs-lookup"><span data-stu-id="329da-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="329da-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="329da-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="329da-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="329da-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="329da-137">Java</span><span class="sxs-lookup"><span data-stu-id="329da-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedsku-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="329da-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="329da-138">Response</span></span>
<span data-ttu-id="329da-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="329da-139">Here is an example of the response.</span></span> <span data-ttu-id="329da-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="329da-140">Note: The response object shown here might be shortened for readability.</span></span>
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
