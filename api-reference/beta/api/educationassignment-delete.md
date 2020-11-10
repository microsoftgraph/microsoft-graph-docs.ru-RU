---
title: Удаление educationAssignment
description: Удаление существующего назначения. Удалять назначения могут только преподаватели внутри класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3e85d23fc4ef128a3c1231f51a8a037036b0a3d7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966609"
---
# <a name="delete-educationassignment"></a><span data-ttu-id="c9c36-104">Удаление educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c9c36-104">Delete educationAssignment</span></span>

<span data-ttu-id="c9c36-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9c36-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9c36-106">Удаление существующего назначения.</span><span class="sxs-lookup"><span data-stu-id="c9c36-106">Delete an existing assignment.</span></span> <span data-ttu-id="c9c36-107">Удалять назначения могут только преподаватели внутри класса.</span><span class="sxs-lookup"><span data-stu-id="c9c36-107">Only teachers within a class can delete assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="c9c36-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c36-108">Permissions</span></span>

<span data-ttu-id="c9c36-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9c36-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c9c36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9c36-111">Permission type</span></span>                        | <span data-ttu-id="c9c36-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9c36-112">Permissions (from least to most privileged)</span></span>             |
| :------------------------------------- | :------------------------------------------------------ |
| <span data-ttu-id="c9c36-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9c36-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c9c36-114">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9c36-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c9c36-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9c36-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9c36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c36-116">Not Supported.</span></span>                                          |
| <span data-ttu-id="c9c36-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c9c36-117">Application</span></span>                            | <span data-ttu-id="c9c36-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9c36-118">Not Supported.</span></span>                                          |

## <a name="http-request"></a><span data-ttu-id="c9c36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9c36-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c9c36-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9c36-120">Request headers</span></span>

| <span data-ttu-id="c9c36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9c36-121">Header</span></span>        | <span data-ttu-id="c9c36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c9c36-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c9c36-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9c36-123">Authorization</span></span> | <span data-ttu-id="c9c36-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9c36-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9c36-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9c36-126">Request body</span></span>

<span data-ttu-id="c9c36-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9c36-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9c36-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c36-128">Response</span></span>

<span data-ttu-id="c9c36-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c9c36-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9c36-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c9c36-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9c36-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9c36-132">Request</span></span>

<span data-ttu-id="c9c36-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9c36-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c9c36-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c9c36-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="c9c36-135">C#</span><span class="sxs-lookup"><span data-stu-id="c9c36-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c9c36-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c9c36-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c9c36-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c9c36-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c9c36-138">Java</span><span class="sxs-lookup"><span data-stu-id="c9c36-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c9c36-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9c36-139">Response</span></span>
<span data-ttu-id="c9c36-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c9c36-140">The following is an example of the response.</span></span> 


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
  "description": "Delete educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


