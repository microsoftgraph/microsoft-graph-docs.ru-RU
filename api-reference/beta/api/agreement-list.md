---
title: Список соглашений
description: Получение списка объектов Agreement.
localization_priority: Normal
ms.openlocfilehash: d11c561dcd52970ab3143f93a0e3a7917969216d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439807"
---
# <a name="list-agreements"></a><span data-ttu-id="6fe2f-103">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="6fe2f-103">List agreements</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fe2f-104">Получение списка объектов [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="6fe2f-104">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="6fe2f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe2f-105">Permissions</span></span>
<span data-ttu-id="6fe2f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fe2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fe2f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6fe2f-108">Permission type</span></span>                        | <span data-ttu-id="6fe2f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6fe2f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6fe2f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6fe2f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fe2f-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="6fe2f-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="6fe2f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6fe2f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fe2f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-113">Not supported.</span></span> |
|<span data-ttu-id="6fe2f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6fe2f-114">Application</span></span>                            | <span data-ttu-id="6fe2f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fe2f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6fe2f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="6fe2f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6fe2f-117">Request headers</span></span>
| <span data-ttu-id="6fe2f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6fe2f-118">Name</span></span>         | <span data-ttu-id="6fe2f-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6fe2f-119">Type</span></span>        | <span data-ttu-id="6fe2f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6fe2f-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6fe2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fe2f-121">Authorization</span></span> | <span data-ttu-id="6fe2f-122">string</span><span class="sxs-lookup"><span data-stu-id="6fe2f-122">string</span></span> | <span data-ttu-id="6fe2f-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fe2f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6fe2f-125">Request body</span></span>
<span data-ttu-id="6fe2f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6fe2f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe2f-127">Response</span></span>
<span data-ttu-id="6fe2f-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-128">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6fe2f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6fe2f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6fe2f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6fe2f-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6fe2f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fe2f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6fe2f-132">C#</span><span class="sxs-lookup"><span data-stu-id="6fe2f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6fe2f-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6fe2f-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6fe2f-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6fe2f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6fe2f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6fe2f-135">Response</span></span>
><span data-ttu-id="6fe2f-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6fe2f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
