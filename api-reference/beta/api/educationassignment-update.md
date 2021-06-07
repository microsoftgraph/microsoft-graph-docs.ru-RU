---
title: Обновление системы образования
description: Обновление объекта назначения. Это могут сделать только преподаватели в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы изменить состояние назначения, используйте действие публикации.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39f9f1a56fca07078b4be74447de563b7b7f8d31
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780773"
---
# <a name="update-educationassignment"></a><span data-ttu-id="42970-106">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="42970-106">Update educationassignment</span></span>

<span data-ttu-id="42970-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42970-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42970-108">Обновление объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="42970-108">Update the assignment object.</span></span> <span data-ttu-id="42970-109">Это могут сделать только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="42970-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="42970-110">Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="42970-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="42970-111">Чтобы [изменить](../api/educationassignment-publish.md) состояние назначения, используйте действие публикации.</span><span class="sxs-lookup"><span data-stu-id="42970-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="42970-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="42970-112">Permissions</span></span>
<span data-ttu-id="42970-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42970-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42970-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="42970-115">Permission type</span></span>      | <span data-ttu-id="42970-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="42970-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="42970-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="42970-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="42970-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="42970-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="42970-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="42970-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="42970-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42970-120">Not supported.</span></span>  |
|<span data-ttu-id="42970-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="42970-121">Application</span></span> | <span data-ttu-id="42970-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42970-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="42970-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="42970-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="42970-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="42970-124">Request headers</span></span>
| <span data-ttu-id="42970-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="42970-125">Header</span></span>       | <span data-ttu-id="42970-126">Значение</span><span class="sxs-lookup"><span data-stu-id="42970-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="42970-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="42970-127">Authorization</span></span>  | <span data-ttu-id="42970-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="42970-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="42970-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="42970-130">Content-Type</span></span>  | <span data-ttu-id="42970-131">application/json</span><span class="sxs-lookup"><span data-stu-id="42970-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="42970-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="42970-132">Request body</span></span>
<span data-ttu-id="42970-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="42970-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="42970-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="42970-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="42970-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="42970-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="42970-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="42970-136">Property</span></span>     | <span data-ttu-id="42970-137">Тип</span><span class="sxs-lookup"><span data-stu-id="42970-137">Type</span></span>   |<span data-ttu-id="42970-138">Описание</span><span class="sxs-lookup"><span data-stu-id="42970-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42970-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="42970-139">addedStudentAction</span></span>|<span data-ttu-id="42970-140">String</span><span class="sxs-lookup"><span data-stu-id="42970-140">String</span></span>| <span data-ttu-id="42970-141">Управление поведением учащихся, добавленных после публикации задания.</span><span class="sxs-lookup"><span data-stu-id="42970-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="42970-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="42970-142">allowLateSubmissions</span></span>|<span data-ttu-id="42970-143">Логический</span><span class="sxs-lookup"><span data-stu-id="42970-143">Boolean</span></span>| <span data-ttu-id="42970-144">Можно ли отправку представлений после даты.</span><span class="sxs-lookup"><span data-stu-id="42970-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="42970-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="42970-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="42970-146">Логический</span><span class="sxs-lookup"><span data-stu-id="42970-146">Boolean</span></span>| <span data-ttu-id="42970-147">Может ли учащийся добавлять ресурсы в отправку.</span><span class="sxs-lookup"><span data-stu-id="42970-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="42970-148">Указано, поступили ли из списка ресурсов назначения только элементы, указанные в представлении.</span><span class="sxs-lookup"><span data-stu-id="42970-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="42970-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="42970-149">assignDateTime</span></span>|<span data-ttu-id="42970-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42970-150">DateTimeOffset</span></span>| <span data-ttu-id="42970-151">Дата публикации назначения учащимся.</span><span class="sxs-lookup"><span data-stu-id="42970-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="42970-152">assignTo</span><span class="sxs-lookup"><span data-stu-id="42970-152">assignTo</span></span>|<span data-ttu-id="42970-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="42970-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="42970-154">Студенты, получаювшие назначение.</span><span class="sxs-lookup"><span data-stu-id="42970-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="42970-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="42970-155">closeDateTime</span></span>|<span data-ttu-id="42970-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42970-156">DateTimeOffset</span></span>| <span data-ttu-id="42970-157">Дата закрытия назначения для отправки.</span><span class="sxs-lookup"><span data-stu-id="42970-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="42970-158">Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="42970-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="42970-159">displayName</span><span class="sxs-lookup"><span data-stu-id="42970-159">displayName</span></span>|<span data-ttu-id="42970-160">String</span><span class="sxs-lookup"><span data-stu-id="42970-160">String</span></span>| <span data-ttu-id="42970-161">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="42970-161">Name of assignment.</span></span> |
|<span data-ttu-id="42970-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="42970-162">dueDateTime</span></span>|<span data-ttu-id="42970-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="42970-163">DateTimeOffset</span></span>| <span data-ttu-id="42970-164">Назначение даты должно быть.</span><span class="sxs-lookup"><span data-stu-id="42970-164">Date assignment is due.</span></span> |
|<span data-ttu-id="42970-165">классификация</span><span class="sxs-lookup"><span data-stu-id="42970-165">grading</span></span>|<span data-ttu-id="42970-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="42970-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="42970-167">Оценка назначения.</span><span class="sxs-lookup"><span data-stu-id="42970-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="42970-168">инструкции</span><span class="sxs-lookup"><span data-stu-id="42970-168">instructions</span></span>|<span data-ttu-id="42970-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="42970-169">itemBody</span></span>| <span data-ttu-id="42970-170">Инструкции, которые будут даны учащимся вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="42970-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="42970-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="42970-171">notificationChannelUrl</span></span>|<span data-ttu-id="42970-172">String</span><span class="sxs-lookup"><span data-stu-id="42970-172">String</span></span>| <span data-ttu-id="42970-173">Канал для публикации уведомления о публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="42970-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="42970-174">Обновление URL-адреса канала не допускается после публикации назначения и допускается только в том случае, если **значение assignTo** является [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="42970-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="42970-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="42970-175">Response</span></span>
<span data-ttu-id="42970-176">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="42970-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="42970-177">Пример</span><span class="sxs-lookup"><span data-stu-id="42970-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="42970-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="42970-178">Request</span></span>
<span data-ttu-id="42970-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="42970-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42970-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="42970-180">HTTP</span></span>](#tab/http)
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
  "dueDateTime": "2014-02-01T00:00:00Z",
  "addedStudentAction": "none",
  "addToCalendarAction": "studentsAndPublisher",
}
```
# <a name="c"></a>[<span data-ttu-id="42970-181">C#</span><span class="sxs-lookup"><span data-stu-id="42970-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42970-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42970-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42970-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42970-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42970-184">Java</span><span class="sxs-lookup"><span data-stu-id="42970-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="42970-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="42970-185">Response</span></span>
<span data-ttu-id="42970-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="42970-186">The following is an example of the response.</span></span> 

><span data-ttu-id="42970-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="42970-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "closeDateTime": "2014-02-11T00:00:00Z",
  "addToCalendarAction": "studentsAndPublisher",
  "dueDateTime": "2014-02-01T00:00:00Z",
  "assignDateTime": "2014-01-01T00:00:00Z",
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
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
  ]
}
-->


