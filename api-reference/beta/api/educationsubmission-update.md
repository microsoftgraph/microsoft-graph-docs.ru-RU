---
title: Обновление educationsubmission
description: Добавьте марки и свои отзывы и предложения для отправки. Только учителя можно выполнить эту операцию. Обратите внимание на то, не имеет доступа к свойствам марки основные разрешения и поэтому не могут выполнять запись марки или свои отзывы и предложения. Это действие не освобождает марки и свои отзывы и предложения для учащихся. Преподаватель должен выполнить действие явные выпуска для данных марки должно быть возвращено для студента.
author: dipakboyed
localization_priority: Normal
ms.openlocfilehash: 516940f9a6dd43460aa0ceb9b955c41dc89196c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828786"
---
# <a name="update-educationsubmission"></a><span data-ttu-id="2dbe8-107">Обновление educationsubmission</span><span class="sxs-lookup"><span data-stu-id="2dbe8-107">Update educationsubmission</span></span>

> <span data-ttu-id="2dbe8-108">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2dbe8-109">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2dbe8-110">Добавьте марки и свои отзывы и предложения для отправки.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-110">Add a grade and feedback to a submission.</span></span> <span data-ttu-id="2dbe8-111">Только учителя можно выполнить эту операцию.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-111">Only teachers can perform this operation.</span></span> <span data-ttu-id="2dbe8-112">Обратите внимание на то, не имеет доступа к свойствам марки основные разрешения и поэтому не могут выполнять запись марки или свои отзывы и предложения.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-112">Note that the Basic permission does not have access to the grade properties, and therefore cannot write to grade or feedback.</span></span> <span data-ttu-id="2dbe8-113">Это действие не освобождает марки и свои отзывы и предложения для учащихся.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-113">This action does not release the grade and feedback to the student.</span></span> <span data-ttu-id="2dbe8-114">Преподаватель должен выполнить действие явные выпуска для данных марки должно быть возвращено для студента.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-114">A teacher must take an explicit release action for the grade data to be returned to the student.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dbe8-115">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2dbe8-115">Permissions</span></span>
<span data-ttu-id="2dbe8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dbe8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dbe8-118">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2dbe8-118">Permission type</span></span>      | <span data-ttu-id="2dbe8-119">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2dbe8-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dbe8-120">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2dbe8-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="2dbe8-121">EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2dbe8-121">EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2dbe8-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2dbe8-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dbe8-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-123">Not supported.</span></span>   |
|<span data-ttu-id="2dbe8-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2dbe8-124">Application</span></span> | <span data-ttu-id="2dbe8-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2dbe8-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2dbe8-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/submissions/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2dbe8-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2dbe8-127">Request headers</span></span>
| <span data-ttu-id="2dbe8-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2dbe8-128">Header</span></span>       | <span data-ttu-id="2dbe8-129">Значение</span><span class="sxs-lookup"><span data-stu-id="2dbe8-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2dbe8-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2dbe8-130">Authorization</span></span>  | <span data-ttu-id="2dbe8-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2dbe8-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2dbe8-133">Request body</span></span>
<span data-ttu-id="2dbe8-134">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="2dbe8-135">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="2dbe8-136">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-136">For best performance, don't include existing values that haven't changed.</span></span>

<!-- Provide the property descriptions. -->

| <span data-ttu-id="2dbe8-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dbe8-137">Property</span></span>     | <span data-ttu-id="2dbe8-138">Тип</span><span class="sxs-lookup"><span data-stu-id="2dbe8-138">Type</span></span>   |<span data-ttu-id="2dbe8-139">Описание</span><span class="sxs-lookup"><span data-stu-id="2dbe8-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dbe8-140">свои отзывы и предложения</span><span class="sxs-lookup"><span data-stu-id="2dbe8-140">feedback</span></span>|<span data-ttu-id="2dbe8-141">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="2dbe8-141">educationFeedback</span></span>||
|<span data-ttu-id="2dbe8-142">оценка</span><span class="sxs-lookup"><span data-stu-id="2dbe8-142">grade</span></span>|<span data-ttu-id="2dbe8-143">educationAssignmentGrade</span><span class="sxs-lookup"><span data-stu-id="2dbe8-143">educationAssignmentGrade</span></span>||

## <a name="response"></a><span data-ttu-id="2dbe8-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="2dbe8-144">Response</span></span>
<span data-ttu-id="2dbe8-145">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationSubmission](../resources/educationsubmission.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-145">If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2dbe8-146">Пример</span><span class="sxs-lookup"><span data-stu-id="2dbe8-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2dbe8-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="2dbe8-147">Request</span></span>
<span data-ttu-id="2dbe8-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-148">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2dbe8-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="2dbe8-149">Response</span></span>
<span data-ttu-id="2dbe8-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-150">The following is an example of the response.</span></span> 

><span data-ttu-id="2dbe8-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2dbe8-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationsubmission",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
