---
title: Обновление educationOutcome
description: Обновление свойств объекта educationOutcome.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcc9c011b4c23c088f887184891781af2f9f8338
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991359"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="27a19-103">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="27a19-103">Update educationoutcome</span></span>

<span data-ttu-id="27a19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27a19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="27a19-105">Обновление свойств объекта [educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="27a19-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="27a19-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27a19-106">Permissions</span></span>

<span data-ttu-id="27a19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27a19-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a19-109">Permission type</span></span>                        | <span data-ttu-id="27a19-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a19-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="27a19-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a19-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="27a19-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27a19-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="27a19-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a19-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="27a19-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a19-114">Not supported.</span></span> |
| <span data-ttu-id="27a19-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a19-115">Application</span></span>                            | <span data-ttu-id="27a19-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a19-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="27a19-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
```

## <a name="request-headers"></a><span data-ttu-id="27a19-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a19-118">Request headers</span></span>

| <span data-ttu-id="27a19-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27a19-119">Name</span></span>       | <span data-ttu-id="27a19-120">Описание</span><span class="sxs-lookup"><span data-stu-id="27a19-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="27a19-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="27a19-121">Authorization</span></span> | <span data-ttu-id="27a19-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="27a19-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="27a19-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27a19-123">Request body</span></span>

<span data-ttu-id="27a19-124">В теле запроса поставляют только значения полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="27a19-124">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="27a19-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="27a19-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="27a19-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="27a19-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="27a19-127">Объект educationOutcome будет одним из следующих производных типов: **educationPointsOutcome,** **educationFeedbackOutcome** или **educationRubricOutcome.**</span><span class="sxs-lookup"><span data-stu-id="27a19-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="27a19-128">Поставляем конкретные свойства, соответствующие типу исправленного результата.</span><span class="sxs-lookup"><span data-stu-id="27a19-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="27a19-129">Все производные типы результатов имеют обычное и "опубликованное" свойство, соответствующее этому типу результатов; например, **точки** и **опубликованныеPoints,** **отзывы** и **опубликованныеFeedback**.</span><span class="sxs-lookup"><span data-stu-id="27a19-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="27a19-130">Не обновляйте свойство "опубликовано"; это для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="27a19-130">Don't update the "published" property; it is for internal use.</span></span> <span data-ttu-id="27a19-131">Например, чтобы назначить точки **в educationPointsOutcome,** обновите свойство точек, но не обновляйте **опубликованные Точки**. </span><span class="sxs-lookup"><span data-stu-id="27a19-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but Don't update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="27a19-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a19-132">Response</span></span>

<span data-ttu-id="27a19-133">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationOutcome](../resources/educationoutcome.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="27a19-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="27a19-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="27a19-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="27a19-135">Пример 1. Обновление результатов обратной связи</span><span class="sxs-lookup"><span data-stu-id="27a19-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="27a19-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a19-136">Request</span></span>

<span data-ttu-id="27a19-137">Ниже приводится пример запроса на обновление результатов обратной связи.</span><span class="sxs-lookup"><span data-stu-id="27a19-137">The following is an example of the request for updating a feedback outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="27a19-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="27a19-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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
# <a name="c"></a>[<span data-ttu-id="27a19-139">C#</span><span class="sxs-lookup"><span data-stu-id="27a19-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationfeedbackoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27a19-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27a19-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationfeedbackoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27a19-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27a19-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationfeedbackoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27a19-142">Java</span><span class="sxs-lookup"><span data-stu-id="27a19-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationfeedbackoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="27a19-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a19-143">Response</span></span>

<span data-ttu-id="27a19-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27a19-144">The following is an example of the response.</span></span>

> <span data-ttu-id="27a19-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27a19-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="27a19-146">Пример 2. Обновление результатов баллов</span><span class="sxs-lookup"><span data-stu-id="27a19-146">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="27a19-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a19-147">Request</span></span>

<span data-ttu-id="27a19-148">Ниже приводится пример запроса на обновление результатов точек.</span><span class="sxs-lookup"><span data-stu-id="27a19-148">The following is an example of the request for updating a points outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="27a19-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="27a19-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationpointsoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.educationPointsOutcome",
    "points":{
        "@odata.type":"#microsoft.graph.educationAssignmentPointsGrade",
        "points":85.0
    }
}
```
# <a name="c"></a>[<span data-ttu-id="27a19-150">C#</span><span class="sxs-lookup"><span data-stu-id="27a19-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationpointsoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27a19-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27a19-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationpointsoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27a19-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27a19-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationpointsoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27a19-153">Java</span><span class="sxs-lookup"><span data-stu-id="27a19-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationpointsoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="27a19-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a19-154">Response</span></span>

<span data-ttu-id="27a19-155">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27a19-155">The following is an example of the response.</span></span>

> <span data-ttu-id="27a19-156">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27a19-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="27a19-157">Пример 3. Обновление итога рубрики</span><span class="sxs-lookup"><span data-stu-id="27a19-157">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="27a19-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a19-158">Request</span></span>

<span data-ttu-id="27a19-159">Ниже приводится пример запроса на обновление результатов рубрики.</span><span class="sxs-lookup"><span data-stu-id="27a19-159">The following is an example of the request for updating a rubric outcome.</span></span>


# <a name="http"></a>[<span data-ttu-id="27a19-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="27a19-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationoutcome"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
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
# <a name="c"></a>[<span data-ttu-id="27a19-161">C#</span><span class="sxs-lookup"><span data-stu-id="27a19-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationoutcome-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="27a19-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="27a19-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationoutcome-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="27a19-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="27a19-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationoutcome-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="27a19-164">Java</span><span class="sxs-lookup"><span data-stu-id="27a19-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationoutcome-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="27a19-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a19-165">Response</span></span>

<span data-ttu-id="27a19-166">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="27a19-166">The following is an example of the response.</span></span>

> <span data-ttu-id="27a19-167">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27a19-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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


