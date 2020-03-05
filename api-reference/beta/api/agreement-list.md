---
title: Список соглашений
description: Получение списка объектов Agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4b8aea71f60607f8f0a82080c0cec3c493cfeedd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441664"
---
# <a name="list-agreements"></a><span data-ttu-id="c305d-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="c305d-103">List agreements</span></span>

<span data-ttu-id="c305d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c305d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c305d-105">Получение списка объектов [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="c305d-105">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c305d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c305d-106">Permissions</span></span>
<span data-ttu-id="c305d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c305d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c305d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c305d-109">Permission type</span></span>                        | <span data-ttu-id="c305d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c305d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c305d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c305d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c305d-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="c305d-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="c305d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c305d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c305d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c305d-114">Not supported.</span></span> |
|<span data-ttu-id="c305d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c305d-115">Application</span></span>                            | <span data-ttu-id="c305d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c305d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c305d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c305d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="c305d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c305d-118">Request headers</span></span>
| <span data-ttu-id="c305d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c305d-119">Name</span></span>         | <span data-ttu-id="c305d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c305d-120">Type</span></span>        | <span data-ttu-id="c305d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c305d-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c305d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c305d-122">Authorization</span></span> | <span data-ttu-id="c305d-123">string</span><span class="sxs-lookup"><span data-stu-id="c305d-123">string</span></span> | <span data-ttu-id="c305d-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c305d-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c305d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c305d-126">Request body</span></span>
<span data-ttu-id="c305d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c305d-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c305d-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="c305d-128">Response</span></span>
<span data-ttu-id="c305d-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c305d-129">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c305d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c305d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c305d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c305d-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c305d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c305d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/agreements
```
# <a name="c"></a>[<span data-ttu-id="c305d-133">C#</span><span class="sxs-lookup"><span data-stu-id="c305d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c305d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c305d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c305d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c305d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c305d-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c305d-136">Response</span></span>
><span data-ttu-id="c305d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c305d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
