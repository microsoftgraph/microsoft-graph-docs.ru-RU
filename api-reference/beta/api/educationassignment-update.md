---
title: Обновление educationassignment
description: Обновление объекта назначения. Это можно сделать только преподавателями в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы изменить состояние назначения, используйте действие "опубликовать".
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e8efe5064196e179fade55704d4ea28a349fb801
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966501"
---
# <a name="update-educationassignment"></a><span data-ttu-id="edd9c-106">Обновление educationassignment</span><span class="sxs-lookup"><span data-stu-id="edd9c-106">Update educationassignment</span></span>

<span data-ttu-id="edd9c-107">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edd9c-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd9c-108">Обновление объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-108">Update the assignment object.</span></span> <span data-ttu-id="edd9c-109">Это можно сделать только преподавателями в классе.</span><span class="sxs-lookup"><span data-stu-id="edd9c-109">Only teachers in the class can do this.</span></span> <span data-ttu-id="edd9c-110">Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-110">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="edd9c-111">Чтобы изменить состояние назначения, используйте действие " [опубликовать](../api/educationassignment-publish.md) ".</span><span class="sxs-lookup"><span data-stu-id="edd9c-111">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="edd9c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="edd9c-112">Permissions</span></span>
<span data-ttu-id="edd9c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edd9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edd9c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edd9c-115">Permission type</span></span>      | <span data-ttu-id="edd9c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edd9c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edd9c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edd9c-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="edd9c-118">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="edd9c-118">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="edd9c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edd9c-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="edd9c-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd9c-120">Not supported.</span></span>  |
|<span data-ttu-id="edd9c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edd9c-121">Application</span></span> | <span data-ttu-id="edd9c-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edd9c-122">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="edd9c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edd9c-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="edd9c-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edd9c-124">Request headers</span></span>
| <span data-ttu-id="edd9c-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edd9c-125">Header</span></span>       | <span data-ttu-id="edd9c-126">Значение</span><span class="sxs-lookup"><span data-stu-id="edd9c-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edd9c-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edd9c-127">Authorization</span></span>  | <span data-ttu-id="edd9c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edd9c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edd9c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edd9c-130">Content-Type</span></span>  | <span data-ttu-id="edd9c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="edd9c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edd9c-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edd9c-132">Request body</span></span>
<span data-ttu-id="edd9c-133">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="edd9c-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="edd9c-134">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="edd9c-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="edd9c-135">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="edd9c-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="edd9c-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="edd9c-136">Property</span></span>     | <span data-ttu-id="edd9c-137">Тип</span><span class="sxs-lookup"><span data-stu-id="edd9c-137">Type</span></span>   |<span data-ttu-id="edd9c-138">Описание</span><span class="sxs-lookup"><span data-stu-id="edd9c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edd9c-139">алловлатесубмиссионс</span><span class="sxs-lookup"><span data-stu-id="edd9c-139">allowLateSubmissions</span></span>|<span data-ttu-id="edd9c-140">Логический</span><span class="sxs-lookup"><span data-stu-id="edd9c-140">Boolean</span></span>| <span data-ttu-id="edd9c-141">Можно ли отправлять отправку после даты выполнения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-141">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="edd9c-142">алловстудентстоаддресаурцестосубмиссион</span><span class="sxs-lookup"><span data-stu-id="edd9c-142">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="edd9c-143">Логический</span><span class="sxs-lookup"><span data-stu-id="edd9c-143">Boolean</span></span>| <span data-ttu-id="edd9c-144">Может ли студент добавить ресурсы в отправку.</span><span class="sxs-lookup"><span data-stu-id="edd9c-144">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="edd9c-145">Указывает, поступили ли только элементы, отправленные в отправке, из списка ресурсов назначения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-145">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="edd9c-146">ассигндатетиме</span><span class="sxs-lookup"><span data-stu-id="edd9c-146">assignDateTime</span></span>|<span data-ttu-id="edd9c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edd9c-147">DateTimeOffset</span></span>| <span data-ttu-id="edd9c-148">Дата, когда назначение должно быть опубликовано для учащихся.</span><span class="sxs-lookup"><span data-stu-id="edd9c-148">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="edd9c-149">ассигнто</span><span class="sxs-lookup"><span data-stu-id="edd9c-149">assignTo</span></span>|<span data-ttu-id="edd9c-150">едукатионассигнментреЦипиент</span><span class="sxs-lookup"><span data-stu-id="edd9c-150">educationAssignmentRecipient</span></span>| <span data-ttu-id="edd9c-151">Студенты, которые получают назначение.</span><span class="sxs-lookup"><span data-stu-id="edd9c-151">Students who get the assignment.</span></span>|
|<span data-ttu-id="edd9c-152">клоседатетиме</span><span class="sxs-lookup"><span data-stu-id="edd9c-152">closeDateTime</span></span>|<span data-ttu-id="edd9c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edd9c-153">DateTimeOffset</span></span>| <span data-ttu-id="edd9c-154">Дата, когда назначение будет закрыто для отправки.</span><span class="sxs-lookup"><span data-stu-id="edd9c-154">Date when the assignment will be closed for submissions.</span></span> <span data-ttu-id="edd9c-155">Это необязательное поле, которое может иметь значение null, если назначение не Алловлатесубмиссионс или Клоседатетиме совпадает с Дуедатетиме, но если указано, оно должно быть больше или равно Дуедатетиме.</span><span class="sxs-lookup"><span data-stu-id="edd9c-155">This is an optional field that can be null if the assignment does not allowLateSubmissions or the closeDateTime is the same as the dueDateTime but if specified, it must be greater than or equal to the dueDateTime.</span></span>|
|<span data-ttu-id="edd9c-156">displayName</span><span class="sxs-lookup"><span data-stu-id="edd9c-156">displayName</span></span>|<span data-ttu-id="edd9c-157">String</span><span class="sxs-lookup"><span data-stu-id="edd9c-157">String</span></span>| <span data-ttu-id="edd9c-158">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-158">Name of assignment.</span></span> |
|<span data-ttu-id="edd9c-159">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="edd9c-159">dueDateTime</span></span>|<span data-ttu-id="edd9c-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edd9c-160">DateTimeOffset</span></span>| <span data-ttu-id="edd9c-161">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-161">Date assignment is due.</span></span> |
|<span data-ttu-id="edd9c-162">снижения</span><span class="sxs-lookup"><span data-stu-id="edd9c-162">grading</span></span>|<span data-ttu-id="edd9c-163">едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="edd9c-163">educationAssignmentGradeType</span></span>| <span data-ttu-id="edd9c-164">Как будет выполняться оценка назначения.</span><span class="sxs-lookup"><span data-stu-id="edd9c-164">How the assignment will be graded.</span></span>|
|<span data-ttu-id="edd9c-165">выполнен</span><span class="sxs-lookup"><span data-stu-id="edd9c-165">instructions</span></span>|<span data-ttu-id="edd9c-166">itemBody</span><span class="sxs-lookup"><span data-stu-id="edd9c-166">itemBody</span></span>| <span data-ttu-id="edd9c-167">Инструкции, которые необходимо предоставить студентам вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="edd9c-167">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="edd9c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="edd9c-168">Response</span></span>
<span data-ttu-id="edd9c-169">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edd9c-169">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="edd9c-170">Пример</span><span class="sxs-lookup"><span data-stu-id="edd9c-170">Example</span></span>
##### <a name="request"></a><span data-ttu-id="edd9c-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="edd9c-171">Request</span></span>
<span data-ttu-id="edd9c-172">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edd9c-172">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="edd9c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="edd9c-173">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="edd9c-174">C#</span><span class="sxs-lookup"><span data-stu-id="edd9c-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="edd9c-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="edd9c-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="edd9c-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="edd9c-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="edd9c-177">Java</span><span class="sxs-lookup"><span data-stu-id="edd9c-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="edd9c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="edd9c-178">Response</span></span>
<span data-ttu-id="edd9c-179">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edd9c-179">The following is an example of the response.</span></span> 

><span data-ttu-id="edd9c-180">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="edd9c-180">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="edd9c-181">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edd9c-181">All of the properties will be returned from an actual call.</span></span>

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


