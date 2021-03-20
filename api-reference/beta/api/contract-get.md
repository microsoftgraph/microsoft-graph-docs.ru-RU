---
title: Получить контракт
description: Извлечение свойств и связей объекта контракта.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f199dece53ce5082a775787c24af88e4ced474f3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946954"
---
# <a name="get-contract"></a><span data-ttu-id="d2156-103">Получить контракт</span><span class="sxs-lookup"><span data-stu-id="d2156-103">Get Contract</span></span>

<span data-ttu-id="d2156-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2156-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2156-105">Извлечение свойств и связей объекта [контракта.](../resources/contract.md)</span><span class="sxs-lookup"><span data-stu-id="d2156-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2156-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d2156-106">Permissions</span></span>

<span data-ttu-id="d2156-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2156-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d2156-109">Permission type</span></span>      | <span data-ttu-id="d2156-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d2156-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2156-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d2156-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d2156-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d2156-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d2156-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d2156-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2156-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2156-114">Not supported.</span></span>    |
|<span data-ttu-id="d2156-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d2156-115">Application</span></span> | <span data-ttu-id="d2156-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2156-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2156-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d2156-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2156-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d2156-118">Optional query parameters</span></span>

<span data-ttu-id="d2156-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d2156-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2156-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d2156-120">Request headers</span></span>

| <span data-ttu-id="d2156-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d2156-121">Name</span></span>      |<span data-ttu-id="d2156-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d2156-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2156-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d2156-123">Authorization</span></span>  | <span data-ttu-id="d2156-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d2156-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2156-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d2156-126">Request body</span></span>

<span data-ttu-id="d2156-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d2156-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2156-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2156-128">Response</span></span>

<span data-ttu-id="d2156-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект Contract](../resources/contract.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d2156-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2156-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d2156-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2156-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d2156-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d2156-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d2156-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="d2156-133">C#</span><span class="sxs-lookup"><span data-stu-id="d2156-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d2156-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d2156-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d2156-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d2156-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d2156-136">Java</span><span class="sxs-lookup"><span data-stu-id="d2156-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d2156-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d2156-137">Response</span></span>
<span data-ttu-id="d2156-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d2156-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
