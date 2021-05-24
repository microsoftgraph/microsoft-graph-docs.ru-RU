---
title: Обновление системы образования
description: Обновление объекта назначения. Это могут сделать только преподаватели в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы изменить состояние назначения, используйте действие публикации.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcaed5b3c73039aeac6c1861a8b1ddcd4e5f19d8
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629207"
---
# <a name="update-educationassignment"></a><span data-ttu-id="5607a-106">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="5607a-106">Update educationassignment</span></span>

<span data-ttu-id="5607a-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5607a-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5607a-108">Обновление объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="5607a-108">Update the assignment object.</span></span> <span data-ttu-id="5607a-109">Это могут сделать только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="5607a-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="5607a-110">Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="5607a-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="5607a-111">Чтобы [изменить](../api/educationassignment-publish.md) состояние назначения, используйте действие публикации.</span><span class="sxs-lookup"><span data-stu-id="5607a-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="5607a-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5607a-112">Permissions</span></span>
<span data-ttu-id="5607a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5607a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5607a-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5607a-115">Permission type</span></span>      | <span data-ttu-id="5607a-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5607a-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5607a-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5607a-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="5607a-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5607a-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5607a-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5607a-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5607a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5607a-120">Not supported.</span></span>  |
|<span data-ttu-id="5607a-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5607a-121">Application</span></span> | <span data-ttu-id="5607a-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5607a-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5607a-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5607a-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5607a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5607a-124">Request headers</span></span>
| <span data-ttu-id="5607a-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5607a-125">Header</span></span>       | <span data-ttu-id="5607a-126">Значение</span><span class="sxs-lookup"><span data-stu-id="5607a-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5607a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5607a-127">Authorization</span></span>  | <span data-ttu-id="5607a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5607a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5607a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5607a-130">Content-Type</span></span>  | <span data-ttu-id="5607a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="5607a-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5607a-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5607a-132">Request body</span></span>
<span data-ttu-id="5607a-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="5607a-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5607a-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="5607a-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5607a-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5607a-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5607a-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="5607a-136">Property</span></span>     | <span data-ttu-id="5607a-137">Тип</span><span class="sxs-lookup"><span data-stu-id="5607a-137">Type</span></span>   |<span data-ttu-id="5607a-138">Описание</span><span class="sxs-lookup"><span data-stu-id="5607a-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5607a-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="5607a-139">addedStudentAction</span></span>|<span data-ttu-id="5607a-140">Строка</span><span class="sxs-lookup"><span data-stu-id="5607a-140">String</span></span>| <span data-ttu-id="5607a-141">Управление поведением учащихся, добавленных после публикации задания.</span><span class="sxs-lookup"><span data-stu-id="5607a-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="5607a-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="5607a-142">allowLateSubmissions</span></span>|<span data-ttu-id="5607a-143">Логический</span><span class="sxs-lookup"><span data-stu-id="5607a-143">Boolean</span></span>| <span data-ttu-id="5607a-144">Можно ли отправку представлений после даты.</span><span class="sxs-lookup"><span data-stu-id="5607a-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="5607a-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="5607a-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="5607a-146">Логический</span><span class="sxs-lookup"><span data-stu-id="5607a-146">Boolean</span></span>| <span data-ttu-id="5607a-147">Может ли учащийся добавлять ресурсы в отправку.</span><span class="sxs-lookup"><span data-stu-id="5607a-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="5607a-148">Указано, поступили ли из списка ресурсов назначения только элементы, указанные в представлении.</span><span class="sxs-lookup"><span data-stu-id="5607a-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="5607a-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="5607a-149">assignDateTime</span></span>|<span data-ttu-id="5607a-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5607a-150">DateTimeOffset</span></span>| <span data-ttu-id="5607a-151">Дата публикации назначения учащимся.</span><span class="sxs-lookup"><span data-stu-id="5607a-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="5607a-152">assignTo</span><span class="sxs-lookup"><span data-stu-id="5607a-152">assignTo</span></span>|<span data-ttu-id="5607a-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="5607a-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="5607a-154">Студенты, получаювшие назначение.</span><span class="sxs-lookup"><span data-stu-id="5607a-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="5607a-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="5607a-155">closeDateTime</span></span>|<span data-ttu-id="5607a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5607a-156">DateTimeOffset</span></span>| <span data-ttu-id="5607a-157">Дата закрытия назначения для отправки.</span><span class="sxs-lookup"><span data-stu-id="5607a-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="5607a-158">Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="5607a-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="5607a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="5607a-159">displayName</span></span>|<span data-ttu-id="5607a-160">Строка</span><span class="sxs-lookup"><span data-stu-id="5607a-160">String</span></span>| <span data-ttu-id="5607a-161">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="5607a-161">Name of assignment.</span></span> |
|<span data-ttu-id="5607a-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="5607a-162">dueDateTime</span></span>|<span data-ttu-id="5607a-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5607a-163">DateTimeOffset</span></span>| <span data-ttu-id="5607a-164">Назначение даты должно быть.</span><span class="sxs-lookup"><span data-stu-id="5607a-164">Date assignment is due.</span></span> |
|<span data-ttu-id="5607a-165">классификация</span><span class="sxs-lookup"><span data-stu-id="5607a-165">grading</span></span>|<span data-ttu-id="5607a-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="5607a-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="5607a-167">Оценка назначения.</span><span class="sxs-lookup"><span data-stu-id="5607a-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="5607a-168">инструкции</span><span class="sxs-lookup"><span data-stu-id="5607a-168">instructions</span></span>|<span data-ttu-id="5607a-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="5607a-169">itemBody</span></span>| <span data-ttu-id="5607a-170">Инструкции, которые будут даны учащимся вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="5607a-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="5607a-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="5607a-171">notificationChannelUrl</span></span>|<span data-ttu-id="5607a-172">Строка</span><span class="sxs-lookup"><span data-stu-id="5607a-172">String</span></span>| <span data-ttu-id="5607a-173">Канал для публикации уведомления о публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="5607a-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="5607a-174">Обновление URL-адреса канала не допускается после публикации назначения и допускается только в том случае, если **значение assignTo** является [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="5607a-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="5607a-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="5607a-175">Response</span></span>
<span data-ttu-id="5607a-176">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5607a-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5607a-177">Пример</span><span class="sxs-lookup"><span data-stu-id="5607a-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="5607a-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="5607a-178">Request</span></span>
<span data-ttu-id="5607a-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5607a-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5607a-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="5607a-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5607a-181">C#</span><span class="sxs-lookup"><span data-stu-id="5607a-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5607a-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5607a-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5607a-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5607a-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5607a-184">Java</span><span class="sxs-lookup"><span data-stu-id="5607a-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5607a-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="5607a-185">Response</span></span>
<span data-ttu-id="5607a-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5607a-186">The following is an example of the response.</span></span> 

><span data-ttu-id="5607a-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5607a-187">**Note:** The response object shown here might be shortened for readability.</span></span>

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


