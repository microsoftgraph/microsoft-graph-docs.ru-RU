---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: dfb973f8a581699ab9bd79851f096288462b9d8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044368"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="56eaf-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="56eaf-103">Get subscribedSku</span></span>

<span data-ttu-id="56eaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56eaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56eaf-105">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="56eaf-105">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="56eaf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56eaf-106">Permissions</span></span>
<span data-ttu-id="56eaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56eaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56eaf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56eaf-109">Permission type</span></span>      | <span data-ttu-id="56eaf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56eaf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56eaf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56eaf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="56eaf-112">Organization. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="56eaf-112">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56eaf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56eaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56eaf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56eaf-114">Not supported.</span></span>    |
|<span data-ttu-id="56eaf-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="56eaf-115">Application</span></span> | <span data-ttu-id="56eaf-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56eaf-116">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56eaf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56eaf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56eaf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="56eaf-118">Optional query parameters</span></span>
<span data-ttu-id="56eaf-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="56eaf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56eaf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56eaf-120">Request headers</span></span>

| <span data-ttu-id="56eaf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="56eaf-121">Name</span></span>       | <span data-ttu-id="56eaf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="56eaf-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="56eaf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56eaf-123">Authorization</span></span>  | <span data-ttu-id="56eaf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56eaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56eaf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56eaf-126">Request body</span></span>
<span data-ttu-id="56eaf-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56eaf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56eaf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="56eaf-128">Response</span></span>

<span data-ttu-id="56eaf-129">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="56eaf-129">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56eaf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="56eaf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56eaf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="56eaf-131">Request</span></span>
<span data-ttu-id="56eaf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56eaf-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="56eaf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="56eaf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="c"></a>[<span data-ttu-id="56eaf-134">C#</span><span class="sxs-lookup"><span data-stu-id="56eaf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="56eaf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="56eaf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="56eaf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="56eaf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56eaf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="56eaf-137">Response</span></span>
<span data-ttu-id="56eaf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="56eaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscribedSku"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 450

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get subscribedSku",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


