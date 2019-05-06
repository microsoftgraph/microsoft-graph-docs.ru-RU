---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e1cb64b412285ff4bfa36db049aa0ab2b0ea0afc
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33597950"
---
# <a name="list-organization"></a><span data-ttu-id="6ffab-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="6ffab-103">List organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ffab-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="6ffab-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ffab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffab-105">Permissions</span></span>
<span data-ttu-id="6ffab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ffab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ffab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ffab-108">Permission type</span></span>      | <span data-ttu-id="6ffab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ffab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ffab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ffab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ffab-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ffab-111">Not supported.</span></span>    |
|<span data-ttu-id="6ffab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ffab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ffab-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ffab-113">Not supported.</span></span>    |
|<span data-ttu-id="6ffab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ffab-114">Application</span></span> | <span data-ttu-id="6ffab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ffab-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ffab-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ffab-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ffab-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ffab-117">Optional query parameters</span></span>
<span data-ttu-id="6ffab-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ffab-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6ffab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ffab-119">Request headers</span></span>
| <span data-ttu-id="6ffab-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6ffab-120">Name</span></span>       | <span data-ttu-id="6ffab-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6ffab-121">Type</span></span> | <span data-ttu-id="6ffab-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6ffab-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6ffab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ffab-123">Authorization</span></span>  | <span data-ttu-id="6ffab-124">string</span><span class="sxs-lookup"><span data-stu-id="6ffab-124">string</span></span>  | <span data-ttu-id="6ffab-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6ffab-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ffab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ffab-127">Request body</span></span>
<span data-ttu-id="6ffab-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ffab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ffab-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6ffab-129">Response</span></span>

<span data-ttu-id="6ffab-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6ffab-130">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ffab-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6ffab-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ffab-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ffab-132">Request</span></span>
<span data-ttu-id="6ffab-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6ffab-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="6ffab-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ffab-134">Response</span></span>
<span data-ttu-id="6ffab-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6ffab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 500

{
  "value": [
    {
      "assignedPlans": [
        {
          "assignedDateTime": "2016-10-19T10:37:00Z",
          "capabilityStatus": "capabilityStatus-value",
          "service": "service-value",
          "servicePlanId": "servicePlanId-value"
        }
      ],
      "businessPhones": [
        "businessPhones-value"
      ],
      "city": "city-value",
      "country": "country-value",
      "countryLetterCode": "countryLetterCode-value",
      "displayName": "displayName-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6ffab-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="6ffab-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6ffab-139">Языках</span><span class="sxs-lookup"><span data-stu-id="6ffab-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ffab-140">Язык</span><span class="sxs-lookup"><span data-stu-id="6ffab-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
