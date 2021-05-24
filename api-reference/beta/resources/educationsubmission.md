---
title: тип ресурса educationSubmission
description: Отправки принадлежат назначению. Представление представляет ресурсы, которые человек (или группа) включит для назначения, и возвращаемую оценку/обратную связь.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f468e0715a07320233db1224c3fcee62e0c8fe63
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629443"
---
# <a name="educationsubmission-resource-type"></a><span data-ttu-id="c1969-104">тип ресурса educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-104">educationSubmission resource type</span></span>

<span data-ttu-id="c1969-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1969-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1969-106">Представление представляет ресурсы, которые человек (или группа) включит для назначения, и результаты (например, оценки или отзывы), связанные с отправкой.</span><span class="sxs-lookup"><span data-stu-id="c1969-106">A submission represents the resources that an individual (or group) turn in for an assignment and the outcomes (such as grades or feedback) that are associated with the submission.</span></span>

<span data-ttu-id="c1969-107">Отправки принадлежат назначению.</span><span class="sxs-lookup"><span data-stu-id="c1969-107">Submissions are owned by an assignment.</span></span> <span data-ttu-id="c1969-108">Отправки создаются автоматически при публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="c1969-108">Submissions are automatically created when an assignment is published.</span></span> <span data-ttu-id="c1969-109">Отправка содержит два списка ресурсов.</span><span class="sxs-lookup"><span data-stu-id="c1969-109">The submission owns two lists of resources.</span></span> <span data-ttu-id="c1969-110">Ресурсы представляют рабочую зону пользователя или группы, а представленные ресурсы представляют ресурсы, которые активно были переданы учащимися.</span><span class="sxs-lookup"><span data-stu-id="c1969-110">Resources represent the user/groups working area while the submitted resources represent the resources that have actively been turned in by students.</span></span>  

<span data-ttu-id="c1969-111">Свойство **status** является только для чтения, а объект перемещается через рабочий процесс с помощью действий.</span><span class="sxs-lookup"><span data-stu-id="c1969-111">The **status** property is read-only and the object is moved through the workflow via actions.</span></span> 

<span data-ttu-id="c1969-112">Если [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) не был вызван на ресурс **educationSubmission,** свойство **resourcesFolderUrl** `null` является .</span><span class="sxs-lookup"><span data-stu-id="c1969-112">If [setUpResourcesFolder](../api/educationsubmission-setupResourcesFolder.md) has not been called on an **educationSubmission** resource, the **resourcesFolderUrl** property is `null`.</span></span>

## <a name="methods"></a><span data-ttu-id="c1969-113">Методы</span><span class="sxs-lookup"><span data-stu-id="c1969-113">Methods</span></span>

| <span data-ttu-id="c1969-114">Метод</span><span class="sxs-lookup"><span data-stu-id="c1969-114">Method</span></span>           | <span data-ttu-id="c1969-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c1969-115">Return Type</span></span>    |<span data-ttu-id="c1969-116">Описание</span><span class="sxs-lookup"><span data-stu-id="c1969-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1969-117">Get educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-117">Get educationSubmission</span></span>](../api/educationsubmission-get.md) | [<span data-ttu-id="c1969-118">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-118">educationSubmission</span></span>](educationsubmission.md) |<span data-ttu-id="c1969-119">Чтение свойств и связей объекта **educationSubmission.**</span><span class="sxs-lookup"><span data-stu-id="c1969-119">Read properties and relationships of an **educationSubmission** object.</span></span>|
|[<span data-ttu-id="c1969-120">Список ресурсов</span><span class="sxs-lookup"><span data-stu-id="c1969-120">List resources</span></span>](../api/educationsubmission-list-resources.md) |<span data-ttu-id="c1969-121">[коллекция educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-121">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="c1969-122">Получите **коллекцию объектов educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="c1969-122">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="c1969-123">Список, представленныйРесурсеи</span><span class="sxs-lookup"><span data-stu-id="c1969-123">List submittedResources</span></span>](../api/educationsubmission-list-submittedresources.md) |<span data-ttu-id="c1969-124">[коллекция educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-124">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="c1969-125">Получите **коллекцию объектов educationSubmissionResource.**</span><span class="sxs-lookup"><span data-stu-id="c1969-125">Get an **educationSubmissionResource** object collection.</span></span>|
|[<span data-ttu-id="c1969-126">Результаты списка</span><span class="sxs-lookup"><span data-stu-id="c1969-126">List outcomes</span></span>](../api/educationsubmission-list-outcomes.md) |<span data-ttu-id="c1969-127">[коллекция educationOutcome](educationoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-127">[educationOutcome](educationoutcome.md) collection</span></span>| <span data-ttu-id="c1969-128">Получите **коллекцию объектов educationOutcome.**</span><span class="sxs-lookup"><span data-stu-id="c1969-128">Get an **educationOutcome** object collection.</span></span>|
|[<span data-ttu-id="c1969-129">возвращение</span><span class="sxs-lookup"><span data-stu-id="c1969-129">return</span></span>](../api/educationsubmission-return.md)|[<span data-ttu-id="c1969-130">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-130">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="c1969-131">Учитель использует возврат, чтобы указать, что оценки/отзывы могут быть показаны учащемуся.</span><span class="sxs-lookup"><span data-stu-id="c1969-131">A teacher uses return to indicate that the grades/feedback can be shown to the student.</span></span>|
|[<span data-ttu-id="c1969-132">Настройка папки определенных ресурсов для отправки</span><span class="sxs-lookup"><span data-stu-id="c1969-132">Set up submission specific resources folder</span></span>](../api/educationsubmission-setupResourcesFolder.md) |[<span data-ttu-id="c1969-133">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-133">educationSubmission</span></span>](educationsubmission.md) | <span data-ttu-id="c1969-134">Создайте SharePoint папку (в заранее определенном расположении) для отправки файлов в качестве ресурсов отправки.</span><span class="sxs-lookup"><span data-stu-id="c1969-134">Create a SharePoint folder (under pre-defined location) to upload files as submission resources.</span></span> |
|[<span data-ttu-id="c1969-135">Отправить</span><span class="sxs-lookup"><span data-stu-id="c1969-135">submit</span></span>](../api/educationsubmission-submit.md)|[<span data-ttu-id="c1969-136">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-136">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="c1969-137">Студент использует отправку для выполнения задания.</span><span class="sxs-lookup"><span data-stu-id="c1969-137">A student uses submit to turn in the assignment.</span></span> <span data-ttu-id="c1969-138">Это скопирует ресурсы в **папку submittedResources** для классификации и обновляет состояние.</span><span class="sxs-lookup"><span data-stu-id="c1969-138">This will copy the resources into the **submittedResources** folder for grading and updates the status.</span></span>|
|[<span data-ttu-id="c1969-139">ото всех</span><span class="sxs-lookup"><span data-stu-id="c1969-139">unsubmit</span></span>](../api/educationsubmission-unsubmit.md)|[<span data-ttu-id="c1969-140">educationSubmission</span><span class="sxs-lookup"><span data-stu-id="c1969-140">educationSubmission</span></span>](educationsubmission.md)|<span data-ttu-id="c1969-141">Студент использует отгрузку, чтобы переместить состояние отправки из отправленной в рабочую.</span><span class="sxs-lookup"><span data-stu-id="c1969-141">A student uses the unsubmit to move the state of the submission from submitted back to working.</span></span> <span data-ttu-id="c1969-142">Это скопирует ресурсы в **папку workingResources** для классификации и обновляет состояние.</span><span class="sxs-lookup"><span data-stu-id="c1969-142">This will copy the resources into the **workingResources** folder for grading and updates the status.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1969-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1969-143">Properties</span></span>
| <span data-ttu-id="c1969-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1969-144">Property</span></span>     | <span data-ttu-id="c1969-145">Тип</span><span class="sxs-lookup"><span data-stu-id="c1969-145">Type</span></span>   |<span data-ttu-id="c1969-146">Описание</span><span class="sxs-lookup"><span data-stu-id="c1969-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1969-147">получатель;</span><span class="sxs-lookup"><span data-stu-id="c1969-147">recipient</span></span>|[<span data-ttu-id="c1969-148">educationSubmissionRecipient</span><span class="sxs-lookup"><span data-stu-id="c1969-148">educationSubmissionRecipient</span></span>](educationsubmissionrecipient.md)|<span data-ttu-id="c1969-149">Кто этому представлению назначено.</span><span class="sxs-lookup"><span data-stu-id="c1969-149">Who this submission is assigned to.</span></span>|
|<span data-ttu-id="c1969-150">returnedBy</span><span class="sxs-lookup"><span data-stu-id="c1969-150">returnedBy</span></span>|[<span data-ttu-id="c1969-151">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1969-151">identitySet</span></span>](identityset.md)|<span data-ttu-id="c1969-152">Пользователь, переместивший состояние этой отправки в возвращенный.</span><span class="sxs-lookup"><span data-stu-id="c1969-152">User who moved the status of this submission to returned.</span></span>|
|<span data-ttu-id="c1969-153">returnedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1969-153">returnedDateTime</span></span>|<span data-ttu-id="c1969-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1969-154">DateTimeOffset</span></span>|<span data-ttu-id="c1969-155">Момент, когда отправка была возвращена.</span><span class="sxs-lookup"><span data-stu-id="c1969-155">Moment in time when the submission was returned.</span></span> <span data-ttu-id="c1969-156">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1969-156">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1969-157">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c1969-157">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c1969-158">resourcesFolderUrl</span><span class="sxs-lookup"><span data-stu-id="c1969-158">resourcesFolderUrl</span></span>|<span data-ttu-id="c1969-159">Строка</span><span class="sxs-lookup"><span data-stu-id="c1969-159">String</span></span>|<span data-ttu-id="c1969-160">Папка, в которой необходимо хранить все ресурсы файла для этой отправки.</span><span class="sxs-lookup"><span data-stu-id="c1969-160">Folder where all file resources for this submission need to be stored.</span></span>|
|<span data-ttu-id="c1969-161">status</span><span class="sxs-lookup"><span data-stu-id="c1969-161">status</span></span>|<span data-ttu-id="c1969-162">string</span><span class="sxs-lookup"><span data-stu-id="c1969-162">string</span></span>| <span data-ttu-id="c1969-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c1969-163">Read-Only.</span></span> <span data-ttu-id="c1969-164">Возможные значения: `working`, `submitted`, `released`, `returned`.</span><span class="sxs-lookup"><span data-stu-id="c1969-164">Possible values are: `working`, `submitted`, `released`, `returned`.</span></span>|
|<span data-ttu-id="c1969-165">submittedBy</span><span class="sxs-lookup"><span data-stu-id="c1969-165">submittedBy</span></span>|[<span data-ttu-id="c1969-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1969-166">identitySet</span></span>](identityset.md)|<span data-ttu-id="c1969-167">Пользователь, переместивший ресурс в состояние отправленного.</span><span class="sxs-lookup"><span data-stu-id="c1969-167">User who moved the resource into the submitted state.</span></span>|
|<span data-ttu-id="c1969-168">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1969-168">submittedDateTime</span></span>|<span data-ttu-id="c1969-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1969-169">DateTimeOffset</span></span>|<span data-ttu-id="c1969-170">Момент времени, когда отправка была перенесена в состояние отправленного.</span><span class="sxs-lookup"><span data-stu-id="c1969-170">Moment in time when the submission was moved into the submitted state.</span></span> <span data-ttu-id="c1969-171">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1969-171">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1969-172">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c1969-172">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="c1969-173">unsubmittedBy</span><span class="sxs-lookup"><span data-stu-id="c1969-173">unsubmittedBy</span></span>|[<span data-ttu-id="c1969-174">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1969-174">identitySet</span></span>](identityset.md)|<span data-ttu-id="c1969-175">Пользователь, переместивший ресурс из отправленного в рабочее состояние.</span><span class="sxs-lookup"><span data-stu-id="c1969-175">User who moved the resource from submitted into the working state.</span></span>|
|<span data-ttu-id="c1969-176">unsubmittedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1969-176">unsubmittedDateTime</span></span>|<span data-ttu-id="c1969-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1969-177">DateTimeOffset</span></span>|<span data-ttu-id="c1969-178">Момент времени, когда отправка была перенесена из представленного в рабочее состояние.</span><span class="sxs-lookup"><span data-stu-id="c1969-178">Moment in time when the submission was moved from submitted into the working state.</span></span> <span data-ttu-id="c1969-179">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c1969-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c1969-180">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="c1969-180">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1969-181">Связи</span><span class="sxs-lookup"><span data-stu-id="c1969-181">Relationships</span></span>
| <span data-ttu-id="c1969-182">Связь</span><span class="sxs-lookup"><span data-stu-id="c1969-182">Relationship</span></span> | <span data-ttu-id="c1969-183">Тип</span><span class="sxs-lookup"><span data-stu-id="c1969-183">Type</span></span>   |<span data-ttu-id="c1969-184">Описание</span><span class="sxs-lookup"><span data-stu-id="c1969-184">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1969-185">resources</span><span class="sxs-lookup"><span data-stu-id="c1969-185">resources</span></span>|<span data-ttu-id="c1969-186">[коллекция educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-186">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="c1969-187">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1969-187">Nullable.</span></span>|
|<span data-ttu-id="c1969-188">submittedResources</span><span class="sxs-lookup"><span data-stu-id="c1969-188">submittedResources</span></span>|<span data-ttu-id="c1969-189">[коллекция educationSubmissionResource](educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-189">[educationSubmissionResource](educationsubmissionresource.md) collection</span></span>| <span data-ttu-id="c1969-p109">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1969-p109">Read-only. Nullable.</span></span>|
|<span data-ttu-id="c1969-192">результаты</span><span class="sxs-lookup"><span data-stu-id="c1969-192">outcomes</span></span>|<span data-ttu-id="c1969-193">[коллекция educationOutcome.](educationOutcome.md)</span><span class="sxs-lookup"><span data-stu-id="c1969-193">[educationOutcome](educationOutcome.md) collection.</span></span> <span data-ttu-id="c1969-194">Содержит сведения о оценках, отзывах и/или рубриках, которые преподаватель назначает этому представлению.</span><span class="sxs-lookup"><span data-stu-id="c1969-194">Holds grades, feedback and/or rubrics information the teacher assigns to this submission</span></span>|<span data-ttu-id="c1969-195">Read-Write.</span><span class="sxs-lookup"><span data-stu-id="c1969-195">Read-Write.</span></span> <span data-ttu-id="c1969-196">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c1969-196">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1969-197">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1969-197">JSON representation</span></span>

<span data-ttu-id="c1969-198">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1969-198">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmission"
}-->

```json
{
    "id":"String (identifier)",
    "recipient":{"@odata.type":"microsoft.graph.educationSubmissionRecipient"},
    "returnedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "returnedDateTime":"String (timestamp)",
    "resourcesFolderUrl":"String",
    "status":"string",
    "submittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "submittedDateTime":"String (timestamp)",
    "unsubmittedBy":{"@odata.type":"microsoft.graph.identitySet"},
    "unsubmittedDateTime":"String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


