---
title: Обновление educationOutcome
description: Обновление свойств объекта educationOutcome.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6b3fba4f87f17528c1e4774b34ba4faeae43bfb
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912738"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="c6955-103">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="c6955-103">Update educationoutcome</span></span>

<span data-ttu-id="c6955-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6955-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6955-105">Обновление свойств объекта [educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="c6955-105">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6955-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6955-106">Permissions</span></span>

<span data-ttu-id="c6955-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6955-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6955-109">Permission type</span></span>                        | <span data-ttu-id="c6955-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c6955-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c6955-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6955-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6955-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6955-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="c6955-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6955-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6955-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6955-114">Not supported.</span></span> |
| <span data-ttu-id="c6955-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6955-115">Application</span></span>                            | <span data-ttu-id="c6955-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6955-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6955-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6955-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141
```

## <a name="request-headers"></a><span data-ttu-id="c6955-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6955-118">Request headers</span></span>

| <span data-ttu-id="c6955-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c6955-119">Name</span></span>       | <span data-ttu-id="c6955-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c6955-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c6955-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c6955-121">Authorization</span></span> | <span data-ttu-id="c6955-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c6955-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6955-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c6955-123">Request body</span></span>

<span data-ttu-id="c6955-124">В теле запроса поставляют только значения полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="c6955-124">In the request body, supply only the values of the fields you want to update.</span></span>

<span data-ttu-id="c6955-125">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="c6955-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c6955-126">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="c6955-126">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="c6955-127">Объект educationOutcome будет одним из следующих производных типов: **educationPointsOutcome,** **educationFeedbackOutcome** или **educationRubricOutcome.**</span><span class="sxs-lookup"><span data-stu-id="c6955-127">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="c6955-128">Поставляем конкретные свойства, соответствующие типу исправленного результата.</span><span class="sxs-lookup"><span data-stu-id="c6955-128">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="c6955-129">Все производные типы результатов имеют обычное и "опубликованное" свойство, соответствующее этому типу результатов; например, **точки** и **опубликованныеPoints,** **отзывы** и **опубликованныеFeedback**.</span><span class="sxs-lookup"><span data-stu-id="c6955-129">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="c6955-130">Не обновляйте свойство "опубликовано"; это для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c6955-130">Don't update the "published" property; it is for internal use.</span></span> <span data-ttu-id="c6955-131">Например, чтобы назначить точки **в educationPointsOutcome,** обновите свойство точек, но не обновляйте **опубликованные Точки**. </span><span class="sxs-lookup"><span data-stu-id="c6955-131">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but Don't update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="c6955-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6955-132">Response</span></span>

<span data-ttu-id="c6955-133">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект educationOutcome](../resources/educationoutcome.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c6955-133">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6955-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="c6955-134">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="c6955-135">Пример 1. Обновление результатов обратной связи</span><span class="sxs-lookup"><span data-stu-id="c6955-135">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="c6955-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6955-136">Request</span></span>

<span data-ttu-id="c6955-137">Ниже приводится пример запроса на обновление результатов обратной связи.</span><span class="sxs-lookup"><span data-stu-id="c6955-137">The following is an example of the request for updating a feedback outcome.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c6955-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6955-138">Response</span></span>

<span data-ttu-id="c6955-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6955-139">The following is an example of the response.</span></span>

> <span data-ttu-id="c6955-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6955-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="c6955-141">Пример 2. Обновление результатов баллов</span><span class="sxs-lookup"><span data-stu-id="c6955-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="c6955-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6955-142">Request</span></span>

<span data-ttu-id="c6955-143">Ниже приводится пример запроса на обновление результатов точек.</span><span class="sxs-lookup"><span data-stu-id="c6955-143">The following is an example of the request for updating a points outcome.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c6955-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6955-144">Response</span></span>

<span data-ttu-id="c6955-145">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6955-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c6955-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6955-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="c6955-147">Пример 3. Обновление итога рубрики</span><span class="sxs-lookup"><span data-stu-id="c6955-147">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="c6955-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6955-148">Request</span></span>

<span data-ttu-id="c6955-149">Ниже приводится пример запроса на обновление результатов рубрики.</span><span class="sxs-lookup"><span data-stu-id="c6955-149">The following is an example of the request for updating a rubric outcome.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c6955-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6955-150">Response</span></span>

<span data-ttu-id="c6955-151">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6955-151">The following is an example of the response.</span></span>

> <span data-ttu-id="c6955-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6955-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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


