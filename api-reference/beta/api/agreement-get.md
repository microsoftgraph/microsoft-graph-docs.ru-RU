---
title: Получение соглашения
description: Получение свойств и связей объекта Agreement.
localization_priority: Normal
ms.openlocfilehash: 587ec829881dea30118b6f8998acfd1ab87f9c44
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439821"
---
# <a name="get-agreement"></a><span data-ttu-id="d1b0c-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="d1b0c-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1b0c-104">Получение свойств и связей объекта [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="d1b0c-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1b0c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1b0c-105">Permissions</span></span>
<span data-ttu-id="d1b0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1b0c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1b0c-108">Permission type</span></span>                        | <span data-ttu-id="d1b0c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1b0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1b0c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1b0c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d1b0c-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1b0c-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="d1b0c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1b0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1b0c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-113">Not supported.</span></span> |
|<span data-ttu-id="d1b0c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1b0c-114">Application</span></span>                            | <span data-ttu-id="d1b0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1b0c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1b0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d1b0c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1b0c-117">Request headers</span></span>
| <span data-ttu-id="d1b0c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d1b0c-118">Name</span></span>         | <span data-ttu-id="d1b0c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d1b0c-119">Type</span></span>        | <span data-ttu-id="d1b0c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d1b0c-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d1b0c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1b0c-121">Authorization</span></span> | <span data-ttu-id="d1b0c-122">string</span><span class="sxs-lookup"><span data-stu-id="d1b0c-122">string</span></span> | <span data-ttu-id="d1b0c-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1b0c-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1b0c-125">Request body</span></span>
<span data-ttu-id="d1b0c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d1b0c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1b0c-127">Response</span></span>
<span data-ttu-id="d1b0c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d1b0c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d1b0c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1b0c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1b0c-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d1b0c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1b0c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d1b0c-132">C#</span><span class="sxs-lookup"><span data-stu-id="d1b0c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d1b0c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d1b0c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d1b0c-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d1b0c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d1b0c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1b0c-135">Response</span></span>
><span data-ttu-id="d1b0c-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1b0c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
