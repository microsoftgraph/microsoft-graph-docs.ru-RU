---
title: Удаление Едукатионрубрик из educationAssignment
description: Удаление Едукатионрубрик из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 19b35c7684e3b1886d5479ed9e3d9011683bf06e
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461217"
---
# <a name="remove-educationrubric-from-educationassignment"></a><span data-ttu-id="04170-103">Удаление Едукатионрубрик из educationAssignment</span><span class="sxs-lookup"><span data-stu-id="04170-103">Remove educationRubric from educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04170-104">Удаление [едукатионрубрик](../resources/educationrubric.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04170-104">Remove an [educationRubric](../resources/educationrubric.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>  <span data-ttu-id="04170-105">При этом сам Rubric не удаляется.</span><span class="sxs-lookup"><span data-stu-id="04170-105">This does not delete the rubric itself.</span></span>

## <a name="permissions"></a><span data-ttu-id="04170-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04170-106">Permissions</span></span>

<span data-ttu-id="04170-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04170-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04170-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04170-109">Permission type</span></span>                        | <span data-ttu-id="04170-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04170-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04170-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04170-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04170-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04170-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="04170-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04170-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04170-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04170-114">Not supported.</span></span> |
| <span data-ttu-id="04170-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04170-115">Application</span></span>                            | <span data-ttu-id="04170-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04170-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04170-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04170-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/assignments/{id}/rubric/$ref
```

## <a name="request-headers"></a><span data-ttu-id="04170-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04170-118">Request headers</span></span>

| <span data-ttu-id="04170-119">Имя</span><span class="sxs-lookup"><span data-stu-id="04170-119">Name</span></span>          | <span data-ttu-id="04170-120">Описание</span><span class="sxs-lookup"><span data-stu-id="04170-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04170-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04170-121">Authorization</span></span> | <span data-ttu-id="04170-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="04170-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="04170-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04170-123">Request body</span></span>

<span data-ttu-id="04170-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04170-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04170-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="04170-125">Response</span></span>

<span data-ttu-id="04170-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="04170-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04170-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="04170-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04170-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="04170-129">Request</span></span>

<span data-ttu-id="04170-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04170-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04170-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="04170-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric_from_educationassignment"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/me/assignments/{id}/rubric/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04170-132">C#</span><span class="sxs-lookup"><span data-stu-id="04170-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04170-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04170-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04170-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="04170-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04170-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="04170-135">Response</span></span>

<span data-ttu-id="04170-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04170-136">The following is an example of the response.</span></span>

> <span data-ttu-id="04170-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04170-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
