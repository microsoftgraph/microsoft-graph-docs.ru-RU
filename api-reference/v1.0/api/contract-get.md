---
title: Получение контракта
description: Получение свойств и связей объекта Contract.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e7ac5d4463d424fdcc31ca98cc3a729b95e5d53b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727140"
---
# <a name="get-contract"></a><span data-ttu-id="03a44-103">Получение контракта</span><span class="sxs-lookup"><span data-stu-id="03a44-103">Get Contract</span></span>

<span data-ttu-id="03a44-104">Получение свойств и связей объекта [Contract](../resources/contract.md) .</span><span class="sxs-lookup"><span data-stu-id="03a44-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03a44-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03a44-105">Permissions</span></span>

<span data-ttu-id="03a44-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03a44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="03a44-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03a44-108">Permission type</span></span>      | <span data-ttu-id="03a44-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03a44-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03a44-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03a44-110">Delegated (work or school account)</span></span> | <span data-ttu-id="03a44-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03a44-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03a44-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03a44-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03a44-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03a44-113">Not supported.</span></span>    |
|<span data-ttu-id="03a44-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03a44-114">Application</span></span> | <span data-ttu-id="03a44-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03a44-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="03a44-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03a44-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03a44-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03a44-117">Optional query parameters</span></span>

<span data-ttu-id="03a44-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03a44-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03a44-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03a44-119">Request headers</span></span>

| <span data-ttu-id="03a44-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03a44-120">Name</span></span>      |<span data-ttu-id="03a44-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03a44-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="03a44-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03a44-122">Authorization</span></span>  | <span data-ttu-id="03a44-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03a44-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="03a44-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03a44-125">Request body</span></span>

<span data-ttu-id="03a44-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03a44-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03a44-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="03a44-127">Response</span></span>

<span data-ttu-id="03a44-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [контракта](../resources/contract.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03a44-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03a44-129">Пример</span><span class="sxs-lookup"><span data-stu-id="03a44-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03a44-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="03a44-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="03a44-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="03a44-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="03a44-132">C#</span><span class="sxs-lookup"><span data-stu-id="03a44-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="03a44-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03a44-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="03a44-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="03a44-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="03a44-135">Java</span><span class="sxs-lookup"><span data-stu-id="03a44-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="03a44-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="03a44-136">Response</span></span>
<span data-ttu-id="03a44-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03a44-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
