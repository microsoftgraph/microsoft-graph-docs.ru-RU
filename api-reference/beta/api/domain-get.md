---
title: Получение домена
description: Получение свойств и связей объекта домена.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fa145397ccec8da6444cf0be6c88215e96afe3da
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260476"
---
# <a name="get-domain"></a><span data-ttu-id="b9f46-103">Получение домена</span><span class="sxs-lookup"><span data-stu-id="b9f46-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9f46-104">Получение свойств и связей объекта домена.</span><span class="sxs-lookup"><span data-stu-id="b9f46-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9f46-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f46-105">Permissions</span></span>

<span data-ttu-id="b9f46-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b9f46-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9f46-108">Permission type</span></span>      | <span data-ttu-id="b9f46-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9f46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9f46-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9f46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b9f46-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9f46-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="b9f46-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9f46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9f46-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b9f46-113">Not supported.</span></span>    |
|<span data-ttu-id="b9f46-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9f46-114">Application</span></span> | <span data-ttu-id="b9f46-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f46-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9f46-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9f46-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="b9f46-117">В качестве параметра {id} укажите домен, используя его полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="b9f46-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="b9f46-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9f46-118">Optional query parameters</span></span>

<span data-ttu-id="b9f46-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b9f46-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9f46-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b9f46-120">Request headers</span></span>

| <span data-ttu-id="b9f46-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b9f46-121">Name</span></span>      |<span data-ttu-id="b9f46-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b9f46-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9f46-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b9f46-123">Authorization</span></span>  | <span data-ttu-id="b9f46-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b9f46-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b9f46-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b9f46-126">Content-Type</span></span>  | <span data-ttu-id="b9f46-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f46-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9f46-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b9f46-128">Request body</span></span>
<span data-ttu-id="b9f46-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b9f46-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9f46-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9f46-130">Response</span></span>

<span data-ttu-id="b9f46-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [domain](../resources/domain.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b9f46-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b9f46-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b9f46-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b9f46-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b9f46-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="b9f46-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b9f46-134">Response</span></span>
<span data-ttu-id="b9f46-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b9f46-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b9f46-137">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b9f46-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b9f46-138">C#</span><span class="sxs-lookup"><span data-stu-id="b9f46-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b9f46-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="b9f46-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b9f46-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b9f46-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
