---
title: Список контрактов
description: Извлечение списка объектов контракта, связанных с клиентом-партнером.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1df10b2adc9a2621c6caf9ee1dfbcc71bc8442a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035682"
---
# <a name="list-contracts"></a><span data-ttu-id="af8eb-103">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="af8eb-103">List contracts</span></span>

<span data-ttu-id="af8eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af8eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af8eb-105">Извлечение списка объектов [контракта,](../resources/contract.md) связанных с клиентом-партнером.</span><span class="sxs-lookup"><span data-stu-id="af8eb-105">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="af8eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="af8eb-106">Permissions</span></span>

<span data-ttu-id="af8eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af8eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="af8eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af8eb-109">Permission type</span></span>      | <span data-ttu-id="af8eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="af8eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="af8eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af8eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="af8eb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="af8eb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af8eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af8eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af8eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af8eb-114">Not supported.</span></span>    |
|<span data-ttu-id="af8eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af8eb-115">Application</span></span> | <span data-ttu-id="af8eb-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af8eb-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="af8eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af8eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="af8eb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="af8eb-118">Optional query parameters</span></span>

<span data-ttu-id="af8eb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="af8eb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> 

> <span data-ttu-id="af8eb-120">Фильтрация поддерживается для customerId, defaultDomainName и displayName.</span><span class="sxs-lookup"><span data-stu-id="af8eb-120">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="af8eb-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af8eb-121">Request headers</span></span>

| <span data-ttu-id="af8eb-122">Имя</span><span class="sxs-lookup"><span data-stu-id="af8eb-122">Name</span></span>      |<span data-ttu-id="af8eb-123">Описание</span><span class="sxs-lookup"><span data-stu-id="af8eb-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af8eb-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af8eb-124">Authorization</span></span>  | <span data-ttu-id="af8eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af8eb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af8eb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af8eb-127">Request body</span></span>

<span data-ttu-id="af8eb-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="af8eb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af8eb-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8eb-129">Response</span></span>

<span data-ttu-id="af8eb-130">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [Contract](../resources/contract.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="af8eb-130">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af8eb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="af8eb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af8eb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="af8eb-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="af8eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="af8eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="c"></a>[<span data-ttu-id="af8eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="af8eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="af8eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="af8eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="af8eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="af8eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="af8eb-137">Java</span><span class="sxs-lookup"><span data-stu-id="af8eb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af8eb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="af8eb-138">Response</span></span>

<span data-ttu-id="af8eb-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="af8eb-139">Note: The response object shown here might be shortened for readability.</span></span>
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
