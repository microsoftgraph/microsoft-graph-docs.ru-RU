---
title: Результаты списка
description: Получение списка объектов едукатионауткоме.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fe51b0fae482467f2ceddbffae1537e6399ed800
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007345"
---
# <a name="list-outcomes"></a><span data-ttu-id="1c085-103">Результаты списка</span><span class="sxs-lookup"><span data-stu-id="1c085-103">List outcomes</span></span>

<span data-ttu-id="1c085-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c085-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1c085-105">Получение списка объектов [едукатионауткоме](../resources/educationoutcome.md) .</span><span class="sxs-lookup"><span data-stu-id="1c085-105">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="1c085-106">Существует три типа результатов: **едукатионпоинтсауткоме**, **едукатионфидбаккауткоме**и **едукатионрубрикауткоме**.</span><span class="sxs-lookup"><span data-stu-id="1c085-106">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="1c085-107">При отправке для назначения кредита (у которого нет значения Point без точки и ни одного Rubric) будет [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="1c085-107">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="1c085-108">(Он также может возвращать [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md), но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="1c085-108">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="1c085-109">Отправка для назначения баллов (у которой есть назначенное значение точки) будет иметь как [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md) , так и [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="1c085-109">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="1c085-110">Отправка для назначения с присоединенным Rubric, если Rubric является кредит Rubric (нет точек), будут иметь [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md) и [едукатионрубрикауткоме](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="1c085-110">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="1c085-111">(Он также может возвращать [едукатионпоинтсауткоме](../resources/educationpointsoutcome.md), но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="1c085-111">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="1c085-112">Отправка для назначения с присоединенным Rubric, если Rubric является точкой Rubric, будет иметь [едукатионфидбаккауткоме](../resources/educationpointsoutcome.md), [едукатионпоинтсауткоме] (.. /ресаурцес/едукатионпоинтсауткоме.МД и [едукатионрубрикауткоме](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="1c085-112">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="1c085-113">Все типы результатов имеют обычные и опубликованные свойства, соответствующие этому типу результата; Например, **баллы** и **публишедпоинтс**, **Отзывы** и **публишедфидбакк**.</span><span class="sxs-lookup"><span data-stu-id="1c085-113">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="1c085-114">Регулярное свойство является последним значением, обновленным преподавателем; свойство Published — это последнее значение, возвращенное студенту.</span><span class="sxs-lookup"><span data-stu-id="1c085-114">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c085-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1c085-115">Permissions</span></span>

<span data-ttu-id="1c085-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c085-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1c085-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c085-118">Permission type</span></span>                        | <span data-ttu-id="1c085-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c085-119">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1c085-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c085-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c085-121">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1c085-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1c085-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c085-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c085-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c085-123">Not supported.</span></span> |
| <span data-ttu-id="1c085-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1c085-124">Application</span></span>                            | <span data-ttu-id="1c085-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c085-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c085-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c085-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="1c085-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c085-127">Request headers</span></span>

| <span data-ttu-id="1c085-128">Имя</span><span class="sxs-lookup"><span data-stu-id="1c085-128">Name</span></span>      |<span data-ttu-id="1c085-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1c085-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1c085-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1c085-130">Authorization</span></span> | <span data-ttu-id="1c085-131">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="1c085-131">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c085-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c085-132">Request body</span></span>

<span data-ttu-id="1c085-133">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1c085-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c085-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c085-134">Response</span></span>

<span data-ttu-id="1c085-135">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионауткоме](../resources/educationoutcome.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1c085-135">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1c085-136">Примеры</span><span class="sxs-lookup"><span data-stu-id="1c085-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1c085-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c085-137">Request</span></span>

<span data-ttu-id="1c085-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c085-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1c085-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1c085-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```
# <a name="c"></a>[<span data-ttu-id="1c085-140">C#</span><span class="sxs-lookup"><span data-stu-id="1c085-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1c085-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1c085-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1c085-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1c085-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1c085-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c085-143">Response</span></span>

<span data-ttu-id="1c085-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1c085-144">The following is an example of the response.</span></span>

> <span data-ttu-id="1c085-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c085-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


