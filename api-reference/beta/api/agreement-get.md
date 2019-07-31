---
title: Получение соглашения
description: Получение свойств и связей объекта Agreement.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 21d090a3e1b23a1870fc86d418fd3edfc3ff69ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945701"
---
# <a name="get-agreement"></a><span data-ttu-id="d9f88-103">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="d9f88-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f88-104">Получение свойств и связей объекта [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="d9f88-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d9f88-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f88-105">Permissions</span></span>
<span data-ttu-id="d9f88-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9f88-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d9f88-108">Permission type</span></span>                        | <span data-ttu-id="d9f88-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d9f88-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9f88-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d9f88-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9f88-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9f88-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="d9f88-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d9f88-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f88-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f88-113">Not supported.</span></span> |
|<span data-ttu-id="d9f88-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d9f88-114">Application</span></span>                            | <span data-ttu-id="d9f88-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f88-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d9f88-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d9f88-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="d9f88-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d9f88-117">Request headers</span></span>
| <span data-ttu-id="d9f88-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d9f88-118">Name</span></span>         | <span data-ttu-id="d9f88-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d9f88-119">Type</span></span>        | <span data-ttu-id="d9f88-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d9f88-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d9f88-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9f88-121">Authorization</span></span> | <span data-ttu-id="d9f88-122">string</span><span class="sxs-lookup"><span data-stu-id="d9f88-122">string</span></span> | <span data-ttu-id="d9f88-p102">Носитель \{токен\}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d9f88-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d9f88-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d9f88-125">Request body</span></span>
<span data-ttu-id="d9f88-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d9f88-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d9f88-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f88-127">Response</span></span>
<span data-ttu-id="d9f88-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Agreement](../resources/agreement.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d9f88-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9f88-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d9f88-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9f88-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d9f88-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d9f88-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f88-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d9f88-132">C#</span><span class="sxs-lookup"><span data-stu-id="d9f88-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d9f88-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d9f88-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d9f88-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d9f88-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d9f88-135">Java</span><span class="sxs-lookup"><span data-stu-id="d9f88-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9f88-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d9f88-136">Response</span></span>
><span data-ttu-id="d9f88-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d9f88-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
