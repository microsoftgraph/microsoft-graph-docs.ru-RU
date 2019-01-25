---
title: Обновление educationassignment
description: Обновите объект назначения. Это можно сделать только преподавателей в классе. Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения. Используется для изменения состояния назначения действие опубликовать.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb5762f86e1572f9a9d5876199c945154a25293b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524963"
---
# <a name="update-educationassignment"></a><span data-ttu-id="e0cbe-106">Обновление educationassignment</span><span class="sxs-lookup"><span data-stu-id="e0cbe-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0cbe-107">Обновите объект назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-107">Update the assignment object.</span></span> <span data-ttu-id="e0cbe-108">Это можно сделать только преподавателей в классе.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="e0cbe-109">Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="e0cbe-110">Используется для изменения состояния назначения действие [Опубликовать](../api/educationassignment-publish.md) .</span><span class="sxs-lookup"><span data-stu-id="e0cbe-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0cbe-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0cbe-111">Permissions</span></span>
<span data-ttu-id="e0cbe-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0cbe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0cbe-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0cbe-114">Permission type</span></span>      | <span data-ttu-id="e0cbe-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0cbe-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0cbe-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0cbe-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0cbe-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0cbe-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e0cbe-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0cbe-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0cbe-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-119">Not supported.</span></span>  |
|<span data-ttu-id="e0cbe-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0cbe-120">Application</span></span> | <span data-ttu-id="e0cbe-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e0cbe-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0cbe-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e0cbe-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0cbe-123">Request headers</span></span>
| <span data-ttu-id="e0cbe-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0cbe-124">Header</span></span>       | <span data-ttu-id="e0cbe-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e0cbe-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0cbe-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0cbe-126">Authorization</span></span>  | <span data-ttu-id="e0cbe-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e0cbe-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e0cbe-129">Content-Type</span></span>  | <span data-ttu-id="e0cbe-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e0cbe-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0cbe-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e0cbe-131">Request body</span></span>
<span data-ttu-id="e0cbe-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e0cbe-133">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e0cbe-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e0cbe-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0cbe-135">Property</span></span>     | <span data-ttu-id="e0cbe-136">Тип</span><span class="sxs-lookup"><span data-stu-id="e0cbe-136">Type</span></span>   |<span data-ttu-id="e0cbe-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e0cbe-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0cbe-138">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="e0cbe-138">allowLateSubmissions</span></span>|<span data-ttu-id="e0cbe-139">Логическое</span><span class="sxs-lookup"><span data-stu-id="e0cbe-139">Boolean</span></span>| <span data-ttu-id="e0cbe-140">Является ли отправленные данные можно отправлять после даты выполнения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="e0cbe-141">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="e0cbe-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="e0cbe-142">Логическое</span><span class="sxs-lookup"><span data-stu-id="e0cbe-142">Boolean</span></span>| <span data-ttu-id="e0cbe-143">Является ли студента можно добавить ресурсы для отправки.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="e0cbe-144">Указывает, является ли только элементов на отправку поступил из списка назначений ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="e0cbe-145">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="e0cbe-145">assignDateTime</span></span>|<span data-ttu-id="e0cbe-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0cbe-146">DateTimeOffset</span></span>| <span data-ttu-id="e0cbe-147">Дата назначения должны быть опубликованы для студентов.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="e0cbe-148">assignTo</span><span class="sxs-lookup"><span data-stu-id="e0cbe-148">assignTo</span></span>|<span data-ttu-id="e0cbe-149">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="e0cbe-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="e0cbe-150">Студентов, получение назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="e0cbe-151">displayName</span><span class="sxs-lookup"><span data-stu-id="e0cbe-151">displayName</span></span>|<span data-ttu-id="e0cbe-152">String</span><span class="sxs-lookup"><span data-stu-id="e0cbe-152">String</span></span>| <span data-ttu-id="e0cbe-153">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-153">Name of assignment.</span></span> |
|<span data-ttu-id="e0cbe-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="e0cbe-154">dueDateTime</span></span>|<span data-ttu-id="e0cbe-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0cbe-155">DateTimeOffset</span></span>| <span data-ttu-id="e0cbe-156">Дата назначения должно быть выполнено.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-156">Date assignment is due.</span></span> |
|<span data-ttu-id="e0cbe-157">Оценка успеваемости</span><span class="sxs-lookup"><span data-stu-id="e0cbe-157">grading</span></span>|<span data-ttu-id="e0cbe-158">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="e0cbe-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="e0cbe-159">Как будет выражаемым числом назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="e0cbe-160">Инструкции</span><span class="sxs-lookup"><span data-stu-id="e0cbe-160">instructions</span></span>|<span data-ttu-id="e0cbe-161">item.body</span><span class="sxs-lookup"><span data-stu-id="e0cbe-161">itemBody</span></span>| <span data-ttu-id="e0cbe-162">Инструкции для студентов, а также назначения.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="e0cbe-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0cbe-163">Response</span></span>
<span data-ttu-id="e0cbe-164">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationAssignment](../resources/educationassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e0cbe-165">Пример</span><span class="sxs-lookup"><span data-stu-id="e0cbe-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0cbe-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0cbe-166">Request</span></span>
<span data-ttu-id="e0cbe-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-167">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002
Content-type: application/json
Content-length: 279

{
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z"
}
```
##### <a name="response"></a><span data-ttu-id="e0cbe-168">Ответ</span><span class="sxs-lookup"><span data-stu-id="e0cbe-168">Response</span></span>
<span data-ttu-id="e0cbe-169">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-169">The following is an example of the response.</span></span> 

><span data-ttu-id="e0cbe-170">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-170">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e0cbe-171">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0cbe-171">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "classId": "11021",
  "displayName": "Week 1 reading assignment",
  "instructions": {
    "contentType": "Text",
    "content": "Read chapters 1 through 3"
  },
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
