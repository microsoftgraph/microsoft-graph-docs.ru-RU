---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3b51cf44663aafeee54fa5cf2e8a6a6f80412a1e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965951"
---
# <a name="delete-educationschool"></a><span data-ttu-id="9081b-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="9081b-103">Delete educationSchool</span></span>

<span data-ttu-id="9081b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9081b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9081b-105">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="9081b-105">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9081b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9081b-106">Permissions</span></span>
<span data-ttu-id="9081b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9081b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9081b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9081b-109">Permission type</span></span>      | <span data-ttu-id="9081b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9081b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9081b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9081b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9081b-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9081b-112">Not supported.</span></span>  |
|<span data-ttu-id="9081b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9081b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9081b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9081b-114">Not supported.</span></span>  |
|<span data-ttu-id="9081b-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="9081b-115">Application</span></span> | <span data-ttu-id="9081b-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9081b-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9081b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9081b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9081b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9081b-118">Request headers</span></span>
| <span data-ttu-id="9081b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9081b-119">Header</span></span>       | <span data-ttu-id="9081b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9081b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9081b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9081b-121">Authorization</span></span>  | <span data-ttu-id="9081b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9081b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9081b-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9081b-124">Request body</span></span>
<span data-ttu-id="9081b-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9081b-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="9081b-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9081b-126">Response</span></span>
<span data-ttu-id="9081b-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9081b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9081b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9081b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9081b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9081b-130">Request</span></span>
<span data-ttu-id="9081b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9081b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9081b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9081b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="c"></a>[<span data-ttu-id="9081b-133">C#</span><span class="sxs-lookup"><span data-stu-id="9081b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9081b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9081b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9081b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9081b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9081b-136">Java</span><span class="sxs-lookup"><span data-stu-id="9081b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9081b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9081b-137">Response</span></span>
<span data-ttu-id="9081b-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9081b-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


