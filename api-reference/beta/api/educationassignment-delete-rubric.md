---
title: Удаление educationRubric из educationAssignment
description: Удаление образовательногоRubric из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8fdf11ab9792609813a92aef1c42f79b0cba3b48
ms.sourcegitcommit: 40a8e4b9e344811267025e23c372a6e60e31a1b9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/01/2021
ms.locfileid: "52119014"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="1c941-103">Удаление educationRubric из educationAssignment</span><span class="sxs-lookup"><span data-stu-id="1c941-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="1c941-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c941-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c941-105">Удаление [educationRubric](../resources/educationrubric.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1c941-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="1c941-106">Это не удаляет сам рубрику.</span><span class="sxs-lookup"><span data-stu-id="1c941-106">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c941-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c941-107">Permissions</span></span>

<span data-ttu-id="1c941-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c941-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c941-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c941-110">Permission type</span></span>                        | <span data-ttu-id="1c941-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c941-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c941-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c941-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c941-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c941-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1c941-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c941-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c941-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c941-115">Not supported.</span></span> |
| <span data-ttu-id="1c941-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c941-116">Application</span></span>                            | <span data-ttu-id="1c941-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c941-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c941-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c941-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="1c941-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c941-119">Request headers</span></span>

| <span data-ttu-id="1c941-120">Имя</span><span class="sxs-lookup"><span data-stu-id="1c941-120">Name</span></span>          | <span data-ttu-id="1c941-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1c941-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1c941-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c941-122">Authorization</span></span> | <span data-ttu-id="1c941-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1c941-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c941-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c941-124">Request body</span></span>

<span data-ttu-id="1c941-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c941-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c941-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c941-126">Response</span></span>

<span data-ttu-id="1c941-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1c941-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c941-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c941-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c941-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c941-130">Request</span></span>

<span data-ttu-id="1c941-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c941-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c941-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c941-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="1c941-133">C#</span><span class="sxs-lookup"><span data-stu-id="1c941-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c941-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c941-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c941-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c941-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1c941-136">Java</span><span class="sxs-lookup"><span data-stu-id="1c941-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c941-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c941-137">Response</span></span>

<span data-ttu-id="1c941-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1c941-138">The following is an example of the response.</span></span>

> <span data-ttu-id="1c941-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1c941-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


