---
title: Обновление educationOutcome
description: Обновление свойств объекта educationOutcome.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5f27763d558590e01f61fbc231959b05bee3c296
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043722"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="90602-103">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="90602-103">Update educationoutcome</span></span>

<span data-ttu-id="90602-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90602-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90602-105">Обновление свойств объекта [educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="90602-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="90602-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90602-106">Permissions</span></span>

<span data-ttu-id="90602-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90602-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="90602-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90602-109">Permission type</span></span>                        | <span data-ttu-id="90602-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90602-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="90602-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90602-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="90602-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90602-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="90602-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90602-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90602-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90602-114">Not supported.</span></span> |
| <span data-ttu-id="90602-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90602-115">Application</span></span>                            | <span data-ttu-id="90602-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90602-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90602-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90602-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="90602-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90602-118">Request headers</span></span>

| <span data-ttu-id="90602-119">Имя</span><span class="sxs-lookup"><span data-stu-id="90602-119">Name</span></span>       | <span data-ttu-id="90602-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90602-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="90602-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90602-121">Authorization</span></span> | <span data-ttu-id="90602-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="90602-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="90602-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90602-123">Request body</span></span>

<span data-ttu-id="90602-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="90602-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="90602-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="90602-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="90602-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="90602-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="90602-127">Объект educationOutcome будет одним из следующих производных типов: **educationPointsOutcome,** **educationFeedbackOutcome** или **educationRubricOutcome.**</span><span class="sxs-lookup"><span data-stu-id="90602-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="90602-128">Поставляем конкретные свойства, соответствующие типу исправленного результата.</span><span class="sxs-lookup"><span data-stu-id="90602-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="90602-129">Все производные типы результатов имеют обычное и "опубликованное" свойство, соответствующее этому типу результатов; например, **точки** и **опубликованныеPoints,** **отзывы** и **опубликованныеFeedback**.</span><span class="sxs-lookup"><span data-stu-id="90602-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="90602-130">Не обновляем свойство "опубликовано"; это для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="90602-130">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="90602-131">Например, чтобы назначить точки **в educationPointsOutcome,** обновите свойство точек, но не обновляя **опубликованные Точки**. </span><span class="sxs-lookup"><span data-stu-id="90602-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="90602-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="90602-132">Response</span></span>

<span data-ttu-id="90602-133">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationOutcome](../resources/educationoutcome.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="90602-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="90602-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="90602-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="90602-135">Пример 1. Обновление результатов обратной связи</span><span class="sxs-lookup"><span data-stu-id="90602-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="90602-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="90602-136">Request</span></span>

<span data-ttu-id="90602-137">Ниже приводится пример запроса на обновление результатов обратной связи.</span><span class="sxs-lookup"><span data-stu-id="90602-137">The following is an example of the request for updating a feedback outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="90602-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="90602-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationFeedbackOutcome",
    "feedback":{
        "text":{
            "content":"This is feedback for the assignment as a whole.",
            "contentType":"text"
        }
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="90602-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90602-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationfeedbackoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="90602-140">C#</span><span class="sxs-lookup"><span data-stu-id="90602-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationfeedbackoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90602-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90602-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationfeedbackoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90602-142">Java</span><span class="sxs-lookup"><span data-stu-id="90602-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationfeedbackoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90602-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="90602-143">Response</span></span>

<span data-ttu-id="90602-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90602-144">The following is an example of the response.</span></span>

> <span data-ttu-id="90602-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90602-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFeedbackOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
    "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
    "lastModifiedBy": {
        "user": {
            "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "feedback": {
        "feedbackDateTime": "2019-07-31T21:10:30.3231461Z",
        "text": {
            "content": "This is feedback for the assignment as a whole.",
            "contentType": "text"
        },
        "feedbackBy": {
            "user": {
                "id": "9391878d-903c-406c-bb1c-0f17d00fd878",
            }
        }
    }
}
```

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="90602-146">Пример 2. Обновление результатов баллов</span><span class="sxs-lookup"><span data-stu-id="90602-146">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="90602-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="90602-147">Request</span></span>

<span data-ttu-id="90602-148">Ниже приводится пример запроса на обновление результатов точек.</span><span class="sxs-lookup"><span data-stu-id="90602-148">The following is an example of the request for updating a points outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="90602-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="90602-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```
# <a name="javascript"></a>[<span data-ttu-id="90602-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90602-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationpointsoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="90602-151">C#</span><span class="sxs-lookup"><span data-stu-id="90602-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationpointsoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90602-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90602-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationpointsoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90602-153">Java</span><span class="sxs-lookup"><span data-stu-id="90602-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationpointsoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90602-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="90602-154">Response</span></span>

<span data-ttu-id="90602-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90602-155">The following is an example of the response.</span></span>

> <span data-ttu-id="90602-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90602-156">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "id":"ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
    "lastModifiedBy":{
        "user":{
            "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
        }
    },
    "points":{
        "gradedDateTime":"2019-07-15T22:35:48.2429387Z",
        "points":85.0,
        "gradedBy":{
            "user":{
                "id":"9391878d-903c-406c-bb1c-0f17d00fd878"
            }
        }
    }
}
```

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="90602-157">Пример 3. Обновление итога рубрики</span><span class="sxs-lookup"><span data-stu-id="90602-157">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="90602-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="90602-158">Request</span></span>

<span data-ttu-id="90602-159">Ниже приводится пример запроса на обновление результатов рубрики.</span><span class="sxs-lookup"><span data-stu-id="90602-159">The following is an example of the request for updating a rubric outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="90602-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="90602-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes/{id}
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback":{
                "content":"This is feedback specific to the first quality of the rubric.",
                "contentType":"text"
            }
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback":{
                "content":"This is feedback specific to the second quality of the rubric.",
                "contentType":"text"
            }
        }
    ],
    "rubricQualitySelectedLevels":[
        {
            "qualityId":"9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId":"4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId":"d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId":"aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="90602-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90602-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="90602-162">C#</span><span class="sxs-lookup"><span data-stu-id="90602-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90602-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90602-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90602-164">Java</span><span class="sxs-lookup"><span data-stu-id="90602-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90602-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="90602-165">Response</span></span>

<span data-ttu-id="90602-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90602-166">The following is an example of the response.</span></span>

> <span data-ttu-id="90602-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="90602-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationPointsOutcome"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
    "rubricQualityFeedback": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "feedback": {
                "content": "This is feedback specific to the first quality of the rubric.",
                "contentType": "text"
            }
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "feedback": {
                "content": "This is feedback specific to the second quality of the rubric.",
                "contentType": "text"
            }
        }
    ],
    "rubricQualitySelectedLevels": [
        {
            "qualityId": "9a145aa8-f3d9-43a1-8f77-5387ff0693f2",
            "columnId": "4fb17a1d-5681-46c2-a295-4e305c3eae23"
        },
        {
            "qualityId": "d2331fb2-2761-402e-8de6-93e0afaa076e",
            "columnId": "aac076bf-51ba-48c5-a2e0-ee235b0b9740"
        }
    ]
}
```



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationoutcome",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


