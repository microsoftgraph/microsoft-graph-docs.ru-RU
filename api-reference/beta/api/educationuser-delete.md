---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11d79b905b687f94e3cd5e7fc089cba90b18ac0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323822"
---
# <a name="delete-educationuser"></a><span data-ttu-id="30bd5-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="30bd5-103">Delete educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30bd5-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="30bd5-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="30bd5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="30bd5-105">Permissions</span></span>
<span data-ttu-id="30bd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30bd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30bd5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30bd5-108">Permission type</span></span>      | <span data-ttu-id="30bd5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="30bd5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30bd5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30bd5-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="30bd5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bd5-111">Not supported.</span></span>  |
|<span data-ttu-id="30bd5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30bd5-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="30bd5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bd5-113">Not supported.</span></span>  |
|<span data-ttu-id="30bd5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30bd5-114">Application</span></span> | <span data-ttu-id="30bd5-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30bd5-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="30bd5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30bd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="30bd5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30bd5-117">Request headers</span></span>
| <span data-ttu-id="30bd5-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30bd5-118">Header</span></span>       | <span data-ttu-id="30bd5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="30bd5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="30bd5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30bd5-120">Authorization</span></span>  | <span data-ttu-id="30bd5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="30bd5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30bd5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30bd5-123">Request body</span></span>
<span data-ttu-id="30bd5-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="30bd5-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="30bd5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="30bd5-125">Response</span></span>
<span data-ttu-id="30bd5-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="30bd5-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30bd5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="30bd5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30bd5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="30bd5-129">Request</span></span>
<span data-ttu-id="30bd5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30bd5-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="30bd5-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="30bd5-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="30bd5-132">C#</span><span class="sxs-lookup"><span data-stu-id="30bd5-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="30bd5-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30bd5-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="30bd5-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="30bd5-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="30bd5-135">Java</span><span class="sxs-lookup"><span data-stu-id="30bd5-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="30bd5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="30bd5-136">Response</span></span>
<span data-ttu-id="30bd5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="30bd5-137">The following is an example of the response.</span></span> 
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
  "description": "Delete educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
