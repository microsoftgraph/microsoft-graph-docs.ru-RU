---
title: Удаление educationCategory
description: Удаление существующей системы educationCategory из этого образованияAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 70bde8c8549486347542ff90f9088f1c78bde14a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992473"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="97a1d-103">Удаление educationCategory</span><span class="sxs-lookup"><span data-stu-id="97a1d-103">Remove educationCategory</span></span>

<span data-ttu-id="97a1d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97a1d-105">Удалите [educationCategory](../resources/educationcategory.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="97a1d-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="97a1d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="97a1d-106">Permissions</span></span>
<span data-ttu-id="97a1d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a1d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97a1d-109">Permission type</span></span>      | <span data-ttu-id="97a1d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97a1d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97a1d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97a1d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="97a1d-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97a1d-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="97a1d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97a1d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="97a1d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a1d-114">Not supported.</span></span>  |
|<span data-ttu-id="97a1d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="97a1d-115">Application</span></span> | <span data-ttu-id="97a1d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a1d-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="97a1d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97a1d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="97a1d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="97a1d-118">Request headers</span></span>
| <span data-ttu-id="97a1d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97a1d-119">Header</span></span>       | <span data-ttu-id="97a1d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="97a1d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="97a1d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="97a1d-121">Authorization</span></span>  | <span data-ttu-id="97a1d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a1d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="97a1d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97a1d-124">Content-Type</span></span>  | <span data-ttu-id="97a1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97a1d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97a1d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97a1d-126">Request body</span></span>
<span data-ttu-id="97a1d-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="97a1d-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97a1d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a1d-128">Response</span></span>
<span data-ttu-id="97a1d-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="97a1d-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="97a1d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="97a1d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97a1d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="97a1d-131">Request</span></span>
<span data-ttu-id="97a1d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97a1d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="97a1d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="97a1d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ec98f158-341d-4fea-9f8c-14a250d489ac"],
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```
# <a name="c"></a>[<span data-ttu-id="97a1d-134">C#</span><span class="sxs-lookup"><span data-stu-id="97a1d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-educationcategory-to-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97a1d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97a1d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-educationcategory-to-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97a1d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97a1d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-educationcategory-to-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97a1d-137">Java</span><span class="sxs-lookup"><span data-stu-id="97a1d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-educationcategory-to-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97a1d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a1d-138">Response</span></span>
<span data-ttu-id="97a1d-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="97a1d-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content

{
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


