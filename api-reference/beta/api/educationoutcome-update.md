---
title: Обновление Едукатионауткоме
description: Обновление свойств объекта Едукатионауткоме.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f33383ea8c3c8b7369be47aa852847af022884ef
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966149"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="6baec-103">Обновление едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="6baec-103">Update educationoutcome</span></span>

<span data-ttu-id="6baec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6baec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6baec-105">Обновление свойств объекта [едукатионауткоме](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="6baec-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6baec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6baec-106">Permissions</span></span>

<span data-ttu-id="6baec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6baec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6baec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6baec-109">Permission type</span></span>                        | <span data-ttu-id="6baec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6baec-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6baec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6baec-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6baec-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6baec-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="6baec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6baec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6baec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6baec-114">Not supported.</span></span> |
| <span data-ttu-id="6baec-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6baec-115">Application</span></span>                            | <span data-ttu-id="6baec-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6baec-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6baec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6baec-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6baec-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6baec-118">Request headers</span></span>

| <span data-ttu-id="6baec-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6baec-119">Name</span></span>       | <span data-ttu-id="6baec-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6baec-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6baec-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6baec-121">Authorization</span></span> | <span data-ttu-id="6baec-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6baec-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6baec-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6baec-123">Request body</span></span>

<span data-ttu-id="6baec-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="6baec-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6baec-125">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="6baec-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6baec-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="6baec-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="6baec-127">Объект Едукатионауткоме будет одним из следующих производных типов: **едукатионпоинтсауткоме** , **едукатионфидбаккауткоме** или **едукатионрубрикауткоме**.</span><span class="sxs-lookup"><span data-stu-id="6baec-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome** , **educationFeedbackOutcome** , or **educationRubricOutcome**.</span></span> <span data-ttu-id="6baec-128">Предоставьте конкретные свойства, относящиеся к типу обновляемого результата.</span><span class="sxs-lookup"><span data-stu-id="6baec-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="6baec-129">Все производные типы результатов имеют обычные и публикуемые свойства, соответствующие этому типу результата; Например, **баллы** и **публишедпоинтс** , **Отзывы** и **публишедфидбакк**.</span><span class="sxs-lookup"><span data-stu-id="6baec-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints** , **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="6baec-130">Не обновляйте свойство "Опубликовано"; Он предназначен для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6baec-130">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="6baec-131">Например, чтобы назначить точки **едукатионпоинтсауткоме** , обновите свойство **points** , но не обновляйте **публишедпоинтс**.</span><span class="sxs-lookup"><span data-stu-id="6baec-131">For example, to assign points to an **educationPointsOutcome** , update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="6baec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="6baec-132">Response</span></span>

<span data-ttu-id="6baec-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионауткоме](../resources/educationoutcome.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6baec-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6baec-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="6baec-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="6baec-135">Пример 1: обновление результатов обратной связи</span><span class="sxs-lookup"><span data-stu-id="6baec-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="6baec-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="6baec-136">Request</span></span>

<span data-ttu-id="6baec-137">Ниже приведен пример запроса на обновление результатов обратной связи.</span><span class="sxs-lookup"><span data-stu-id="6baec-137">The following is an example of the request for updating a feedback outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="6baec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6baec-138">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6baec-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6baec-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationfeedbackoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6baec-140">C#</span><span class="sxs-lookup"><span data-stu-id="6baec-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationfeedbackoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6baec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6baec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationfeedbackoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6baec-142">Java</span><span class="sxs-lookup"><span data-stu-id="6baec-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationfeedbackoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6baec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="6baec-143">Response</span></span>

<span data-ttu-id="6baec-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6baec-144">The following is an example of the response.</span></span>

> <span data-ttu-id="6baec-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6baec-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="6baec-147">Пример 2: обновление результата баллов</span><span class="sxs-lookup"><span data-stu-id="6baec-147">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="6baec-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="6baec-148">Request</span></span>

<span data-ttu-id="6baec-149">Ниже приведен пример запроса на обновление результата баллов.</span><span class="sxs-lookup"><span data-stu-id="6baec-149">The following is an example of the request for updating a points outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="6baec-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6baec-150">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6baec-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6baec-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationpointsoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6baec-152">C#</span><span class="sxs-lookup"><span data-stu-id="6baec-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationpointsoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6baec-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6baec-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationpointsoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6baec-154">Java</span><span class="sxs-lookup"><span data-stu-id="6baec-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationpointsoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6baec-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6baec-155">Response</span></span>

<span data-ttu-id="6baec-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6baec-156">The following is an example of the response.</span></span>

> <span data-ttu-id="6baec-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6baec-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="6baec-159">Пример 3: обновление результата Rubric</span><span class="sxs-lookup"><span data-stu-id="6baec-159">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="6baec-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="6baec-160">Request</span></span>

<span data-ttu-id="6baec-161">Ниже приведен пример запроса на обновление результата Rubric.</span><span class="sxs-lookup"><span data-stu-id="6baec-161">The following is an example of the request for updating a rubric outcome.</span></span>

# <a name="http"></a>[<span data-ttu-id="6baec-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="6baec-162">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="6baec-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6baec-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6baec-164">C#</span><span class="sxs-lookup"><span data-stu-id="6baec-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6baec-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6baec-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6baec-166">Java</span><span class="sxs-lookup"><span data-stu-id="6baec-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6baec-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="6baec-167">Response</span></span>

<span data-ttu-id="6baec-168">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6baec-168">The following is an example of the response.</span></span>

> <span data-ttu-id="6baec-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6baec-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


