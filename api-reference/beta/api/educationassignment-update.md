---
title: Обновление educationassignment
description: Обновление объекта назначения. Это можно сделать только преподавателями в классе. Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения. Чтобы изменить состояние назначения, используйте действие "опубликовать".
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 32d0b76d70e3e810b80d4cffd232343ab4e09cc9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436132"
---
# <a name="update-educationassignment"></a><span data-ttu-id="f11f2-106">Обновление educationassignment</span><span class="sxs-lookup"><span data-stu-id="f11f2-106">Update educationassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f11f2-107">Обновление объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-107">Update the assignment object.</span></span> <span data-ttu-id="f11f2-108">Это можно сделать только преподавателями в классе.</span><span class="sxs-lookup"><span data-stu-id="f11f2-108">Only teachers in the class can do this.</span></span> <span data-ttu-id="f11f2-109">Обратите внимание, что вы не можете использовать запрос PATCH для изменения состояния назначения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-109">Note that you can't use a PATCH request to change the status of an assignment.</span></span> <span data-ttu-id="f11f2-110">Чтобы изменить состояние назначения, используйте действие " [опубликовать](../api/educationassignment-publish.md) ".</span><span class="sxs-lookup"><span data-stu-id="f11f2-110">Use the [publish](../api/educationassignment-publish.md) action to change the assignment status.</span></span>

## <a name="permissions"></a><span data-ttu-id="f11f2-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f11f2-111">Permissions</span></span>
<span data-ttu-id="f11f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f11f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f11f2-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f11f2-114">Permission type</span></span>      | <span data-ttu-id="f11f2-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f11f2-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f11f2-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f11f2-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="f11f2-117">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f11f2-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f11f2-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f11f2-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f11f2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f11f2-119">Not supported.</span></span>  |
|<span data-ttu-id="f11f2-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f11f2-120">Application</span></span> | <span data-ttu-id="f11f2-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f11f2-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f11f2-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f11f2-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f11f2-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f11f2-123">Request headers</span></span>
| <span data-ttu-id="f11f2-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f11f2-124">Header</span></span>       | <span data-ttu-id="f11f2-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f11f2-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f11f2-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f11f2-126">Authorization</span></span>  | <span data-ttu-id="f11f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f11f2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f11f2-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f11f2-129">Content-Type</span></span>  | <span data-ttu-id="f11f2-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f11f2-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f11f2-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f11f2-131">Request body</span></span>
<span data-ttu-id="f11f2-132">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="f11f2-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f11f2-133">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="f11f2-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f11f2-134">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f11f2-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f11f2-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="f11f2-135">Property</span></span>     | <span data-ttu-id="f11f2-136">Тип</span><span class="sxs-lookup"><span data-stu-id="f11f2-136">Type</span></span>   |<span data-ttu-id="f11f2-137">Описание</span><span class="sxs-lookup"><span data-stu-id="f11f2-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f11f2-138">Алловлатесубмиссионс</span><span class="sxs-lookup"><span data-stu-id="f11f2-138">allowLateSubmissions</span></span>|<span data-ttu-id="f11f2-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f11f2-139">Boolean</span></span>| <span data-ttu-id="f11f2-140">Можно ли отправлять отправку после даты выполнения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-140">Whether submissions can be submitted after the due date.</span></span>|
|<span data-ttu-id="f11f2-141">Алловстудентстоаддресаурцестосубмиссион</span><span class="sxs-lookup"><span data-stu-id="f11f2-141">allowStudentsToAddResourcesToSubmission</span></span>|<span data-ttu-id="f11f2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f11f2-142">Boolean</span></span>| <span data-ttu-id="f11f2-143">Может ли студент добавить ресурсы в отправку.</span><span class="sxs-lookup"><span data-stu-id="f11f2-143">Whether a student can add resources to a submission.</span></span> <span data-ttu-id="f11f2-144">Указывает, поступили ли только элементы, отправленные в отправке, из списка ресурсов назначения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-144">Indicated whether the only items on the submission came from the assignment resource list.</span></span> |
|<span data-ttu-id="f11f2-145">Ассигндатетиме</span><span class="sxs-lookup"><span data-stu-id="f11f2-145">assignDateTime</span></span>|<span data-ttu-id="f11f2-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f11f2-146">DateTimeOffset</span></span>| <span data-ttu-id="f11f2-147">Дата, когда назначение должно быть опубликовано для учащихся.</span><span class="sxs-lookup"><span data-stu-id="f11f2-147">Date the assignment should be published to students.</span></span> |
|<span data-ttu-id="f11f2-148">Ассигнто</span><span class="sxs-lookup"><span data-stu-id="f11f2-148">assignTo</span></span>|<span data-ttu-id="f11f2-149">ЕдукатионассигнментреЦипиент</span><span class="sxs-lookup"><span data-stu-id="f11f2-149">educationAssignmentRecipient</span></span>| <span data-ttu-id="f11f2-150">Студенты, которые получают назначение.</span><span class="sxs-lookup"><span data-stu-id="f11f2-150">Students who get the assignment.</span></span>|
|<span data-ttu-id="f11f2-151">displayName</span><span class="sxs-lookup"><span data-stu-id="f11f2-151">displayName</span></span>|<span data-ttu-id="f11f2-152">String</span><span class="sxs-lookup"><span data-stu-id="f11f2-152">String</span></span>| <span data-ttu-id="f11f2-153">Имя назначения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-153">Name of assignment.</span></span> |
|<span data-ttu-id="f11f2-154">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="f11f2-154">dueDateTime</span></span>|<span data-ttu-id="f11f2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f11f2-155">DateTimeOffset</span></span>| <span data-ttu-id="f11f2-156">Дата выполнения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-156">Date assignment is due.</span></span> |
|<span data-ttu-id="f11f2-157">снижения</span><span class="sxs-lookup"><span data-stu-id="f11f2-157">grading</span></span>|<span data-ttu-id="f11f2-158">Едукатионассигнментградетипе</span><span class="sxs-lookup"><span data-stu-id="f11f2-158">educationAssignmentGradeType</span></span>| <span data-ttu-id="f11f2-159">Как будет выполняться оценка назначения.</span><span class="sxs-lookup"><span data-stu-id="f11f2-159">How the assignment will be graded.</span></span>|
|<span data-ttu-id="f11f2-160">выполнен</span><span class="sxs-lookup"><span data-stu-id="f11f2-160">instructions</span></span>|<span data-ttu-id="f11f2-161">Итембоди</span><span class="sxs-lookup"><span data-stu-id="f11f2-161">itemBody</span></span>| <span data-ttu-id="f11f2-162">Инструкции, которые необходимо предоставить студентам вместе с назначением.</span><span class="sxs-lookup"><span data-stu-id="f11f2-162">Instructions to be given to the students along with the assignment.</span></span> |

## <a name="response"></a><span data-ttu-id="f11f2-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="f11f2-163">Response</span></span>
<span data-ttu-id="f11f2-164">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f11f2-164">If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f11f2-165">Пример</span><span class="sxs-lookup"><span data-stu-id="f11f2-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f11f2-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="f11f2-166">Request</span></span>
<span data-ttu-id="f11f2-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f11f2-167">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f11f2-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="f11f2-168">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="f11f2-169">C#</span><span class="sxs-lookup"><span data-stu-id="f11f2-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f11f2-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="f11f2-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f11f2-171">Цель — C</span><span class="sxs-lookup"><span data-stu-id="f11f2-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f11f2-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="f11f2-172">Response</span></span>
<span data-ttu-id="f11f2-173">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f11f2-173">The following is an example of the response.</span></span> 

><span data-ttu-id="f11f2-174">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f11f2-174">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f11f2-175">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f11f2-175">All of the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
