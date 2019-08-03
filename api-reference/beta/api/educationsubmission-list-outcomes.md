---
title: Результаты списка
description: Получение списка объектов едукатионауткоме.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7f7827576fbe6719e8a131af465a6ca61c686090
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173113"
---
# <a name="list-outcomes"></a><span data-ttu-id="21fa6-103">Результаты списка</span><span class="sxs-lookup"><span data-stu-id="21fa6-103">List outcomes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21fa6-104">Получение списка объектов [едукатионауткоме](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="21fa6-104">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="21fa6-105">Существует три типа результатов: **едукатионпоинтсауткоме**, **едукатионфидбаккауткоме**и **едукатионрубрикауткоме**.</span><span class="sxs-lookup"><span data-stu-id="21fa6-105">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="21fa6-106">При отправке для назначения кредита (у которого нет значения Point без точки и ни одного Rubric) будет [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="21fa6-106">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="21fa6-107">(Он также может возвращать [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md), но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="21fa6-107">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="21fa6-108">Отправка для назначения баллов (у которой есть назначенное значение точки) будет иметь как [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md) , так и [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="21fa6-108">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="21fa6-109">Отправка для назначения с присоединенным Rubric, если Rubric является кредит Rubric (нет точек), будут иметь [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md) и [едукатионрубрикауткоме](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="21fa6-109">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="21fa6-110">(Он также может возвращать [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md), но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="21fa6-110">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="21fa6-111">Отправка для назначения с присоединенным Rubric, если Rubric является точкой Rubric, будет иметь [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md), [едукатионпоинтсауткоме] (.. /ресаурцес/едукатионпоинтсауткоме.МД и [едукатионрубрикауткоме](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="21fa6-111">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="21fa6-112">Все типы результатов имеют обычные и опубликованные свойства, соответствующие этому типу результата; Например, **баллы** и **публишедпоинтс**, **Отзывы** и **публишедфидбакк**.</span><span class="sxs-lookup"><span data-stu-id="21fa6-112">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="21fa6-113">Регулярное свойство является последним значением, обновленным преподавателем; свойство Published — это последнее значение, возвращенное студенту.</span><span class="sxs-lookup"><span data-stu-id="21fa6-113">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="21fa6-114">Разрешения</span><span class="sxs-lookup"><span data-stu-id="21fa6-114">Permissions</span></span>

<span data-ttu-id="21fa6-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21fa6-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21fa6-117">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21fa6-117">Permission type</span></span>                        | <span data-ttu-id="21fa6-118">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="21fa6-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="21fa6-119">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21fa6-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="21fa6-120">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="21fa6-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="21fa6-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21fa6-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21fa6-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21fa6-122">Not supported.</span></span> |
| <span data-ttu-id="21fa6-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21fa6-123">Application</span></span>                            | <span data-ttu-id="21fa6-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21fa6-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21fa6-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21fa6-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="21fa6-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21fa6-126">Request headers</span></span>

| <span data-ttu-id="21fa6-127">Имя</span><span class="sxs-lookup"><span data-stu-id="21fa6-127">Name</span></span>      |<span data-ttu-id="21fa6-128">Описание</span><span class="sxs-lookup"><span data-stu-id="21fa6-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="21fa6-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="21fa6-129">Authorization</span></span> | <span data-ttu-id="21fa6-130">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="21fa6-130">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="21fa6-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21fa6-131">Request body</span></span>

<span data-ttu-id="21fa6-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="21fa6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21fa6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="21fa6-133">Response</span></span>

<span data-ttu-id="21fa6-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионауткоме](../resources/educationoutcome.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="21fa6-134">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="21fa6-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="21fa6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="21fa6-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="21fa6-136">Request</span></span>

<span data-ttu-id="21fa6-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21fa6-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```http
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```

### <a name="response"></a><span data-ttu-id="21fa6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="21fa6-138">Response</span></span>

<span data-ttu-id="21fa6-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="21fa6-139">The following is an example of the response.</span></span>

> <span data-ttu-id="21fa6-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="21fa6-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationOutcome",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
            "id": "ca05367a-b292-42d5-aff7-5d279feeace8",
            "feedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedFeedback": {
                "feedbackDateTime": "2019-07-15T22:35:46.4847754Z",
                "text": {
                    "content": "This is feedback for the assignment as a whole.",
                    "contentType": "text"
                },
                "feedbackBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationPointsOutcome",
            "id": "ea1351f6-ba33-4940-b2cb-6a7254af2dc8",
            "points": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            },
            "publishedPoints": {
                "gradedDateTime": "2019-07-15T22:36:02.2592364Z",
                "points": 75,
                "gradedBy": {
                    "user": {
                        "id": "9391878d-903c-406c-bb1c-0f17d00fd878"
                    }
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.educationRubricOutcome",
            "id": "65a46d78-1a2b-4a7e-bcf8-78a22ac2611b",
            "rubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "rubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
                }
            ],
            "publishedRubricQualityFeedback": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "feedback": {
                        "content": "This is feedback specific to this quality of the rubric.",
                        "contentType": "text"
                    }
                }
            ],
            "publishedRubricQualitySelectedLevels": [
                {
                    "qualityId": "ebe97fd7-47f7-4e9a-b31b-221ad731fc5a",
                    "columnId": "db2a0c91-abef-44cb-b8b1-ef1f85ef4a77"
                },
                {
                    "qualityId": "bbf3fb4a-a794-4b51-a1ad-c22fb891c5d8",
                    "columnId": "519cd134-c513-40b9-aa71-fdb0d063c084"
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
  "description": "List outcomes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
