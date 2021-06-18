---
title: Обновление системы образования
description: Обновление объекта educationAssigment.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dcfd47deabe9f711bbbbca59c7c7c4b23651f3d3
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993555"
---
# <a name="update-educationassignment"></a><span data-ttu-id="319a2-103">Обновление системы образования</span><span class="sxs-lookup"><span data-stu-id="319a2-103">Update educationassignment</span></span>

<span data-ttu-id="319a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="319a2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="319a2-105">Обновление объекта educationAssigment.</span><span class="sxs-lookup"><span data-stu-id="319a2-105">Update an educationAssigment object.</span></span> 

<span data-ttu-id="319a2-106">Выполнить это действие могут только преподаватели.</span><span class="sxs-lookup"><span data-stu-id="319a2-106">Only teachers can perform this action.</span></span> 

<span data-ttu-id="319a2-107">Кроме того, запрос на изменение состояния назначения с помощью действия [публикации.](../api/educationassignment-publish.md)</span><span class="sxs-lookup"><span data-stu-id="319a2-107">Alternatively, request to change the status of an assignment with [publish](../api/educationassignment-publish.md) action.</span></span> <span data-ttu-id="319a2-108">Для этого не используйте операцию PATCH.</span><span class="sxs-lookup"><span data-stu-id="319a2-108">Don't use a PATCH operation for this purpose.</span></span>

## <a name="permissions"></a><span data-ttu-id="319a2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="319a2-109">Permissions</span></span>
<span data-ttu-id="319a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="319a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="319a2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="319a2-112">Permission type</span></span>      | <span data-ttu-id="319a2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="319a2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="319a2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="319a2-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="319a2-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="319a2-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="319a2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="319a2-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="319a2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="319a2-117">Not supported.</span></span>  |
|<span data-ttu-id="319a2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="319a2-118">Application</span></span> | <span data-ttu-id="319a2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="319a2-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="319a2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="319a2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="request-headers"></a><span data-ttu-id="319a2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="319a2-121">Request headers</span></span>
| <span data-ttu-id="319a2-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="319a2-122">Header</span></span>       | <span data-ttu-id="319a2-123">Значение</span><span class="sxs-lookup"><span data-stu-id="319a2-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="319a2-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="319a2-124">Authorization</span></span>  | <span data-ttu-id="319a2-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="319a2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="319a2-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="319a2-127">Content-Type</span></span>  | <span data-ttu-id="319a2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="319a2-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="319a2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="319a2-129">Request body</span></span>
<span data-ttu-id="319a2-130">В теле запроса поставляют только значения полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="319a2-130">In the request body, supply only the values of the fields you want to update.</span></span> 

<span data-ttu-id="319a2-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="319a2-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="319a2-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="319a2-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="319a2-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="319a2-133">Property</span></span>     | <span data-ttu-id="319a2-134">Тип</span><span class="sxs-lookup"><span data-stu-id="319a2-134">Type</span></span>   |<span data-ttu-id="319a2-135">Описание</span><span class="sxs-lookup"><span data-stu-id="319a2-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="319a2-136">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="319a2-136">addedStudentAction</span></span>|<span data-ttu-id="319a2-137">String</span><span class="sxs-lookup"><span data-stu-id="319a2-137">String</span></span>| <span data-ttu-id="319a2-138">Описывает, следует ли распределять назначение среди учащихся, добавленных после даты публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="319a2-138">Describes if the assignment should be distributed to students who are added after the assignment publication date.</span></span>|
|<span data-ttu-id="319a2-139">allowLateSubmissions</span><span class="sxs-lookup"><span data-stu-id="319a2-139">allowLateSubmissions</span></span>|<span data-ttu-id="319a2-140">Логический</span><span class="sxs-lookup"><span data-stu-id="319a2-140">Boolean</span></span>| <span data-ttu-id="319a2-141">Могут ли студенты отправлять отправку после срока.</span><span class="sxs-lookup"><span data-stu-id="319a2-141">Whether students can send submission after the due date.</span></span>|
|<span data-ttu-id="319a2-142">allowStudentsToAddResourcesToSubmission</span><span class="sxs-lookup"><span data-stu-id="319a2-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="319a2-143">Логический</span><span class="sxs-lookup"><span data-stu-id="319a2-143">Boolean</span></span>| <span data-ttu-id="319a2-144">Может ли студент добавлять ресурсы в отправку или нет.</span><span class="sxs-lookup"><span data-stu-id="319a2-144">Whether a student can add resources to a submission or not.</span></span> <span data-ttu-id="319a2-145">Кроме того, указывает, соответствуют ли все ресурсы в представлении списку ресурсов назначения.</span><span class="sxs-lookup"><span data-stu-id="319a2-145">Also, indicates whether all resources in the submission correspond to the assignment resource list.</span></span> |
|<span data-ttu-id="319a2-146">assignDateTime</span><span class="sxs-lookup"><span data-stu-id="319a2-146">assignDateTime</span></span>|<span data-ttu-id="319a2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319a2-147">DateTimeOffset</span></span>| <span data-ttu-id="319a2-148">Указывает дату публикации назначения для учащихся.</span><span class="sxs-lookup"><span data-stu-id="319a2-148">Indicates the date to publish the assignment to students.</span></span> |
|<span data-ttu-id="319a2-149">assignTo</span><span class="sxs-lookup"><span data-stu-id="319a2-149">assignTo</span></span>|<span data-ttu-id="319a2-150">educationAssignmentRecipient</span><span class="sxs-lookup"><span data-stu-id="319a2-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="319a2-151">Студенты, получаювшие назначение.</span><span class="sxs-lookup"><span data-stu-id="319a2-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="319a2-152">closeDateTime</span><span class="sxs-lookup"><span data-stu-id="319a2-152">closeDateTime</span></span>|<span data-ttu-id="319a2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319a2-153">DateTimeOffset</span></span>| <span data-ttu-id="319a2-154">Дата закрытия назначения для отправки.</span><span class="sxs-lookup"><span data-stu-id="319a2-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="319a2-155">Это необязательный поле, которое может быть равно нуль, если назначение не позволяет использоватьLateSubmissions или closeDateTime то же самое, что и dueDateTime, но если указано, оно должно быть больше или равно dueDateTime.</span><span class="sxs-lookup"><span data-stu-id="319a2-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="319a2-156">displayName</span><span class="sxs-lookup"><span data-stu-id="319a2-156">displayName</span></span>|<span data-ttu-id="319a2-157">String</span><span class="sxs-lookup"><span data-stu-id="319a2-157">String</span></span>| <span data-ttu-id="319a2-158">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="319a2-158">Name of assignment.</span></span> |
|<span data-ttu-id="319a2-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="319a2-159">dueDateTime</span></span>|<span data-ttu-id="319a2-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319a2-160">DateTimeOffset</span></span>| <span data-ttu-id="319a2-161">Назначение даты должно быть.</span><span class="sxs-lookup"><span data-stu-id="319a2-161">Date assignment is due.</span></span> |
|<span data-ttu-id="319a2-162">классификация</span><span class="sxs-lookup"><span data-stu-id="319a2-162">grading</span></span>|<span data-ttu-id="319a2-163">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="319a2-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="319a2-164">Оценка назначения.</span><span class="sxs-lookup"><span data-stu-id="319a2-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="319a2-165">инструкции</span><span class="sxs-lookup"><span data-stu-id="319a2-165">instructions</span></span>|<span data-ttu-id="319a2-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="319a2-166">itemBody</span></span>| <span data-ttu-id="319a2-167">Инструкции, которые будут даны учащимся вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="319a2-167">Instructions to be given to the students along with the assignment.</span></span> |
|<span data-ttu-id="319a2-168">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="319a2-168">notificationChannelUrl</span></span>|<span data-ttu-id="319a2-169">String</span><span class="sxs-lookup"><span data-stu-id="319a2-169">String</span></span>| <span data-ttu-id="319a2-170">Канал для связи уведомлений, связанных с назначением.</span><span class="sxs-lookup"><span data-stu-id="319a2-170">The channel to communicate notifications related to the assignment.</span></span> <span data-ttu-id="319a2-171">Чтобы изменить URL-адрес, `assignTo` установите значение [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="319a2-171">To change the URL, set the `assignTo` value to [educationAssignmentClassRecipient](../resources/educationassignmentclassrecipient.md).</span></span> <span data-ttu-id="319a2-172">URL-адрес канала не может измениться после публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="319a2-172">The channel URL can't change after the publication of the assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="319a2-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="319a2-173">Response</span></span>
<span data-ttu-id="319a2-174">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="319a2-174">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="319a2-175">Пример</span><span class="sxs-lookup"><span data-stu-id="319a2-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="319a2-176">Запрос</span><span class="sxs-lookup"><span data-stu-id="319a2-176">Request</span></span>
<span data-ttu-id="319a2-177">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="319a2-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="319a2-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="319a2-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "update_educationassignment"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8
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
# <a name="c"></a>[<span data-ttu-id="319a2-179">C#</span><span class="sxs-lookup"><span data-stu-id="319a2-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="319a2-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="319a2-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="319a2-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="319a2-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="319a2-182">Java</span><span class="sxs-lookup"><span data-stu-id="319a2-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="319a2-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="319a2-183">Response</span></span>
<span data-ttu-id="319a2-184">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="319a2-184">The following is an example of the response.</span></span> 

><span data-ttu-id="319a2-185">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="319a2-185">**Note:** The response object shown here might be shortened for readability.</span></span>

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


