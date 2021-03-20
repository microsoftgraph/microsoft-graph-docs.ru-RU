---
title: Удаление educationCategory
description: Удаление существующей категории.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4bf5777ee48f4701a3a0ae29f1da9b9f9ab26269
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951708"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="1789e-103">Удаление educationCategory</span><span class="sxs-lookup"><span data-stu-id="1789e-103">Delete educationCategory</span></span>

<span data-ttu-id="1789e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1789e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1789e-105">Удаление существующей категории.</span><span class="sxs-lookup"><span data-stu-id="1789e-105">Delete an existing category.</span></span>

## <a name="permissions"></a><span data-ttu-id="1789e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1789e-106">Permissions</span></span>

<span data-ttu-id="1789e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1789e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1789e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1789e-109">Permission type</span></span>                        | <span data-ttu-id="1789e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1789e-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="1789e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1789e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1789e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1789e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1789e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1789e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1789e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1789e-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="1789e-115">Application</span><span class="sxs-lookup"><span data-stu-id="1789e-115">Application</span></span>                            | <span data-ttu-id="1789e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1789e-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="1789e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1789e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1789e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1789e-118">Request headers</span></span>

| <span data-ttu-id="1789e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1789e-119">Header</span></span>        | <span data-ttu-id="1789e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1789e-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1789e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1789e-121">Authorization</span></span> | <span data-ttu-id="1789e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1789e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1789e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1789e-124">Request body</span></span>

<span data-ttu-id="1789e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1789e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1789e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1789e-126">Response</span></span>

<span data-ttu-id="1789e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1789e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1789e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1789e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1789e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1789e-130">Request</span></span>

<span data-ttu-id="1789e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1789e-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1789e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1789e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignmentCategories/19002
```
# <a name="c"></a>[<span data-ttu-id="1789e-133">C#</span><span class="sxs-lookup"><span data-stu-id="1789e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1789e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1789e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1789e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1789e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1789e-136">Java</span><span class="sxs-lookup"><span data-stu-id="1789e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1789e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1789e-137">Response</span></span>

<span data-ttu-id="1789e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1789e-138">The following is an example of the response.</span></span> 

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


