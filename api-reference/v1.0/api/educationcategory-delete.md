---
title: Удаление educationCategory
description: Удаление существующей категории.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ba6a68358f91e2f965bb5fe8a39145ee20295d93
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992874"
---
# <a name="delete-educationcategory"></a><span data-ttu-id="28d2e-103">Удаление educationCategory</span><span class="sxs-lookup"><span data-stu-id="28d2e-103">Delete educationCategory</span></span>

<span data-ttu-id="28d2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28d2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="28d2e-105">Удаление существующей [категории](../resources/educationcategory.md).</span><span class="sxs-lookup"><span data-stu-id="28d2e-105">Delete an existing [category](../resources/educationcategory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="28d2e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28d2e-106">Permissions</span></span>

<span data-ttu-id="28d2e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="28d2e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28d2e-109">Permission type</span></span>                        | <span data-ttu-id="28d2e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28d2e-110">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="28d2e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28d2e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="28d2e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28d2e-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="28d2e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28d2e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28d2e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d2e-114">Not Supported.</span></span>                                          |
| <span data-ttu-id="28d2e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="28d2e-115">Application</span></span>                            | <span data-ttu-id="28d2e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d2e-116">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="28d2e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28d2e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="28d2e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28d2e-118">Request headers</span></span>

| <span data-ttu-id="28d2e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28d2e-119">Header</span></span>        | <span data-ttu-id="28d2e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="28d2e-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="28d2e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28d2e-121">Authorization</span></span> | <span data-ttu-id="28d2e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28d2e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28d2e-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="28d2e-124">Request body</span></span>

<span data-ttu-id="28d2e-125">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28d2e-125">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d2e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d2e-126">Response</span></span>

<span data-ttu-id="28d2e-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28d2e-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d2e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="28d2e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="28d2e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="28d2e-130">Request</span></span>

<span data-ttu-id="28d2e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28d2e-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="28d2e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="28d2e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment_2"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/c42f493f-42b4-4e7d-8148-af894cbc518b/assignmentCategories/b93d3b6b-360c-45c0-8764-e8bb622a9504
```
# <a name="c"></a>[<span data-ttu-id="28d2e-133">C#</span><span class="sxs-lookup"><span data-stu-id="28d2e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28d2e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28d2e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28d2e-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28d2e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28d2e-136">Java</span><span class="sxs-lookup"><span data-stu-id="28d2e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="28d2e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d2e-137">Response</span></span>

<span data-ttu-id="28d2e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="28d2e-138">The following is an example of the response.</span></span> 

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


