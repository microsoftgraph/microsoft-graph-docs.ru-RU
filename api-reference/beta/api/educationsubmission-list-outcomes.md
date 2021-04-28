---
title: Результаты списка
description: Извлечение списка объектов educationoutcome.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6a351467a96b60aa2bcabd560db910c88d999a67
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061821"
---
# <a name="list-outcomes"></a><span data-ttu-id="d8f3b-103">Результаты списка</span><span class="sxs-lookup"><span data-stu-id="d8f3b-103">List outcomes</span></span>

<span data-ttu-id="d8f3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8f3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8f3b-105">Извлечение списка [объектов educationOutcome.](../resources/educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-105">Retrieve a list of [educationOutcome](../resources/educationoutcome.md) objects.</span></span>  <span data-ttu-id="d8f3b-106">Существует три типа результатов: **educationPointsOutcome,** **educationFeedbackOutcome** и **educationRubricOutcome.**</span><span class="sxs-lookup"><span data-stu-id="d8f3b-106">There are three types of outcomes: **educationPointsOutcome**, **educationFeedbackOutcome**, and **educationRubricOutcome**.</span></span>

<span data-ttu-id="d8f3b-107">Отправка для назначения кредита (не имеет значения точки и нет рубрики) будет иметь [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="d8f3b-107">A submission for a credit assignment (one that has no point value and no rubric) will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md).</span></span> <span data-ttu-id="d8f3b-108">(Это может также вернуть [educationPointsOutcome,](../resources/educationpointsoutcome.md)но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-108">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="d8f3b-109">Отправка для назначения точек (назначенное значение точки) будет иметь как [educationFeedbackOutcome,](../resources/educationpointsoutcome.md) так и [educationPointsOutcome.](../resources/educationpointsoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-109">A submission for a points assignment (one that has a point value assigned) will have both an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationPointsOutcome](../resources/educationpointsoutcome.md).</span></span>

<span data-ttu-id="d8f3b-110">Отправка для назначения с прикрепленной рубрикой, если рубрика является кредитной рубрикой (без баллов), будет иметь [educationFeedbackOutcome](../resources/educationpointsoutcome.md) и [educationRubricOutcome](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="d8f3b-110">A submission for an assignment with an attached rubric, if the rubric is a credit rubric (no points), will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md) and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span> <span data-ttu-id="d8f3b-111">(Это может также вернуть [educationPointsOutcome,](../resources/educationpointsoutcome.md)но этот результат игнорируется.)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-111">(It might also return an [educationPointsOutcome](../resources/educationpointsoutcome.md), but that outcome is ignored.)</span></span>

<span data-ttu-id="d8f3b-112">Отправка для назначения с прикрепленной рубрикой, если рубрика является рубрикой точек, будет иметь [educationFeedbackOutcome](../resources/educationpointsoutcome.md), [educationPointsOutcome].. /resources/educationpointsoutcome.md и [educationRubricOutcome](../resources/educationrubricoutcome.md).</span><span class="sxs-lookup"><span data-stu-id="d8f3b-112">A submission for an assignment with an attached rubric, if the rubric is a points rubric, will have an [educationFeedbackOutcome](../resources/educationpointsoutcome.md), an [educationPointsOutcome](../resources/educationpointsoutcome.md, and an [educationRubricOutcome](../resources/educationrubricoutcome.md).</span></span>

<span data-ttu-id="d8f3b-113">Все типы результатов имеют обычное и опубликованное свойство, соответствующее этому типу результатов; например, **точки** и **опубликованныеPoints,** **отзывы** и **опубликованныеFeedback**.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-113">All outcome types have a regular and a published property appropriate to that type of outcome; for example, **points** and **publishedPoints**, **feedback** and **publishedFeedback**.</span></span>  <span data-ttu-id="d8f3b-114">Обычное свойство — это последнее значение, обновленное преподавателем; опубликованное свойство — это самое последнее значение, возвращенное студенту.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-114">The regular property is the most recent value updated by the teacher; the published property is the most recent value returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8f3b-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8f3b-115">Permissions</span></span>

<span data-ttu-id="d8f3b-p105">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8f3b-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8f3b-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8f3b-118">Permission type</span></span>                        | <span data-ttu-id="d8f3b-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-119">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d8f3b-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-120">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8f3b-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8f3b-121">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="d8f3b-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8f3b-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8f3b-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-123">Not supported.</span></span> |
| <span data-ttu-id="d8f3b-124">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="d8f3b-124">Application\*</span></span>                           | <span data-ttu-id="d8f3b-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8f3b-125">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="d8f3b-126">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-126">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8f3b-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8f3b-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/outcomes
```

## <a name="request-headers"></a><span data-ttu-id="d8f3b-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8f3b-128">Request headers</span></span>

| <span data-ttu-id="d8f3b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="d8f3b-129">Name</span></span>      |<span data-ttu-id="d8f3b-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d8f3b-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d8f3b-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8f3b-131">Authorization</span></span> | <span data-ttu-id="d8f3b-132">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d8f3b-132">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8f3b-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8f3b-133">Request body</span></span>

<span data-ttu-id="d8f3b-134">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8f3b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8f3b-135">Response</span></span>

<span data-ttu-id="d8f3b-136">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [educationOutcome](../resources/educationoutcome.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-136">If successful, this method returns a `200 OK` response code and a collection of [educationOutcome](../resources/educationoutcome.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8f3b-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="d8f3b-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8f3b-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8f3b-138">Request</span></span>

<span data-ttu-id="d8f3b-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d8f3b-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8f3b-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outcomes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/me/assignments/{id}/submissions/{id}/outcomes
```
# <a name="c"></a>[<span data-ttu-id="d8f3b-141">C#</span><span class="sxs-lookup"><span data-stu-id="d8f3b-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outcomes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8f3b-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8f3b-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outcomes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8f3b-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8f3b-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outcomes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8f3b-144">Java</span><span class="sxs-lookup"><span data-stu-id="d8f3b-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outcomes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d8f3b-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8f3b-145">Response</span></span>

<span data-ttu-id="d8f3b-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-146">The following is an example of the response.</span></span>

> <span data-ttu-id="d8f3b-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8f3b-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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


