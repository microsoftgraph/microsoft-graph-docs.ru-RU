---
title: Список контрактов
description: Получение списка объектов контракта, связанных с клиентом партнера.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e2afce05d8be51b02ccfbf8646cb17d1e621f37
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35273922"
---
# <a name="list-contracts"></a><span data-ttu-id="b86cb-103">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="b86cb-103">List contracts</span></span>

<span data-ttu-id="b86cb-104">Получение списка объектов [контракта](../resources/contract.md) , связанных с клиентом партнера.</span><span class="sxs-lookup"><span data-stu-id="b86cb-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b86cb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b86cb-105">Permissions</span></span>

<span data-ttu-id="b86cb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b86cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b86cb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b86cb-108">Permission type</span></span>      | <span data-ttu-id="b86cb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b86cb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b86cb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b86cb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b86cb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b86cb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b86cb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b86cb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b86cb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b86cb-113">Not supported.</span></span>    |
|<span data-ttu-id="b86cb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b86cb-114">Application</span></span> | <span data-ttu-id="b86cb-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b86cb-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b86cb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b86cb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b86cb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b86cb-117">Optional query parameters</span></span>

<span data-ttu-id="b86cb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b86cb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="b86cb-119">Фильтрация поддерживается для customerId, Дефаултдомаиннаме и displayName.</span><span class="sxs-lookup"><span data-stu-id="b86cb-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b86cb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b86cb-120">Request headers</span></span>

| <span data-ttu-id="b86cb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b86cb-121">Name</span></span>      |<span data-ttu-id="b86cb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b86cb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b86cb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b86cb-123">Authorization</span></span>  | <span data-ttu-id="b86cb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b86cb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b86cb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b86cb-126">Request body</span></span>

<span data-ttu-id="b86cb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b86cb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b86cb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="b86cb-128">Response</span></span>

<span data-ttu-id="b86cb-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Contract](../resources/contract.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b86cb-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b86cb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b86cb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b86cb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b86cb-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```

##### <a name="response"></a><span data-ttu-id="b86cb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b86cb-132">Response</span></span>

<span data-ttu-id="b86cb-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b86cb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b86cb-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="b86cb-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b86cb-136">C#</span><span class="sxs-lookup"><span data-stu-id="b86cb-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_contract-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b86cb-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b86cb-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_contract-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="b86cb-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b86cb-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_contract-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/contract-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/contract-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/contract-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
