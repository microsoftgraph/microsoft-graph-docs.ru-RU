---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4337ebb97e156f3e330732e74af436d3d96541d1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363706"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="dd51f-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="dd51f-103">Get subscribedSku</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd51f-104">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="dd51f-104">Get a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd51f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dd51f-105">Permissions</span></span>
<span data-ttu-id="dd51f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd51f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd51f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd51f-108">Permission type</span></span>      | <span data-ttu-id="dd51f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd51f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd51f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd51f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dd51f-111">Organization. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="dd51f-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd51f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd51f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd51f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd51f-113">Not supported.</span></span>    |
|<span data-ttu-id="dd51f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dd51f-114">Application</span></span> | <span data-ttu-id="dd51f-115">Organization. Read. ALL, Directory. Read. ALL, Organization. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="dd51f-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd51f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd51f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dd51f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dd51f-117">Optional query parameters</span></span>
<span data-ttu-id="dd51f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dd51f-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dd51f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dd51f-119">Request headers</span></span>

| <span data-ttu-id="dd51f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="dd51f-120">Name</span></span>       | <span data-ttu-id="dd51f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="dd51f-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="dd51f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dd51f-122">Authorization</span></span>  | <span data-ttu-id="dd51f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd51f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd51f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dd51f-125">Request body</span></span>
<span data-ttu-id="dd51f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dd51f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd51f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd51f-127">Response</span></span>

<span data-ttu-id="dd51f-128">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dd51f-128">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dd51f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dd51f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd51f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd51f-130">Request</span></span>
<span data-ttu-id="dd51f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd51f-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dd51f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd51f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd51f-133">C#</span><span class="sxs-lookup"><span data-stu-id="dd51f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedsku-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd51f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd51f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedsku-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd51f-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dd51f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedsku-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd51f-136">Java</span><span class="sxs-lookup"><span data-stu-id="dd51f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscribedsku-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dd51f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd51f-137">Response</span></span>
<span data-ttu-id="dd51f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd51f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
