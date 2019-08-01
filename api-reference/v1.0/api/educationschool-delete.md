---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 37da6e8ca625a92cb81db086003218ecc3680b83
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002897"
---
# <a name="delete-educationschool"></a><span data-ttu-id="3be5b-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="3be5b-103">Delete educationSchool</span></span>

<span data-ttu-id="3be5b-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="3be5b-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="3be5b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3be5b-105">Permissions</span></span>
<span data-ttu-id="3be5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3be5b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3be5b-108">Permission type</span></span>      | <span data-ttu-id="3be5b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3be5b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3be5b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3be5b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3be5b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be5b-111">Not supported.</span></span>  |
|<span data-ttu-id="3be5b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3be5b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="3be5b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3be5b-113">Not supported.</span></span>  |
|<span data-ttu-id="3be5b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3be5b-114">Application</span></span> | <span data-ttu-id="3be5b-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be5b-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="3be5b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3be5b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3be5b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3be5b-117">Request headers</span></span>
| <span data-ttu-id="3be5b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3be5b-118">Header</span></span>       | <span data-ttu-id="3be5b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3be5b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3be5b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3be5b-120">Authorization</span></span>  | <span data-ttu-id="3be5b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3be5b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3be5b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3be5b-123">Request body</span></span>
<span data-ttu-id="3be5b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3be5b-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3be5b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be5b-125">Response</span></span>
<span data-ttu-id="3be5b-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3be5b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be5b-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3be5b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3be5b-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3be5b-129">Request</span></span>
<span data-ttu-id="3be5b-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3be5b-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3be5b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3be5b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3be5b-132">C#</span><span class="sxs-lookup"><span data-stu-id="3be5b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3be5b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="3be5b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3be5b-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3be5b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3be5b-135">Java</span><span class="sxs-lookup"><span data-stu-id="3be5b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3be5b-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3be5b-136">Response</span></span>
<span data-ttu-id="3be5b-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3be5b-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
