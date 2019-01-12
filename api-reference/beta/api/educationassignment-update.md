---
title: Обновление educationassignment
description: Обновите объект назначения. Это можно сделать только преподавателей в классе. Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения. Используется для изменения состояния назначения действие опубликовать.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: f8d79e11628e3a02a20c9ecdcd46bcd1bff05e7f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960352"
---
# <a name="update-educationassignment"></a><span data-ttu-id="d630b-106">Обновление educationassignment</span><span class="sxs-lookup"><span data-stu-id="d630b-106">Update educationassignment</span></span>

> <span data-ttu-id="d630b-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d630b-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d630b-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d630b-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d630b-109">Обновите объект назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-109">Update the assignment object.</span></span> <span data-ttu-id="d630b-110">Это можно сделать только преподавателей в классе.</span><span class="sxs-lookup"><span data-stu-id="d630b-110">Only teachers in the class can do this.</span></span> <span data-ttu-id="d630b-111">Обратите внимание на то, что запрос на исправление нельзя использовать для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-111">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="d630b-112">Используется для изменения состояния назначения действие [Опубликовать](../api/educationassignment-publish.md) .</span><span class="sxs-lookup"><span data-stu-id="d630b-112">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="d630b-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d630b-113">Permissions</span></span>
<span data-ttu-id="d630b-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d630b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d630b-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d630b-116">Permission type</span></span>      | <span data-ttu-id="d630b-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d630b-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d630b-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d630b-118">Delegated (work or school account)</span></span> |  <span data-ttu-id="d630b-119">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d630b-119">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d630b-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d630b-120">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d630b-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d630b-121">Not supported.</span></span>  |
|<span data-ttu-id="d630b-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d630b-122">Application</span></span> | <span data-ttu-id="d630b-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d630b-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d630b-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d630b-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d630b-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d630b-125">Request headers</span></span>
| <span data-ttu-id="d630b-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d630b-126">Header</span></span>       | <span data-ttu-id="d630b-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d630b-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d630b-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d630b-128">Authorization</span></span>  | <span data-ttu-id="d630b-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d630b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d630b-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d630b-131">Content-Type</span></span>  | <span data-ttu-id="d630b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="d630b-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d630b-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d630b-133">Request body</span></span>
<span data-ttu-id="d630b-134">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="d630b-134">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="d630b-135">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="d630b-135">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d630b-136">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="d630b-136">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d630b-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="d630b-137">Property</span></span>     | <span data-ttu-id="d630b-138">Тип</span><span class="sxs-lookup"><span data-stu-id="d630b-138">Type</span></span>   |<span data-ttu-id="d630b-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d630b-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d630b-140">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="d630b-140">allowLateSubmissions</span></span>|<span data-ttu-id="d630b-141">Логический</span><span class="sxs-lookup"><span data-stu-id="d630b-141">Boolean</span></span>| <span data-ttu-id="d630b-142">Является ли отправленные данные можно отправлять после даты выполнения.</span><span class="sxs-lookup"><span data-stu-id="d630b-142">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="d630b-143">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="d630b-143">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="d630b-144">Логический</span><span class="sxs-lookup"><span data-stu-id="d630b-144">Boolean</span></span>| <span data-ttu-id="d630b-145">Является ли студента можно добавить ресурсы для отправки.</span><span class="sxs-lookup"><span data-stu-id="d630b-145">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="d630b-146">Указывает, является ли только элементов на отправку поступил из списка назначений ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d630b-146">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="d630b-147">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="d630b-147">assignDateTime</span></span>|<span data-ttu-id="d630b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d630b-148">DateTimeOffset</span></span>| <span data-ttu-id="d630b-149">Дата назначения должны быть опубликованы для студентов.</span><span class="sxs-lookup"><span data-stu-id="d630b-149">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="d630b-150">assignTo</span><span class="sxs-lookup"><span data-stu-id="d630b-150">assignTo</span></span>|<span data-ttu-id="d630b-151">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="d630b-151">educationAssignmentRecipient</span></span>| <span data-ttu-id="d630b-152">Студентов, получение назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-152">Students who get the assignment.</span></span>|
|<span data-ttu-id="d630b-153">displayName</span><span class="sxs-lookup"><span data-stu-id="d630b-153">displayName</span></span>|<span data-ttu-id="d630b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="d630b-154">String</span></span>| <span data-ttu-id="d630b-155">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-155">Name of assignment.</span></span> |
|<span data-ttu-id="d630b-156">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="d630b-156">dueDateTime</span></span>|<span data-ttu-id="d630b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d630b-157">DateTimeOffset</span></span>| <span data-ttu-id="d630b-158">Дата назначения должно быть выполнено.</span><span class="sxs-lookup"><span data-stu-id="d630b-158">Date assignment is due.</span></span> |
|<span data-ttu-id="d630b-159">Оценка успеваемости</span><span class="sxs-lookup"><span data-stu-id="d630b-159">grading</span></span>|<span data-ttu-id="d630b-160">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="d630b-160">educationAssignmentGradeType</span></span>| <span data-ttu-id="d630b-161">Как будет выражаемым числом назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-161">How the assignment will be graded.</span></span>|
|<span data-ttu-id="d630b-162">инструкции</span><span class="sxs-lookup"><span data-stu-id="d630b-162">instructions</span></span>|<span data-ttu-id="d630b-163">itemBody</span><span class="sxs-lookup"><span data-stu-id="d630b-163">itemBody</span></span>| <span data-ttu-id="d630b-164">Инструкции для студентов, а также назначения.</span><span class="sxs-lookup"><span data-stu-id="d630b-164">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="d630b-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="d630b-165">Response</span></span>
<span data-ttu-id="d630b-166">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [educationAssignment](../resources/educationassignment.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d630b-166">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d630b-167">Пример</span><span class="sxs-lookup"><span data-stu-id="d630b-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d630b-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="d630b-168">Request</span></span>
<span data-ttu-id="d630b-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d630b-169">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="d630b-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="d630b-170">Response</span></span>
<span data-ttu-id="d630b-171">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d630b-171">The following is an example of the response.</span></span> 

><span data-ttu-id="d630b-172">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d630b-172">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d630b-173">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d630b-173">All of the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
