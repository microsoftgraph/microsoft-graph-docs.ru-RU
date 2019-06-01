---
title: Вывод объекта SubscribedSku
description: Получение определенной коммерческой подписки, приобретенной организацией.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c780ef1460c98e558eee03ae8535b150b25c99b8
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657457"
---
# <a name="get-subscribedsku"></a><span data-ttu-id="aa873-103">Вывод объекта SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="aa873-103">Get subscribedSku</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa873-104">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="aa873-104">Retrieve a specific commercial subscription that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa873-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa873-105">Permissions</span></span>
<span data-ttu-id="aa873-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa873-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="aa873-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa873-108">Permission type</span></span>      | <span data-ttu-id="aa873-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa873-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aa873-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa873-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aa873-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aa873-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aa873-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa873-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa873-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa873-113">Not supported.</span></span>    |
|<span data-ttu-id="aa873-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aa873-114">Application</span></span> | <span data-ttu-id="aa873-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa873-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aa873-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa873-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aa873-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aa873-117">Optional query parameters</span></span>
<span data-ttu-id="aa873-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aa873-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aa873-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa873-119">Request headers</span></span>
| <span data-ttu-id="aa873-120">Имя</span><span class="sxs-lookup"><span data-stu-id="aa873-120">Name</span></span>       | <span data-ttu-id="aa873-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aa873-121">Type</span></span> | <span data-ttu-id="aa873-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aa873-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="aa873-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa873-123">Authorization</span></span>  | <span data-ttu-id="aa873-124">string</span><span class="sxs-lookup"><span data-stu-id="aa873-124">string</span></span>  | <span data-ttu-id="aa873-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa873-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa873-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="aa873-127">Request body</span></span>
<span data-ttu-id="aa873-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aa873-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa873-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="aa873-129">Response</span></span>

<span data-ttu-id="aa873-130">В случае успеха этот метод возвращает код отклика `200 OK` и объект [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa873-130">If successful, this method returns a `200 OK` response code and [subscribedSku](../resources/subscribedsku.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aa873-131">Пример</span><span class="sxs-lookup"><span data-stu-id="aa873-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aa873-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa873-132">Request</span></span>
<span data-ttu-id="aa873-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aa873-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_subscribedsku"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus/{id}
```
##### <a name="response"></a><span data-ttu-id="aa873-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa873-134">Response</span></span>
<span data-ttu-id="aa873-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aa873-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="aa873-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="aa873-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aa873-139">C#</span><span class="sxs-lookup"><span data-stu-id="aa873-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aa873-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="aa873-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscribedsku-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscribedsku-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
