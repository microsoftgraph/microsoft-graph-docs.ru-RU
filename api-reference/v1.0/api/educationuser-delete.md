---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 862dc5dff342fa1b5510a830d09e8244380deaf4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015133"
---
# <a name="delete-educationuser"></a><span data-ttu-id="7fc22-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="7fc22-103">Delete educationUser</span></span>

<span data-ttu-id="7fc22-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fc22-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="7fc22-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc22-105">Permissions</span></span>
<span data-ttu-id="7fc22-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7fc22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7fc22-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7fc22-108">Permission type</span></span>      | <span data-ttu-id="7fc22-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7fc22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7fc22-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7fc22-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7fc22-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc22-111">Not supported.</span></span>  |
|<span data-ttu-id="7fc22-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7fc22-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7fc22-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7fc22-113">Not supported.</span></span>  |
|<span data-ttu-id="7fc22-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7fc22-114">Application</span></span> | <span data-ttu-id="7fc22-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fc22-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7fc22-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7fc22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7fc22-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7fc22-117">Request headers</span></span>
| <span data-ttu-id="7fc22-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7fc22-118">Header</span></span>       | <span data-ttu-id="7fc22-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7fc22-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7fc22-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7fc22-120">Authorization</span></span>  | <span data-ttu-id="7fc22-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7fc22-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fc22-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7fc22-123">Request body</span></span>
<span data-ttu-id="7fc22-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7fc22-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7fc22-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc22-125">Response</span></span>
<span data-ttu-id="7fc22-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7fc22-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7fc22-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7fc22-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7fc22-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7fc22-129">Request</span></span>
<span data-ttu-id="7fc22-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7fc22-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7fc22-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7fc22-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7fc22-132">C#</span><span class="sxs-lookup"><span data-stu-id="7fc22-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7fc22-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7fc22-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7fc22-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7fc22-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7fc22-135">Java</span><span class="sxs-lookup"><span data-stu-id="7fc22-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7fc22-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7fc22-136">Response</span></span>
<span data-ttu-id="7fc22-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7fc22-137">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
