---
title: Получение orgContact
description: Получение свойств и связей объекта orgcontact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 71ea3dae98a6fa1f5d1ae9c2c0e4dd264026ba57
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266852"
---
# <a name="get-orgcontact"></a><span data-ttu-id="f883b-103">Получение orgContact</span><span class="sxs-lookup"><span data-stu-id="f883b-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f883b-104">Получение свойств и связей объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="f883b-104">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f883b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f883b-105">Permissions</span></span>
<span data-ttu-id="f883b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f883b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f883b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f883b-108">Permission type</span></span>      | <span data-ttu-id="f883b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f883b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f883b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f883b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f883b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f883b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f883b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f883b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f883b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f883b-113">Not supported.</span></span>    |
|<span data-ttu-id="f883b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f883b-114">Application</span></span> | <span data-ttu-id="f883b-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f883b-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f883b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f883b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f883b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f883b-117">Optional query parameters</span></span>
<span data-ttu-id="f883b-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f883b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f883b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f883b-119">Request headers</span></span>
| <span data-ttu-id="f883b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f883b-120">Name</span></span>       | <span data-ttu-id="f883b-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f883b-121">Type</span></span> | <span data-ttu-id="f883b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f883b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f883b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f883b-123">Authorization</span></span>  | <span data-ttu-id="f883b-124">string</span><span class="sxs-lookup"><span data-stu-id="f883b-124">string</span></span>  | <span data-ttu-id="f883b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f883b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f883b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f883b-127">Request body</span></span>
<span data-ttu-id="f883b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f883b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f883b-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="f883b-129">Response</span></span>

<span data-ttu-id="f883b-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f883b-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f883b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="f883b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f883b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="f883b-132">Request</span></span>
<span data-ttu-id="f883b-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f883b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="f883b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="f883b-134">Response</span></span>
<span data-ttu-id="f883b-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f883b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f883b-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="f883b-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f883b-139">C#</span><span class="sxs-lookup"><span data-stu-id="f883b-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_orgcontact-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f883b-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f883b-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_orgcontact-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f883b-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f883b-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_orgcontact-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/orgcontact-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
