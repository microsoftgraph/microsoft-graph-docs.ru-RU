---
title: Список организаций
description: Получение списка объектов организаций.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b9bbcdc43c16e1010668417c728a5dbf8b1f1f09
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274398"
---
# <a name="list-organization"></a><span data-ttu-id="1dc78-103">Список организаций</span><span class="sxs-lookup"><span data-stu-id="1dc78-103">List organization</span></span>



<span data-ttu-id="1dc78-104">Получение списка объектов организаций.</span><span class="sxs-lookup"><span data-stu-id="1dc78-104">Retrieve a list of organization objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="1dc78-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dc78-105">Permissions</span></span>
<span data-ttu-id="1dc78-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dc78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dc78-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dc78-108">Permission type</span></span>      | <span data-ttu-id="1dc78-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dc78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dc78-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dc78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1dc78-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc78-111">User.Read, Directory.Read.All, Directory.ReadWrite.All</span></span>   |
|<span data-ttu-id="1dc78-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dc78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dc78-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dc78-113">Not supported.</span></span>    |
|<span data-ttu-id="1dc78-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dc78-114">Application</span></span> | <span data-ttu-id="1dc78-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc78-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="1dc78-116">Примечание. Приложения с разрешением User.Read могут читать только такие свойства организации, как *id*, *displayName* и *verifiedDomains*.</span><span class="sxs-lookup"><span data-stu-id="1dc78-116">Note: Applications granted the User.Read permission are able to read only the *id*, *displayName*, and *verifiedDomains* properties of the organization.</span></span>  <span data-ttu-id="1dc78-117">Для всех остальных свойств возвращается значение `null`.</span><span class="sxs-lookup"><span data-stu-id="1dc78-117">All other properties will return with `null` values.</span></span> <span data-ttu-id="1dc78-118">Читать все свойства можно с помощью Directory.Read.All.</span><span class="sxs-lookup"><span data-stu-id="1dc78-118">To read all properties, use Directory.Read.All.</span></span>

## <a name="http-request"></a><span data-ttu-id="1dc78-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dc78-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /organization
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1dc78-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1dc78-120">Optional query parameters</span></span>
<span data-ttu-id="1dc78-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1dc78-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1dc78-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dc78-122">Request headers</span></span>
| <span data-ttu-id="1dc78-123">Имя</span><span class="sxs-lookup"><span data-stu-id="1dc78-123">Name</span></span>       | <span data-ttu-id="1dc78-124">Тип</span><span class="sxs-lookup"><span data-stu-id="1dc78-124">Type</span></span> | <span data-ttu-id="1dc78-125">Описание</span><span class="sxs-lookup"><span data-stu-id="1dc78-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1dc78-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dc78-126">Authorization</span></span>  | <span data-ttu-id="1dc78-127">string</span><span class="sxs-lookup"><span data-stu-id="1dc78-127">string</span></span>  | <span data-ttu-id="1dc78-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dc78-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dc78-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dc78-130">Request body</span></span>
<span data-ttu-id="1dc78-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dc78-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc78-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="1dc78-132">Response</span></span>

<span data-ttu-id="1dc78-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [organization](../resources/organization.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1dc78-133">If successful, this method returns a `200 OK` response code and collection of [organization](../resources/organization.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1dc78-134">Пример</span><span class="sxs-lookup"><span data-stu-id="1dc78-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dc78-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dc78-135">Request</span></span>
<span data-ttu-id="1dc78-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dc78-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organization"
}-->
```http
GET https://graph.microsoft.com/beta/organization
```
##### <a name="response"></a><span data-ttu-id="1dc78-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dc78-137">Response</span></span>
<span data-ttu-id="1dc78-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1dc78-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1dc78-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="1dc78-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1dc78-142">C#</span><span class="sxs-lookup"><span data-stu-id="1dc78-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dc78-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="1dc78-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_organization-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="1dc78-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1dc78-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_organization-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
