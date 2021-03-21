---
title: тип ресурса emailFileAssessmentRequest
description: Используется для создания и получения оценки угрозы файлов электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 707cc20666df8d225e0e2f0853cf47cb9b6352c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959307"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="e9c91-103">тип ресурса emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9c91-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="e9c91-104">Используется для создания и получения оценки угрозы файлов электронной почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="e9c91-104">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="e9c91-105">Файл электронной почты может быть типом файла .eml.</span><span class="sxs-lookup"><span data-stu-id="e9c91-105">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="e9c91-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e9c91-106">Methods</span></span>

| <span data-ttu-id="e9c91-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e9c91-107">Method</span></span>       | <span data-ttu-id="e9c91-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e9c91-108">Return Type</span></span> | <span data-ttu-id="e9c91-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e9c91-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e9c91-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9c91-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="e9c91-111">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9c91-111">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="e9c91-112">Создайте новый запрос на оценку файлов электронной почты, разместив объект **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="e9c91-112">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="e9c91-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9c91-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="e9c91-114">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e9c91-114">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="e9c91-115">Ознакомьтесь с свойствами и отношениями объекта **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="e9c91-115">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9c91-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9c91-116">Properties</span></span>

| <span data-ttu-id="e9c91-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9c91-117">Property</span></span>     | <span data-ttu-id="e9c91-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e9c91-118">Type</span></span>        | <span data-ttu-id="e9c91-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e9c91-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9c91-120">contentData</span><span class="sxs-lookup"><span data-stu-id="e9c91-120">contentData</span></span>|<span data-ttu-id="e9c91-121">String</span><span class="sxs-lookup"><span data-stu-id="e9c91-121">String</span></span>|<span data-ttu-id="e9c91-122">Base64 закодированное содержимое файлов электронной почты .eml.</span><span class="sxs-lookup"><span data-stu-id="e9c91-122">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="e9c91-123">Содержимое файла не может получить обратно, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="e9c91-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="e9c91-124">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="e9c91-124">destinationRoutingReason</span></span>|[<span data-ttu-id="e9c91-125">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="e9c91-125">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="e9c91-126">Причина направления почты в пункт назначения.</span><span class="sxs-lookup"><span data-stu-id="e9c91-126">The reason for mail routed to its destination.</span></span> <span data-ttu-id="e9c91-127">Возможные значения: `none` `mailFlowRule` , , , , , `safeSender` , `blockedSender` , `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` , `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` , .</span><span class="sxs-lookup"><span data-stu-id="e9c91-127">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="e9c91-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="e9c91-128">recipientEmail</span></span>|<span data-ttu-id="e9c91-129">String</span><span class="sxs-lookup"><span data-stu-id="e9c91-129">String</span></span>|<span data-ttu-id="e9c91-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="e9c91-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="e9c91-131">category</span><span class="sxs-lookup"><span data-stu-id="e9c91-131">category</span></span>|[<span data-ttu-id="e9c91-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="e9c91-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="e9c91-133">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="e9c91-133">The threat category.</span></span> <span data-ttu-id="e9c91-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="e9c91-135">contentType</span><span class="sxs-lookup"><span data-stu-id="e9c91-135">contentType</span></span>|[<span data-ttu-id="e9c91-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="e9c91-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="e9c91-137">Тип оценки угрозы контента.</span><span class="sxs-lookup"><span data-stu-id="e9c91-137">The content type of threat assessment.</span></span> <span data-ttu-id="e9c91-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="e9c91-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="e9c91-139">createdBy</span></span>|[<span data-ttu-id="e9c91-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9c91-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="e9c91-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e9c91-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="e9c91-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9c91-142">createdDateTime</span></span>|<span data-ttu-id="e9c91-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9c91-143">DateTimeOffset</span></span>|<span data-ttu-id="e9c91-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e9c91-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9c91-145">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e9c91-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e9c91-146">expectedAssessment</span></span>|[<span data-ttu-id="e9c91-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e9c91-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="e9c91-148">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="e9c91-148">The expected assessment from submitter.</span></span> <span data-ttu-id="e9c91-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="e9c91-150">id</span><span class="sxs-lookup"><span data-stu-id="e9c91-150">id</span></span>|<span data-ttu-id="e9c91-151">String</span><span class="sxs-lookup"><span data-stu-id="e9c91-151">String</span></span>|<span data-ttu-id="e9c91-152">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="e9c91-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e9c91-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="e9c91-153">requestSource</span></span>|[<span data-ttu-id="e9c91-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="e9c91-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="e9c91-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e9c91-155">The source of threat assessment request.</span></span> <span data-ttu-id="e9c91-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="e9c91-157">status</span><span class="sxs-lookup"><span data-stu-id="e9c91-157">status</span></span>|[<span data-ttu-id="e9c91-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="e9c91-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="e9c91-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="e9c91-159">The assessment process status.</span></span> <span data-ttu-id="e9c91-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="e9c91-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9c91-161">Связи</span><span class="sxs-lookup"><span data-stu-id="e9c91-161">Relationships</span></span>

| <span data-ttu-id="e9c91-162">Связь</span><span class="sxs-lookup"><span data-stu-id="e9c91-162">Relationship</span></span> | <span data-ttu-id="e9c91-163">Тип</span><span class="sxs-lookup"><span data-stu-id="e9c91-163">Type</span></span>        | <span data-ttu-id="e9c91-164">Описание</span><span class="sxs-lookup"><span data-stu-id="e9c91-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9c91-165">results</span><span class="sxs-lookup"><span data-stu-id="e9c91-165">results</span></span>|<span data-ttu-id="e9c91-166">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="e9c91-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="e9c91-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="e9c91-167">A collection of threat assessment results.</span></span> <span data-ttu-id="e9c91-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e9c91-168">Read-only.</span></span> <span data-ttu-id="e9c91-169">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="e9c91-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9c91-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9c91-170">JSON representation</span></span>

<span data-ttu-id="e9c91-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9c91-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String",
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailFileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

