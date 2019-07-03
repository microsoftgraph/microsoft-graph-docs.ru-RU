---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b7c3bfe0d2a99fe7fe72e6d6303e66d81191650a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445200"
---
# <a name="delete-educationschool"></a><span data-ttu-id="1dddb-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="1dddb-103">Delete educationSchool</span></span>

<span data-ttu-id="1dddb-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="1dddb-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dddb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1dddb-105">Permissions</span></span>
<span data-ttu-id="1dddb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dddb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dddb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1dddb-108">Permission type</span></span>      | <span data-ttu-id="1dddb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1dddb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dddb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1dddb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="1dddb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dddb-111">Not supported.</span></span>  |
|<span data-ttu-id="1dddb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dddb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1dddb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dddb-113">Not supported.</span></span>  |
|<span data-ttu-id="1dddb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1dddb-114">Application</span></span> | <span data-ttu-id="1dddb-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dddb-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1dddb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1dddb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1dddb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1dddb-117">Request headers</span></span>
| <span data-ttu-id="1dddb-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1dddb-118">Header</span></span>       | <span data-ttu-id="1dddb-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1dddb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1dddb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1dddb-120">Authorization</span></span>  | <span data-ttu-id="1dddb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1dddb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1dddb-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1dddb-123">Request body</span></span>
<span data-ttu-id="1dddb-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1dddb-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="1dddb-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dddb-125">Response</span></span>
<span data-ttu-id="1dddb-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1dddb-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dddb-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1dddb-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dddb-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1dddb-129">Request</span></span>
<span data-ttu-id="1dddb-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1dddb-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1dddb-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dddb-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1dddb-132">C#</span><span class="sxs-lookup"><span data-stu-id="1dddb-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1dddb-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="1dddb-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1dddb-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="1dddb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1dddb-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1dddb-135">Response</span></span>
<span data-ttu-id="1dddb-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1dddb-136">The following is an example of the response.</span></span> 

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
