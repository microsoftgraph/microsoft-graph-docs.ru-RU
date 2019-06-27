---
title: Список доменов
description: Получение списка объектов Domain.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ebe0f6fa53e146044a641eafe81b5f139628ed42
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272116"
---
# <a name="list-domains"></a><span data-ttu-id="c3014-103">Список доменов</span><span class="sxs-lookup"><span data-stu-id="c3014-103">List domains</span></span>

<span data-ttu-id="c3014-104">Получение списка объектов Domain.</span><span class="sxs-lookup"><span data-stu-id="c3014-104">Retrieve a list of domain objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3014-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3014-105">Permissions</span></span>
<span data-ttu-id="c3014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3014-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3014-108">Permission type</span></span>      | <span data-ttu-id="c3014-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3014-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3014-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3014-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3014-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3014-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="c3014-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3014-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3014-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3014-113">Not supported.</span></span>    |
|<span data-ttu-id="c3014-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3014-114">Application</span></span> | <span data-ttu-id="c3014-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3014-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3014-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3014-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3014-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c3014-117">Optional query parameters</span></span>
<span data-ttu-id="c3014-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c3014-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3014-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3014-119">Request headers</span></span>
| <span data-ttu-id="c3014-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c3014-120">Name</span></span>      |<span data-ttu-id="c3014-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c3014-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3014-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3014-122">Authorization</span></span>  | <span data-ttu-id="c3014-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3014-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="c3014-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3014-125">Accept</span></span>         | <span data-ttu-id="c3014-126">приложение/JSON;</span><span class="sxs-lookup"><span data-stu-id="c3014-126">application/json;</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3014-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c3014-127">Request body</span></span>
<span data-ttu-id="c3014-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c3014-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3014-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="c3014-129">Response</span></span>

<span data-ttu-id="c3014-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [domain](../resources/domain.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3014-130">If successful, this method returns a `200 OK` response code and collection of [domain](../resources/domain.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3014-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c3014-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3014-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3014-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domains"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains
```
##### <a name="response"></a><span data-ttu-id="c3014-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3014-133">Response</span></span>
<span data-ttu-id="c3014-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3014-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "value": [
    {
      "authenticationType": "authenticationType-value",
      "availabilityStatus": "availabilityStatus-value",
      "isAdminManaged": true,
      "isDefault": true,
      "isInitial": true,
      "isRoot": true,
      "id": "contoso.com",
      "supportedServices": [
        "Email",
        "OfficeCommunicationsOnline"
      ]
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c3014-136">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c3014-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c3014-137">C#</span><span class="sxs-lookup"><span data-stu-id="c3014-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_domains-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c3014-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c3014-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_domains-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c3014-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c3014-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_domains-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domains",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
