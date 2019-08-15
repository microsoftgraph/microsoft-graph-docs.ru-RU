---
title: Список объектов SubscribedSku
description: Получение списка коммерческих подписок, приобретенных организацией.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 476fe93f2cef5828c7d747fc50b3613a6612dd0f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36409919"
---
# <a name="list-subscribedskus"></a><span data-ttu-id="64755-103">Список объектов SubscribedSku</span><span class="sxs-lookup"><span data-stu-id="64755-103">List subscribedSkus</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64755-104">Получение списка коммерческих подписок, приобретенных Организацией.</span><span class="sxs-lookup"><span data-stu-id="64755-104">Get the list of commercial subscriptions that an organization has acquired.</span></span>

## <a name="permissions"></a><span data-ttu-id="64755-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64755-105">Permissions</span></span>
<span data-ttu-id="64755-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64755-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="64755-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64755-108">Permission type</span></span>      | <span data-ttu-id="64755-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64755-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64755-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64755-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64755-111">Organization. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="64755-111">Organization.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="64755-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64755-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64755-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64755-113">Not supported.</span></span>    |
|<span data-ttu-id="64755-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64755-114">Application</span></span> | <span data-ttu-id="64755-115">Organization. Read. ALL, Directory. Read. ALL, Organization. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="64755-115">Organization.Read.All, Directory.Read.All, Organization.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64755-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64755-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /subscribedSkus
```
## <a name="optional-query-parameters"></a><span data-ttu-id="64755-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="64755-117">Optional query parameters</span></span>
<span data-ttu-id="64755-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="64755-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="64755-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64755-119">Request headers</span></span>

| <span data-ttu-id="64755-120">Имя</span><span class="sxs-lookup"><span data-stu-id="64755-120">Name</span></span>       | <span data-ttu-id="64755-121">Описание</span><span class="sxs-lookup"><span data-stu-id="64755-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="64755-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="64755-122">Authorization</span></span>  | <span data-ttu-id="64755-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="64755-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="64755-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64755-125">Request body</span></span>
<span data-ttu-id="64755-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="64755-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64755-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="64755-127">Response</span></span>

<span data-ttu-id="64755-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [subscribedSku](../resources/subscribedsku.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="64755-128">If successful, this method returns a `200 OK` response code and collection of [subscribedSku](../resources/subscribedsku.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64755-129">Пример</span><span class="sxs-lookup"><span data-stu-id="64755-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64755-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="64755-130">Request</span></span>
<span data-ttu-id="64755-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64755-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="64755-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="64755-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscribedskus"
}-->
```http
GET https://graph.microsoft.com/beta/subscribedSkus
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64755-133">C#</span><span class="sxs-lookup"><span data-stu-id="64755-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscribedskus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64755-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64755-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscribedskus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64755-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="64755-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscribedskus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="64755-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="64755-136">Response</span></span>
<span data-ttu-id="64755-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="64755-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
