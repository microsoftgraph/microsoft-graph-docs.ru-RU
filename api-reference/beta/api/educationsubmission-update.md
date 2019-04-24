---
title: Обновление educationsubmission
description: Добавьте оценку и обратную связь к отправке. Эту операцию могут выполнять только преподаватели. Обратите внимание на то, что основное разрешение не имеет доступа к свойствам уровня, поэтому не может выполнять запись для оценки или обратной связи. Это действие не приводит к выпуску оценки и обратной связи с студентом. Преподаватель должен принять явное действие по выпуску, чтобы данные оценки были возвращены студенту.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c420d2c6e512d8fed0d713340fea482b0888ca1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464852"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="4a9d0-107">Обновление educationsubmission</span><span class="sxs-lookup"><span data-stu-id="4a9d0-107">Update educationsubmission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a9d0-108">Добавьте оценку и обратную связь к отправке.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-108">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="4a9d0-109">Эту операцию могут выполнять только преподаватели.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-109">Only teachers can perform this operation.</span></span> <span data-ttu-id="4a9d0-110">Обратите внимание на то, что основное разрешение не имеет доступа к свойствам уровня, поэтому не может выполнять запись для оценки или обратной связи.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-110">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="4a9d0-111">Это действие не приводит к выпуску оценки и обратной связи с студентом.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-111">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="4a9d0-112">Преподаватель должен принять явное действие по выпуску, чтобы данные оценки были возвращены студенту.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-112">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a9d0-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a9d0-113">Permissions</span></span>
<span data-ttu-id="4a9d0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a9d0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a9d0-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a9d0-116">Permission type</span></span>      | <span data-ttu-id="4a9d0-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a9d0-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a9d0-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a9d0-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a9d0-119">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4a9d0-119">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4a9d0-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a9d0-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a9d0-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-121">Not supported.</span></span>   |
|<span data-ttu-id="4a9d0-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a9d0-122">Application</span></span> | <span data-ttu-id="4a9d0-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a9d0-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a9d0-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4a9d0-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a9d0-125">Request headers</span></span>
| <span data-ttu-id="4a9d0-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a9d0-126">Header</span></span>       | <span data-ttu-id="4a9d0-127">Значение</span><span class="sxs-lookup"><span data-stu-id="4a9d0-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a9d0-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a9d0-128">Authorization</span></span>  | <span data-ttu-id="4a9d0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a9d0-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a9d0-131">Request body</span></span>
<span data-ttu-id="4a9d0-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4a9d0-133">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4a9d0-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-134">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="4a9d0-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a9d0-135">Property</span></span>     | <span data-ttu-id="4a9d0-136">Тип</span><span class="sxs-lookup"><span data-stu-id="4a9d0-136">Type</span></span>   |<span data-ttu-id="4a9d0-137">Описание</span><span class="sxs-lookup"><span data-stu-id="4a9d0-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a9d0-138">замечания</span><span class="sxs-lookup"><span data-stu-id="4a9d0-138">feedback</span></span>|<span data-ttu-id="4a9d0-139">Едукатионфидбакк</span><span class="sxs-lookup"><span data-stu-id="4a9d0-139">educationFeedback</span></span>||
|<span data-ttu-id="4a9d0-140">оценка</span><span class="sxs-lookup"><span data-stu-id="4a9d0-140">grade</span></span>|<span data-ttu-id="4a9d0-141">Едукатионассигнментграде</span><span class="sxs-lookup"><span data-stu-id="4a9d0-141">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="4a9d0-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a9d0-142">Response</span></span>
<span data-ttu-id="4a9d0-143">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-143">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a9d0-144">Пример</span><span class="sxs-lookup"><span data-stu-id="4a9d0-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a9d0-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a9d0-145">Request</span></span>
<span data-ttu-id="4a9d0-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationsubmission"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7
Content-type: application/json
Content-length: 658

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
      "gradedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
      "@odata.type": "microsoft.graph.identitySet"
    },
    "gradedDateTime": "2014-01-01T00:00:00Z",
    "@odata.type": "microsoft.graph.educationAssignmentGrade"
  }
}
```
##### <a name="response"></a><span data-ttu-id="4a9d0-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a9d0-147">Response</span></span>
<span data-ttu-id="4a9d0-148">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-148">The following is an example of the response.</span></span> 

><span data-ttu-id="4a9d0-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4a9d0-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1217

{
  "feedback": {
    "text": {
      "content": "Good work!",
      "contentType": "Text"
    },
    "feedbackDateTime": "2014-01-01T00:00:00Z",
    "feedbackBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      }
    },
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "grade": {
         "gradedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
          "@odata.type": "microsoft.graph.identitySet"
        },
        "gradedDateTime": "2014-01-01T00:00:00Z",
        "@odata.type": "microsoft.graph.educationAssignmentGrade"
  },
  "id": "850f51b7",
  "recipient": {
    userId:"dsfewsddf",
    "@odata.type": "#microsoft.graph.educationSubmissionRecipient"
  },
  "releasedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "releasedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "String",
  "status": "completed",
  "submittedBy": {
    "user": {
      "displayName": "Susana Rocha",
      "id": "14012"
    },
  },
  "submittedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmission-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
