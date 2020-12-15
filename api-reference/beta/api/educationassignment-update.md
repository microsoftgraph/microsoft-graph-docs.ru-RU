---
title: Обновление educationassignment
description: Обновление объекта назначения. Это могут делать только преподаватели в классе. Обратите внимание, что нельзя использовать запрос PATCH для изменения состояния назначения. Используйте действие публикации, чтобы изменить состояние назначения.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d0f0f965eece0d7998769e72afe58b56c7acd159
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49676005"
---
# <a name="update-educationassignment"></a><span data-ttu-id="18661-106">Обновление educationassignment</span><span class="sxs-lookup"><span data-stu-id="18661-106">Update educationassignment</span></span>

<span data-ttu-id="18661-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18661-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18661-108">Обновление объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-108">Update the assignment object.</span></span> <span data-ttu-id="18661-109">Это могут делать только преподаватели в классе.</span><span class="sxs-lookup"><span data-stu-id="18661-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="18661-110">Обратите внимание, что нельзя использовать запрос PATCH для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="18661-111">Используйте действие [публикации,](../api/educationassignment-publish.md) чтобы изменить состояние назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="18661-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="18661-112">Permissions</span></span>
<span data-ttu-id="18661-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18661-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18661-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="18661-115">Permission type</span></span>      | <span data-ttu-id="18661-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="18661-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="18661-117">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="18661-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="18661-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="18661-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="18661-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="18661-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="18661-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18661-120">Not supported.</span></span>  |
|<span data-ttu-id="18661-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="18661-121">Application</span></span> | <span data-ttu-id="18661-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18661-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="18661-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="18661-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="18661-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="18661-124">Request headers</span></span>
| <span data-ttu-id="18661-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="18661-125">Header</span></span>       | <span data-ttu-id="18661-126">Значение</span><span class="sxs-lookup"><span data-stu-id="18661-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="18661-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="18661-127">Authorization</span></span>  | <span data-ttu-id="18661-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="18661-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="18661-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="18661-130">Content-Type</span></span>  | <span data-ttu-id="18661-131">application/json</span><span class="sxs-lookup"><span data-stu-id="18661-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="18661-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="18661-132">Request body</span></span>
<span data-ttu-id="18661-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="18661-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="18661-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="18661-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="18661-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="18661-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="18661-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="18661-136">Property</span></span>     | <span data-ttu-id="18661-137">Тип</span><span class="sxs-lookup"><span data-stu-id="18661-137">Type</span></span>   |<span data-ttu-id="18661-138">Описание</span><span class="sxs-lookup"><span data-stu-id="18661-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18661-139">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="18661-139">addedStudentAction</span></span>|<span data-ttu-id="18661-140">String</span><span class="sxs-lookup"><span data-stu-id="18661-140">String</span></span>| <span data-ttu-id="18661-141">Управляет поведением учащихся, добавляемого после публикации задания.</span><span class="sxs-lookup"><span data-stu-id="18661-141">Controls the behavior for students who are added after the assignment is published.</span></span>|
|<span data-ttu-id="18661-142">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="18661-142">allowLateSubmissions</span></span>|<span data-ttu-id="18661-143">Логический</span><span class="sxs-lookup"><span data-stu-id="18661-143">Boolean</span></span>| <span data-ttu-id="18661-144">Может ли отправка отправки после даты окончания срока действия.</span><span class="sxs-lookup"><span data-stu-id="18661-144">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="18661-145">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="18661-145">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="18661-146">Логический</span><span class="sxs-lookup"><span data-stu-id="18661-146">Boolean</span></span>| <span data-ttu-id="18661-147">Может ли учащийся добавлять ресурсы в отправку.</span><span class="sxs-lookup"><span data-stu-id="18661-147">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="18661-148">Указывает, поступили ли из списка ресурсов назначения только элементы в отправке.</span><span class="sxs-lookup"><span data-stu-id="18661-148">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="18661-149">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="18661-149">assignDateTime</span></span>|<span data-ttu-id="18661-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18661-150">DateTimeOffset</span></span>| <span data-ttu-id="18661-151">Дата публикации задания учащимся.</span><span class="sxs-lookup"><span data-stu-id="18661-151">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="18661-152">assignTo</span><span class="sxs-lookup"><span data-stu-id="18661-152">assignTo</span></span>|<span data-ttu-id="18661-153">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="18661-153">educationAssignmentRecipient</span></span>| <span data-ttu-id="18661-154">Учащиеся, которые получают назначение.</span><span class="sxs-lookup"><span data-stu-id="18661-154">Students who get the assignment.</span></span>|
|<span data-ttu-id="18661-155">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="18661-155">closeDateTime</span></span>|<span data-ttu-id="18661-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18661-156">DateTimeOffset</span></span>| <span data-ttu-id="18661-157">Дата закрытия назначения для отправки.</span><span class="sxs-lookup"><span data-stu-id="18661-157">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="18661-158">Это необязательное поле, которое может иметь null, если назначение не разрешаетLateSubmissions или closeDateTime такое же, как dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="18661-158">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="18661-159">displayName</span><span class="sxs-lookup"><span data-stu-id="18661-159">displayName</span></span>|<span data-ttu-id="18661-160">String</span><span class="sxs-lookup"><span data-stu-id="18661-160">String</span></span>| <span data-ttu-id="18661-161">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-161">Name of assignment.</span></span> |
|<span data-ttu-id="18661-162">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="18661-162">dueDateTime</span></span>|<span data-ttu-id="18661-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18661-163">DateTimeOffset</span></span>| <span data-ttu-id="18661-164">Дата назначения должна быть.</span><span class="sxs-lookup"><span data-stu-id="18661-164">Date assignment is due.</span></span> |
|<span data-ttu-id="18661-165">grading</span><span class="sxs-lookup"><span data-stu-id="18661-165">grading</span></span>|<span data-ttu-id="18661-166">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="18661-166">educationAssignmentGradeType</span></span>| <span data-ttu-id="18661-167">Как будет оклассовка назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-167">How the assignment will be graded.</span></span>|
|<span data-ttu-id="18661-168">инструкции</span><span class="sxs-lookup"><span data-stu-id="18661-168">instructions</span></span>|<span data-ttu-id="18661-169">itemBody</span><span class="sxs-lookup"><span data-stu-id="18661-169">itemBody</span></span>| <span data-ttu-id="18661-170">Инструкции, которые необходимо дать учащимся вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="18661-170">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="18661-171">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="18661-171">notificationChannelUrl</span></span>|<span data-ttu-id="18661-172">String</span><span class="sxs-lookup"><span data-stu-id="18661-172">String</span></span>| <span data-ttu-id="18661-173">Канал для публикации уведомления о публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="18661-173">Channel to post assignment publish notification.</span></span> <span data-ttu-id="18661-174">Обновление URL-адреса канала запрещено после публикации назначения и допускается, только если значение **assignTo** — [educationAssignmentClassRecipient.](../resources/educationassignmentclassrecipient.md)</span><span class="sxs-lookup"><span data-stu-id="18661-174">Updating the channel URL is not allowed after the assignment has been published and is only allowed when the **assignTo** value is [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span>|

## <a name="response"></a><span data-ttu-id="18661-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="18661-175">Response</span></span>
<span data-ttu-id="18661-176">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="18661-176">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="18661-177">Пример</span><span class="sxs-lookup"><span data-stu-id="18661-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="18661-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="18661-178">Request</span></span>
<span data-ttu-id="18661-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="18661-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18661-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="18661-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="18661-181">C#</span><span class="sxs-lookup"><span data-stu-id="18661-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18661-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18661-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18661-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18661-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18661-184">Java</span><span class="sxs-lookup"><span data-stu-id="18661-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="18661-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="18661-185">Response</span></span>
<span data-ttu-id="18661-186">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="18661-186">The following is an example of the response.</span></span> 

><span data-ttu-id="18661-187">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18661-187">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="18661-188">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="18661-188">All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->


