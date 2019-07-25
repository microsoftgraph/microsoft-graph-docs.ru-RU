---
title: Удаление educationClass
description: Удаление класса. Так как класс также является универсальной группой, удаление класса приводит к удалению группы.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: cb901c2cee42203292a417d35fdb038264c1c29c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888413"
---
# <a name="delete-educationclass"></a><span data-ttu-id="99270-104">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="99270-104">Delete educationClass</span></span>

<span data-ttu-id="99270-105">Удаление класса.</span><span class="sxs-lookup"><span data-stu-id="99270-105">Delete a class.</span></span> <span data-ttu-id="99270-106">Так как класс также является универсальной группой, удаление класса приводит к удалению группы.</span><span class="sxs-lookup"><span data-stu-id="99270-106">Because a class is also a universal group, deleting a class deletes the group.</span></span>

## <a name="permissions"></a><span data-ttu-id="99270-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99270-107">Permissions</span></span>
<span data-ttu-id="99270-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99270-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99270-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99270-110">Permission type</span></span>      | <span data-ttu-id="99270-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99270-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99270-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99270-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="99270-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99270-113">Not supported.</span></span>  |
|<span data-ttu-id="99270-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99270-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="99270-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99270-115">Not supported.</span></span>  |
|<span data-ttu-id="99270-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99270-116">Application</span></span> | <span data-ttu-id="99270-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99270-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="99270-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99270-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}

```
## <a name="request-headers"></a><span data-ttu-id="99270-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99270-119">Request headers</span></span>
| <span data-ttu-id="99270-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99270-120">Header</span></span>       | <span data-ttu-id="99270-121">Значение</span><span class="sxs-lookup"><span data-stu-id="99270-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99270-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99270-122">Authorization</span></span>  | <span data-ttu-id="99270-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99270-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99270-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99270-125">Request body</span></span>
<span data-ttu-id="99270-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99270-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="99270-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="99270-127">Response</span></span>
<span data-ttu-id="99270-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="99270-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99270-130">Пример</span><span class="sxs-lookup"><span data-stu-id="99270-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="99270-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="99270-131">Request</span></span>
<span data-ttu-id="99270-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99270-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99270-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="99270-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationclass"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99270-134">C#</span><span class="sxs-lookup"><span data-stu-id="99270-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99270-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="99270-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99270-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="99270-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="99270-137">Java</span><span class="sxs-lookup"><span data-stu-id="99270-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99270-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="99270-138">Response</span></span>
<span data-ttu-id="99270-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99270-139">The following is an example of the response.</span></span> 

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
  "description": "Delete educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
