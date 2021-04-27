---
title: Обновление educationRubric
description: Обновление свойств объекта educationRubric.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e0bcea6b95b83cad3f4467e0a3687a3e2c401b56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043481"
---
# <a name="update-educationrubric"></a><span data-ttu-id="a5a4f-103">Обновление educationRubric</span><span class="sxs-lookup"><span data-stu-id="a5a4f-103">Update educationRubric</span></span>

<span data-ttu-id="a5a4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5a4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5a4f-105">Обновление свойств объекта [educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="a5a4f-105">Update the properties of an [educationRubric](../resources/educationrubric.md) object.</span></span>

<span data-ttu-id="a5a4f-106">Обновление рубрики, присоединенной к назначению ( ) возможно только до публикации назначения, и обновление фактически является исходной рубрикой, которая существует `PATCH /education/me/assignments/{id}/rubric` под `/education/users/{id}/rubrics` .</span><span class="sxs-lookup"><span data-stu-id="a5a4f-106">Updating a rubric attached to an assignment (`PATCH /education/me/assignments/{id}/rubric`) is only possible before the assignment is published, and what is updated is actually the original rubric that exists under `/education/users/{id}/rubrics`.</span></span> <span data-ttu-id="a5a4f-107">После публикации назначения будет выполнена неопубликоваемая копия рубрики, прикрепленная к этому конкретному назначению.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-107">After the assignment is published, an immutable copy of the rubric is made that is attached to that specific assignment.</span></span> <span data-ttu-id="a5a4f-108">Эту рубрику можно получить с помощью [GET/education/me/assignments/{id}/rubric,](educationrubric-get.md)но ее нельзя обновить.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-108">That rubric can be retrieved using [GET /education/me/assignments/{id}/rubric](educationrubric-get.md), but it cannot be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5a4f-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a4f-109">Permissions</span></span>

<span data-ttu-id="a5a4f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5a4f-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a4f-112">Permission type</span></span>                        | <span data-ttu-id="a5a4f-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a4f-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5a4f-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a4f-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5a4f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a5a4f-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="a5a4f-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a4f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5a4f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-117">Not supported.</span></span> |
| <span data-ttu-id="a5a4f-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a5a4f-118">Application</span></span>                            | <span data-ttu-id="a5a4f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5a4f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a4f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me/rubrics/{id}
PATCH /education/me/assignments/{id}/rubric
```

## <a name="request-headers"></a><span data-ttu-id="a5a4f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a4f-121">Request headers</span></span>

| <span data-ttu-id="a5a4f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="a5a4f-122">Name</span></span>       | <span data-ttu-id="a5a4f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a4f-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5a4f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5a4f-124">Authorization</span></span> | <span data-ttu-id="a5a4f-125">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="a5a4f-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5a4f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a5a4f-126">Request body</span></span>

<span data-ttu-id="a5a4f-127">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a5a4f-128">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5a4f-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a5a4f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5a4f-130">Property</span></span>     | <span data-ttu-id="a5a4f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a5a4f-131">Type</span></span>        | <span data-ttu-id="a5a4f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a5a4f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5a4f-133">description</span><span class="sxs-lookup"><span data-stu-id="a5a4f-133">description</span></span>|<span data-ttu-id="a5a4f-134">itemBody</span><span class="sxs-lookup"><span data-stu-id="a5a4f-134">itemBody</span></span>|<span data-ttu-id="a5a4f-135">Описание этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-135">The description of this rubric.</span></span>|
|<span data-ttu-id="a5a4f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a5a4f-136">displayName</span></span>|<span data-ttu-id="a5a4f-137">String</span><span class="sxs-lookup"><span data-stu-id="a5a4f-137">String</span></span>|<span data-ttu-id="a5a4f-138">Название этой рубрики.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-138">The name of this rubric.</span></span>|
|<span data-ttu-id="a5a4f-139">классификация</span><span class="sxs-lookup"><span data-stu-id="a5a4f-139">grading</span></span>|<span data-ttu-id="a5a4f-140">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="a5a4f-140">educationAssignmentGradeType</span></span>|<span data-ttu-id="a5a4f-141">Имеет ли эта рубрика очки или нет.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-141">Whether this rubric has points or not.</span></span>|
|<span data-ttu-id="a5a4f-142">уровни</span><span class="sxs-lookup"><span data-stu-id="a5a4f-142">levels</span></span>|<span data-ttu-id="a5a4f-143">коллекция rubricLevel</span><span class="sxs-lookup"><span data-stu-id="a5a4f-143">rubricLevel collection</span></span>|<span data-ttu-id="a5a4f-144">Коллекция уровней, в которые состоит эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-144">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="a5a4f-145">качества</span><span class="sxs-lookup"><span data-stu-id="a5a4f-145">qualities</span></span>|<span data-ttu-id="a5a4f-146">rubricQuality collection</span><span class="sxs-lookup"><span data-stu-id="a5a4f-146">rubricQuality collection</span></span>|<span data-ttu-id="a5a4f-147">Коллекция качеств, из которых состоит эта рубрика.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-147">The collection of qualities making up this rubric.</span></span>|

## <a name="response"></a><span data-ttu-id="a5a4f-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a4f-148">Response</span></span>

<span data-ttu-id="a5a4f-149">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationRubric](../resources/educationrubric.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-149">If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5a4f-150">Примеры</span><span class="sxs-lookup"><span data-stu-id="a5a4f-150">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a5a4f-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a4f-151">Request</span></span>

<span data-ttu-id="a5a4f-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-152">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5a4f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a4f-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/rubrics/{id}
Content-type: application/json

{
  "displayName": "Example Credit Rubric after display name patch"
}
```
# <a name="c"></a>[<span data-ttu-id="a5a4f-154">C#</span><span class="sxs-lookup"><span data-stu-id="a5a4f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5a4f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5a4f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5a4f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5a4f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5a4f-157">Java</span><span class="sxs-lookup"><span data-stu-id="a5a4f-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a5a4f-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a4f-158">Response</span></span>

<span data-ttu-id="a5a4f-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-159">The following is an example of the response.</span></span>

> <span data-ttu-id="a5a4f-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a5a4f-160">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "displayName": "Example Credit Rubric after display name patch",
    "id": "c4459fcb-a761-4f70-ac5b-e9466cb77c2a",
    "description": {
        "content": "This is an example of a credit rubric (no points)",
        "contentType": "text"
    },
    "levels": [
        {
            "levelId": "dec665d4-cf1b-4481-ac61-1d5b6188f4f5",
            "displayName": "Good",
            "description": {
                "content": "",
                "contentType": "text"
            }
        },
        {
            "levelId": "3f2e4b0f-508e-4005-984b-17e061bc5377",
            "displayName": "Poor",
            "description": {
                "content": "",
                "contentType": "text"
            }
        }
    ],
    "qualities": [
        {
            "qualityId": "dc79dcbf-b536-4797-9c5b-902f28129fd0",
            "description": {
                "content": "Argument",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "8937fa15-4a7c-4f27-bd01-ca3471d2d1d5",
                    "description": {
                        "content": "The essay's argument is persuasive.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "4dfb5263-1d3f-4f0a-93ef-d24d800d0f69",
                    "description": {
                        "content": "The essay's argument does not make sense.",
                        "contentType": "text"
                    }
                }
            ]
        },
        {
            "qualityId": "7e087062-ac25-4629-8386-a946350936db",
            "description": {
                "content": "Spelling and Grammar",
                "contentType": "text"
            },
            "criteria": [
                {
                    "id": "12276eb2-122c-4ad2-ba92-335ea798c88e",
                    "description": {
                        "content": "The essay uses proper spelling and grammar with few or no errors.",
                        "contentType": "text"
                    }
                },
                {
                    "id": "3db7e6b2-2b1b-4f8e-9fca-bea701159145",
                    "description": {
                        "content": "The essay has numerous errors in spelling and/or grammar.",
                        "contentType": "text"
                    }
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationrubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


