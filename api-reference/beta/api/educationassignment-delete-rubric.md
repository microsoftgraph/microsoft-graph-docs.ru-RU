---
title: Удаление Едукатионрубрик из educationAssignment
description: Удаление Едукатионрубрик из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8fb3bb1c18a3373c17ecc8c19533c5db32a8e632
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427804"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="c2326-103">Удаление Едукатионрубрик из educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c2326-103">Remove educationRubric from educationAssignment</span></span>

<span data-ttu-id="c2326-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2326-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2326-105">Удаление [едукатионрубрик](../resources/educationrubric.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c2326-105">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="c2326-106">При этом сам Rubric не удаляется.</span><span class="sxs-lookup"><span data-stu-id="c2326-106">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2326-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2326-107">Permissions</span></span>

<span data-ttu-id="c2326-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2326-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2326-110">Permission type</span></span>                        | <span data-ttu-id="c2326-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2326-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c2326-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2326-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2326-113">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c2326-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c2326-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2326-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2326-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2326-115">Not supported.</span></span> |
| <span data-ttu-id="c2326-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2326-116">Application</span></span>                            | <span data-ttu-id="c2326-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2326-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2326-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2326-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c2326-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2326-119">Request headers</span></span>

| <span data-ttu-id="c2326-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c2326-120">Name</span></span>          | <span data-ttu-id="c2326-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c2326-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2326-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2326-122">Authorization</span></span> | <span data-ttu-id="c2326-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c2326-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2326-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2326-124">Request body</span></span>

<span data-ttu-id="c2326-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2326-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2326-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2326-126">Response</span></span>

<span data-ttu-id="c2326-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2326-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2326-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2326-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2326-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2326-130">Request</span></span>

<span data-ttu-id="c2326-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2326-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2326-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2326-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="c"></a>[<span data-ttu-id="c2326-133">C#</span><span class="sxs-lookup"><span data-stu-id="c2326-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2326-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2326-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2326-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2326-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2326-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2326-136">Response</span></span>

<span data-ttu-id="c2326-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2326-137">The following is an example of the response.</span></span>

> <span data-ttu-id="c2326-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2326-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
