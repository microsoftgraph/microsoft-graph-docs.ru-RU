---
title: Список контрактов
description: Извлечение списка объектов контракта, связанных с клиентом-партнером.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: da5c6e1d6e4b3bffc6be502eb901ed4ada1c1a9f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434722"
---
# <a name="list-contracts"></a><span data-ttu-id="4f51b-103">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="4f51b-103">List contracts</span></span>

<span data-ttu-id="4f51b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f51b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f51b-105">Извлечение списка объектов [контракта,](../resources/contract.md) связанных с клиентом-партнером.</span><span class="sxs-lookup"><span data-stu-id="4f51b-105">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f51b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4f51b-106">Permissions</span></span>

<span data-ttu-id="4f51b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f51b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4f51b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f51b-109">Permission type</span></span>      | <span data-ttu-id="4f51b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f51b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4f51b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f51b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4f51b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4f51b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4f51b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f51b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f51b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f51b-114">Not supported.</span></span>    |
|<span data-ttu-id="4f51b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f51b-115">Application</span></span> | <span data-ttu-id="4f51b-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f51b-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f51b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f51b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f51b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4f51b-118">Optional query parameters</span></span>

<span data-ttu-id="4f51b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4f51b-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> 

> <span data-ttu-id="4f51b-120">Фильтрация поддерживается для customerId, defaultDomainName и displayName.</span><span class="sxs-lookup"><span data-stu-id="4f51b-120">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f51b-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f51b-121">Request headers</span></span>

| <span data-ttu-id="4f51b-122">Имя</span><span class="sxs-lookup"><span data-stu-id="4f51b-122">Name</span></span>      |<span data-ttu-id="4f51b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="4f51b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4f51b-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4f51b-124">Authorization</span></span>  | <span data-ttu-id="4f51b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4f51b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f51b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4f51b-127">Request body</span></span>

<span data-ttu-id="4f51b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4f51b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f51b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f51b-129">Response</span></span>

<span data-ttu-id="4f51b-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [Contract](../resources/contract.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4f51b-130">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f51b-131">Пример</span><span class="sxs-lookup"><span data-stu-id="4f51b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4f51b-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f51b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4f51b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f51b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="c"></a>[<span data-ttu-id="4f51b-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f51b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f51b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f51b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f51b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f51b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f51b-137">Java</span><span class="sxs-lookup"><span data-stu-id="4f51b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4f51b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f51b-138">Response</span></span>

<span data-ttu-id="4f51b-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4f51b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
