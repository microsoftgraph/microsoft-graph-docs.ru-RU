---
title: Удаление Едукатионкатегори
description: Удаление существующей категории.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6bd82f9e901ede49ab2581c7e3be444075e2f6bd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955539"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="8065e-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="8065e-103">Delete educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8065e-104">Удаление существующей категории.</span><span class="sxs-lookup"><span data-stu-id="8065e-104">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="8065e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8065e-105">Permissions</span></span>

<span data-ttu-id="8065e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8065e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8065e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8065e-108">Permission type</span></span>                        | <span data-ttu-id="8065e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8065e-109">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="8065e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8065e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8065e-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8065e-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8065e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8065e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8065e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8065e-113">Not Supported.</span></span>                                          |
| <span data-ttu-id="8065e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8065e-114">Application</span></span>                            | <span data-ttu-id="8065e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8065e-115">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="8065e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8065e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8065e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8065e-117">Request headers</span></span>

| <span data-ttu-id="8065e-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8065e-118">Header</span></span>        | <span data-ttu-id="8065e-119">Значение</span><span class="sxs-lookup"><span data-stu-id="8065e-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8065e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8065e-120">Authorization</span></span> | <span data-ttu-id="8065e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8065e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8065e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8065e-123">Request body</span></span>

<span data-ttu-id="8065e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8065e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8065e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8065e-125">Response</span></span>

<span data-ttu-id="8065e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8065e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8065e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8065e-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8065e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8065e-129">Request</span></span>

<span data-ttu-id="8065e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8065e-130">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8065e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8065e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8065e-132">C#</span><span class="sxs-lookup"><span data-stu-id="8065e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8065e-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="8065e-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8065e-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8065e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8065e-135">Java</span><span class="sxs-lookup"><span data-stu-id="8065e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8065e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8065e-136">Response</span></span>

<span data-ttu-id="8065e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8065e-137">The following is an example of the response.</span></span> 

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
