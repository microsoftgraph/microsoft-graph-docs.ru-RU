---
title: Удаление Едукатионкатегори
description: Удаление существующей категории.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0e5e88d13af85b109e139f68866ab1959a729d19
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860696"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="85def-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="85def-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85def-104">Удаление существующей категории.</span><span class="sxs-lookup"><span data-stu-id="85def-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="85def-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85def-105">Permissions</span></span>

<span data-ttu-id="85def-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85def-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85def-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85def-108">Permission type</span></span>                        | <span data-ttu-id="85def-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85def-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="85def-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85def-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85def-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85def-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="85def-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85def-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85def-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85def-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="85def-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85def-114">Application</span></span>                            | <span data-ttu-id="85def-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85def-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="85def-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85def-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="85def-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85def-117">Request headers</span></span>

| <span data-ttu-id="85def-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85def-118">Header</span></span>        | <span data-ttu-id="85def-119">Значение</span><span class="sxs-lookup"><span data-stu-id="85def-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="85def-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85def-120">Authorization</span></span> | <span data-ttu-id="85def-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85def-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85def-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85def-123">Request body</span></span>

<span data-ttu-id="85def-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85def-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85def-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="85def-125">Response</span></span>

<span data-ttu-id="85def-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85def-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85def-128">Пример</span><span class="sxs-lookup"><span data-stu-id="85def-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="85def-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="85def-129">Request</span></span>

<span data-ttu-id="85def-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85def-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="85def-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="85def-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="85def-132">C#</span><span class="sxs-lookup"><span data-stu-id="85def-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="85def-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="85def-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="85def-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="85def-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="85def-135">Java</span><span class="sxs-lookup"><span data-stu-id="85def-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85def-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="85def-136">Response</span></span>

<span data-ttu-id="85def-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="85def-137">The following is an example of the response.</span></span> 

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
  "description": "Delete educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
