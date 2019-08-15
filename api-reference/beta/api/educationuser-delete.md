---
title: Удаление educationUser
description: Удаление пользователя.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: df0dd3a99a6f158ce7de20767df6b10dae137ded
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415913"
---
# <a name="delete-educationuser"></a><span data-ttu-id="7bc07-103">Удаление educationUser</span><span class="sxs-lookup"><span data-stu-id="7bc07-103">Delete educationUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bc07-104">Удаление пользователя.</span><span class="sxs-lookup"><span data-stu-id="7bc07-104">Delete a user.</span></span>


## <a name="permissions"></a><span data-ttu-id="7bc07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc07-105">Permissions</span></span>
<span data-ttu-id="7bc07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7bc07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7bc07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7bc07-108">Permission type</span></span>      | <span data-ttu-id="7bc07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7bc07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7bc07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7bc07-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7bc07-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc07-111">Not supported.</span></span>  |
|<span data-ttu-id="7bc07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7bc07-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7bc07-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bc07-113">Not supported.</span></span>  |
|<span data-ttu-id="7bc07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7bc07-114">Application</span></span> | <span data-ttu-id="7bc07-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7bc07-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7bc07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7bc07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="7bc07-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7bc07-117">Request headers</span></span>
| <span data-ttu-id="7bc07-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7bc07-118">Header</span></span>       | <span data-ttu-id="7bc07-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7bc07-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7bc07-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7bc07-120">Authorization</span></span>  | <span data-ttu-id="7bc07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7bc07-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7bc07-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7bc07-123">Request body</span></span>
<span data-ttu-id="7bc07-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7bc07-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7bc07-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc07-125">Response</span></span>
<span data-ttu-id="7bc07-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7bc07-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7bc07-128">Пример</span><span class="sxs-lookup"><span data-stu-id="7bc07-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7bc07-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="7bc07-129">Request</span></span>
<span data-ttu-id="7bc07-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7bc07-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7bc07-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="7bc07-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationuser"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/users/13019
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7bc07-132">C#</span><span class="sxs-lookup"><span data-stu-id="7bc07-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7bc07-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7bc07-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7bc07-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7bc07-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7bc07-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7bc07-135">Response</span></span>
<span data-ttu-id="7bc07-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7bc07-136">The following is an example of the response.</span></span> 
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
