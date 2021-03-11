---
title: тип ресурса accessPackageAssignmentRequest
description: Запрос на назначение пакета доступа создается пользователем, который хочет получить назначение пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 83218058d375a9f78a24b2af837c39fb5ee77a2c
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720440"
---
# <a name="accesspackageassignmentrequest-resource-type"></a><span data-ttu-id="89051-103">тип ресурса accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89051-103">accessPackageAssignmentRequest resource type</span></span>

<span data-ttu-id="89051-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89051-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89051-105">В [управлении правами Azure AD](entitlementmanagement-root.md)запрос на назначение пакета доступа создается пользователем или от имени пользователя, который хочет получить назначение пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="89051-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package assignment request is created by or on behalf of a user who wants to obtain an access package assignment.</span></span> <span data-ttu-id="89051-106">Если запрос является успешным, с любыми необходимыми утверждениями, пользователь получает назначение пакета доступа и является субъектом этого назначения пакета доступа.</span><span class="sxs-lookup"><span data-stu-id="89051-106">If the request is successful, with any necessary approvals, the user receives an access package assignment, and is the subject of that resulting access package assignment.</span></span>  <span data-ttu-id="89051-107">Azure AD также создает запросы на назначение пакетов доступа автоматически для отслеживания удаления доступа.</span><span class="sxs-lookup"><span data-stu-id="89051-107">Azure AD also creates access package assignment requests automatically for tracking access removal.</span></span>

## <a name="methods"></a><span data-ttu-id="89051-108">Методы</span><span class="sxs-lookup"><span data-stu-id="89051-108">Methods</span></span>

| <span data-ttu-id="89051-109">Метод</span><span class="sxs-lookup"><span data-stu-id="89051-109">Method</span></span>       | <span data-ttu-id="89051-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="89051-110">Return Type</span></span> | <span data-ttu-id="89051-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89051-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="89051-112">Список accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="89051-112">List accessPackageAssignmentRequests</span></span>](../api/accesspackageassignmentrequest-list.md) | <span data-ttu-id="89051-113">[accessPackageAssignmentRequest collection](accesspackageassignmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="89051-113">[accessPackageAssignmentRequest](accesspackageassignmentrequest.md) collection</span></span> | <span data-ttu-id="89051-114">Извлечение списка объектов accesspackageassignmentrequest.</span><span class="sxs-lookup"><span data-stu-id="89051-114">Retrieve a list of accesspackageassignmentrequest objects.</span></span> |
| [<span data-ttu-id="89051-115">Создание accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89051-115">Create accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-post.md) | [<span data-ttu-id="89051-116">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89051-116">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="89051-117">Создание нового accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="89051-117">Create a new accessPackageAssignmentRequest.</span></span> |
| [<span data-ttu-id="89051-118">Получить accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89051-118">Get accessPackageAssignmentRequest</span></span>](../api/accesspackageassignmentrequest-get.md) | [<span data-ttu-id="89051-119">accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="89051-119">accessPackageAssignmentRequest</span></span>](accesspackageassignmentrequest.md) | <span data-ttu-id="89051-120">Чтение свойств и связей объекта accessPackageAssignmentRequest.</span><span class="sxs-lookup"><span data-stu-id="89051-120">Read properties and relationships of an accessPackageAssignmentRequest object.</span></span> |

## <a name="properties"></a><span data-ttu-id="89051-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="89051-121">Properties</span></span>

| <span data-ttu-id="89051-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="89051-122">Property</span></span>     | <span data-ttu-id="89051-123">Тип</span><span class="sxs-lookup"><span data-stu-id="89051-123">Type</span></span>        | <span data-ttu-id="89051-124">Описание</span><span class="sxs-lookup"><span data-stu-id="89051-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89051-125">completedDate</span><span class="sxs-lookup"><span data-stu-id="89051-125">completedDate</span></span>|<span data-ttu-id="89051-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89051-126">DateTimeOffset</span></span>|<span data-ttu-id="89051-127">Дата окончания обработки , успешной или неудачной, запроса.</span><span class="sxs-lookup"><span data-stu-id="89051-127">The date of the end of processing, either successful or failure, of a request.</span></span> <span data-ttu-id="89051-128">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="89051-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="89051-129">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="89051-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="89051-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-130">Read-only.</span></span>|
|<span data-ttu-id="89051-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89051-131">createdDateTime</span></span>|<span data-ttu-id="89051-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89051-132">DateTimeOffset</span></span>|<span data-ttu-id="89051-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="89051-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="89051-134">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="89051-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="89051-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-135">Read-only.</span></span>|
|<span data-ttu-id="89051-136">id</span><span class="sxs-lookup"><span data-stu-id="89051-136">id</span></span>|<span data-ttu-id="89051-137">String</span><span class="sxs-lookup"><span data-stu-id="89051-137">String</span></span>| <span data-ttu-id="89051-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-138">Read-only.</span></span>|
|<span data-ttu-id="89051-139">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="89051-139">isValidationOnly</span></span>|<span data-ttu-id="89051-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="89051-140">Boolean</span></span>|<span data-ttu-id="89051-141">True, если запрос не обрабатывается для назначения.</span><span class="sxs-lookup"><span data-stu-id="89051-141">True if the request is not to be processed for assignment.</span></span>|
|<span data-ttu-id="89051-142">обоснование</span><span class="sxs-lookup"><span data-stu-id="89051-142">justification</span></span>|<span data-ttu-id="89051-143">String</span><span class="sxs-lookup"><span data-stu-id="89051-143">String</span></span>|<span data-ttu-id="89051-144">Предоставлено обоснование запроса.</span><span class="sxs-lookup"><span data-stu-id="89051-144">The requestor's supplied justification.</span></span>|
|<span data-ttu-id="89051-145">requestState</span><span class="sxs-lookup"><span data-stu-id="89051-145">requestState</span></span>|<span data-ttu-id="89051-146">String</span><span class="sxs-lookup"><span data-stu-id="89051-146">String</span></span>|<span data-ttu-id="89051-147">Один `PendingApproval` из `Canceled` , , , , , или  `Denied` `Delivering` `Delivered` `PartiallyDelivered` `Submitted` `Scheduled` .</span><span class="sxs-lookup"><span data-stu-id="89051-147">One of `PendingApproval`, `Canceled`,  `Denied`, `Delivering`, `Delivered`, `PartiallyDelivered`, `Submitted` or `Scheduled`.</span></span> <span data-ttu-id="89051-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-148">Read-only.</span></span>|
|<span data-ttu-id="89051-149">requestStatus</span><span class="sxs-lookup"><span data-stu-id="89051-149">requestStatus</span></span>|<span data-ttu-id="89051-150">String</span><span class="sxs-lookup"><span data-stu-id="89051-150">String</span></span>|<span data-ttu-id="89051-151">Дополнительные сведения о состоянии обработки запросов.</span><span class="sxs-lookup"><span data-stu-id="89051-151">More information on the request processing status.</span></span> <span data-ttu-id="89051-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-152">Read-only.</span></span>|
|<span data-ttu-id="89051-153">requestType</span><span class="sxs-lookup"><span data-stu-id="89051-153">requestType</span></span>|<span data-ttu-id="89051-154">String</span><span class="sxs-lookup"><span data-stu-id="89051-154">String</span></span>|<span data-ttu-id="89051-155">Один `UserAdd` из `UserRemove` , , или `AdminAdd` `AdminRemove` `SystemRemove` .</span><span class="sxs-lookup"><span data-stu-id="89051-155">One of `UserAdd`, `UserRemove`, `AdminAdd`, `AdminRemove` or `SystemRemove`.</span></span> <span data-ttu-id="89051-156">Запрос от самого пользователя будет иметь requestType или `UserAdd` `UserRemove` .</span><span class="sxs-lookup"><span data-stu-id="89051-156">A request from the user themselves would have requestType of `UserAdd` or `UserRemove`.</span></span> <span data-ttu-id="89051-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-157">Read-only.</span></span>|
|<span data-ttu-id="89051-158">schedule</span><span class="sxs-lookup"><span data-stu-id="89051-158">schedule</span></span>|[<span data-ttu-id="89051-159">requestSchedule</span><span class="sxs-lookup"><span data-stu-id="89051-159">requestSchedule</span></span>](requestschedule.md)| <span data-ttu-id="89051-160">Диапазон дат, которые должен быть назначен запросчику.</span><span class="sxs-lookup"><span data-stu-id="89051-160">The range of dates that access is to be assigned to the requestor.</span></span> <span data-ttu-id="89051-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-161">Read-only.</span></span>|
|<span data-ttu-id="89051-162">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="89051-162">accessPackageAssignment</span></span>|[<span data-ttu-id="89051-163">accessPackageAssignment</span><span class="sxs-lookup"><span data-stu-id="89051-163">accessPackageAssignment</span></span>](accesspackageassignment.md)| <span data-ttu-id="89051-164">Для requestType или , это назначение пакета `UserAdd` `AdminAdd` доступа, запрашиваемого для создания.</span><span class="sxs-lookup"><span data-stu-id="89051-164">For a requestType of `UserAdd` or `AdminAdd`, this is an access package assignment requested to be created.</span></span>  <span data-ttu-id="89051-165">Для requestType или , это свойство существующего `UserRemove` `AdminRemove` `SystemRemove` `id` назначения, которые будут удалены.</span><span class="sxs-lookup"><span data-stu-id="89051-165">For a requestType of `UserRemove`, `AdminRemove` or `SystemRemove`, this has the `id` property of an existing assignment to be removed.</span></span>|
|<span data-ttu-id="89051-166">ответы</span><span class="sxs-lookup"><span data-stu-id="89051-166">answers</span></span>|<span data-ttu-id="89051-167">[коллекция accessPackageAnswer](accesspackageanswer.md)</span><span class="sxs-lookup"><span data-stu-id="89051-167">[accessPackageAnswer](accesspackageanswer.md) collection</span></span>|<span data-ttu-id="89051-168">Ответы, предоставленные запрашивателем для [доступа кPackageQuestions,](accesspackagequestion.md) заданные им во время запроса.</span><span class="sxs-lookup"><span data-stu-id="89051-168">Answers provided by the requestor to [accessPackageQuestions](accesspackagequestion.md) asked of them at the time of request.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89051-169">Связи</span><span class="sxs-lookup"><span data-stu-id="89051-169">Relationships</span></span>

| <span data-ttu-id="89051-170">Связь</span><span class="sxs-lookup"><span data-stu-id="89051-170">Relationship</span></span> | <span data-ttu-id="89051-171">Тип</span><span class="sxs-lookup"><span data-stu-id="89051-171">Type</span></span>        | <span data-ttu-id="89051-172">Описание</span><span class="sxs-lookup"><span data-stu-id="89051-172">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89051-173">запросчик</span><span class="sxs-lookup"><span data-stu-id="89051-173">requestor</span></span>|[<span data-ttu-id="89051-174">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="89051-174">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="89051-175">Субъекту, который запрашивал или, если прямое назначение, было назначено.</span><span class="sxs-lookup"><span data-stu-id="89051-175">The subject who requested or, if a direct assignment, was assigned.</span></span> <span data-ttu-id="89051-176">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89051-176">Read-only.</span></span> <span data-ttu-id="89051-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="89051-177">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89051-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89051-178">JSON representation</span></span>

<span data-ttu-id="89051-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89051-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "keyProperty": "id"
}-->

```json
{
    "createdDateTime": "string",
    "completedDate": "string",
    "id": "string",
    "requestType": "string",
    "requestState": "string",
    "requestStatus": "string",
    "isValidationOnly": false,
    "justification": "string",
    "answers": [{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "string",
        "answeredQuestion": {
            "id": "string",
            "text": {
                "defaultText": "string",
                "localizedTexts": [{
                    "text": "string",
                    "languageCode": "string"
                }]
            },
            "isRequired": true,
            "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
            "isSingleLineQuestion": true
        }
    }]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

