---
title: Обновление Едукатионауткоме
description: Обновление свойств объекта Едукатионауткоме.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2c7b85d3456927e6a63f61f11722dfe8eccf270e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173183"
---
# <a name="update-educationoutcome"></a><span data-ttu-id="bd858-103">Обновление едукатионауткоме</span><span class="sxs-lookup"><span data-stu-id="bd858-103">Update educationoutcome</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd858-104">Обновление свойств объекта [едукатионауткоме](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="bd858-104">Update the properties of an [educationOutcome](../resources/educationoutcome.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd858-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd858-105">Permissions</span></span>

<span data-ttu-id="bd858-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd858-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd858-108">Permission type</span></span>                        | <span data-ttu-id="bd858-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd858-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bd858-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd858-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd858-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd858-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="bd858-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd858-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd858-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd858-113">Not supported.</span></span> |
| <span data-ttu-id="bd858-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd858-114">Application</span></span>                            | <span data-ttu-id="bd858-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd858-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd858-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd858-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bd858-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd858-117">Request headers</span></span>

| <span data-ttu-id="bd858-118">Имя</span><span class="sxs-lookup"><span data-stu-id="bd858-118">Name</span></span>       | <span data-ttu-id="bd858-119">Описание</span><span class="sxs-lookup"><span data-stu-id="bd858-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bd858-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd858-120">Authorization</span></span> | <span data-ttu-id="bd858-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="bd858-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd858-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd858-122">Request body</span></span>

<span data-ttu-id="bd858-123">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="bd858-123">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bd858-124">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="bd858-124">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bd858-125">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="bd858-125">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="bd858-126">Объект Едукатионауткоме будет одним из следующих производных типов: **едукатионпоинтсауткоме**, **едукатионфидбаккауткоме**или **едукатионрубрикауткоме**.</span><span class="sxs-lookup"><span data-stu-id="bd858-126">The educationOutcome object will be one of the following derived types: **educationPointsOutcome**, **educationFeedbackOutcome**, or **educationRubricOutcome**.</span></span> <span data-ttu-id="bd858-127">Предоставьте конкретные свойства, относящиеся к типу обновляемого результата.</span><span class="sxs-lookup"><span data-stu-id="bd858-127">Supply the specific properties relevant to the type of outcome being patched.</span></span>

<span data-ttu-id="bd858-128">Все производные типы результатов имеют обычные и публикуемые свойства, соответствующие этому типу результата; Например, **баллы** и **публишедпоинтс**, **Отзывы** и **публишедфидбакк**.</span><span class="sxs-lookup"><span data-stu-id="bd858-128">All derived outcome types have a regular and a "published" property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span> <span data-ttu-id="bd858-129">Не обновляйте свойство "Опубликовано"; Он предназначен для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="bd858-129">Do not update the "published" property; it is for internal use.</span></span> <span data-ttu-id="bd858-130">Например, чтобы назначить точки **едукатионпоинтсауткоме**, обновите свойство Points \*\*\*\* , но не обновляйте **публишедпоинтс**.</span><span class="sxs-lookup"><span data-stu-id="bd858-130">For example, to assign points to an **educationPointsOutcome**, update the **points** property, but do not update **publishedPoints**.</span></span>

## <a name="response"></a><span data-ttu-id="bd858-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd858-131">Response</span></span>

<span data-ttu-id="bd858-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [едукатионауткоме](../resources/educationoutcome.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd858-132">If successful, this method returns a `200 OK` response code and an updated [educationOutcome](../resources/educationoutcome.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bd858-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="bd858-133">Examples</span></span>

### <a name="example-1-update-a-feedback-outcome"></a><span data-ttu-id="bd858-134">Пример 1: обновление результатов обратной связи</span><span class="sxs-lookup"><span data-stu-id="bd858-134">Example 1: Update a Feedback Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="bd858-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd858-135">Request</span></span>

<span data-ttu-id="bd858-136">Ниже приведен пример запроса на обновление результатов обратной связи.</span><span class="sxs-lookup"><span data-stu-id="bd858-136">The following is an example of the request for updating a feedback outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="bd858-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd858-137">Response</span></span>

<span data-ttu-id="bd858-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd858-138">The following is an example of the response.</span></span>

> <span data-ttu-id="bd858-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd858-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-points-outcome"></a><span data-ttu-id="bd858-141">Пример 2: обновление результата баллов</span><span class="sxs-lookup"><span data-stu-id="bd858-141">Example 2: Update a Points Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="bd858-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd858-142">Request</span></span>

<span data-ttu-id="bd858-143">Ниже приведен пример запроса на обновление результата баллов.</span><span class="sxs-lookup"><span data-stu-id="bd858-143">The following is an example of the request for updating a points outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="bd858-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd858-144">Response</span></span>

<span data-ttu-id="bd858-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd858-145">The following is an example of the response.</span></span>

> <span data-ttu-id="bd858-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd858-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-update-a-rubric-outcome"></a><span data-ttu-id="bd858-148">Пример 3: обновление результата Rubric</span><span class="sxs-lookup"><span data-stu-id="bd858-148">Example 3: Update a Rubric Outcome</span></span>

#### <a name="request"></a><span data-ttu-id="bd858-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd858-149">Request</span></span>

<span data-ttu-id="bd858-150">Ниже приведен пример запроса на обновление результата Rubric.</span><span class="sxs-lookup"><span data-stu-id="bd858-150">The following is an example of the request for updating a rubric outcome.</span></span>
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

#### <a name="response"></a><span data-ttu-id="bd858-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd858-151">Response</span></span>

<span data-ttu-id="bd858-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd858-152">The following is an example of the response.</span></span>

> <span data-ttu-id="bd858-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd858-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
