---
title: Список соглашений
description: Получение списка объектов Agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 46f4aa8f7cdc5ef7c650166be079da8cc0b0bb2d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962465"
---
# <a name="list-agreements"></a><span data-ttu-id="5391c-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="5391c-103">List agreements</span></span>

<span data-ttu-id="5391c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5391c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5391c-105">Получение списка объектов [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="5391c-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5391c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5391c-106">Permissions</span></span>
<span data-ttu-id="5391c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5391c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5391c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5391c-109">Permission type</span></span>                        | <span data-ttu-id="5391c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5391c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5391c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5391c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5391c-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="5391c-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="5391c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5391c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5391c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5391c-114">Not supported.</span></span> |
|<span data-ttu-id="5391c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5391c-115">Application</span></span>                            | <span data-ttu-id="5391c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5391c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5391c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5391c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="5391c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5391c-118">Request headers</span></span>
| <span data-ttu-id="5391c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="5391c-119">Name</span></span>         | <span data-ttu-id="5391c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="5391c-120">Type</span></span>        | <span data-ttu-id="5391c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="5391c-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="5391c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5391c-122">Authorization</span></span> | <span data-ttu-id="5391c-123">string</span><span class="sxs-lookup"><span data-stu-id="5391c-123">string</span></span> | <span data-ttu-id="5391c-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5391c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5391c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5391c-126">Request body</span></span>
<span data-ttu-id="5391c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5391c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5391c-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="5391c-128">Response</span></span>
<span data-ttu-id="5391c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5391c-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5391c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5391c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5391c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5391c-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5391c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5391c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/agreements
```
# <a name="c"></a>[<span data-ttu-id="5391c-133">C#</span><span class="sxs-lookup"><span data-stu-id="5391c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5391c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5391c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5391c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5391c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5391c-136">Java</span><span class="sxs-lookup"><span data-stu-id="5391c-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5391c-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="5391c-137">Response</span></span>
><span data-ttu-id="5391c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5391c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
