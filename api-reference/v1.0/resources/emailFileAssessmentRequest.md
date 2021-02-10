---
title: Тип ресурса emailFileAssessmentRequest
description: Используется для создания и извлечения оценки угрозы файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 43c7f1cbfe3087a092ca498969ce6df5250a7af8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153461"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="38b56-103">Тип ресурса emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="38b56-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="38b56-104">Используется для создания и извлечения оценки угрозы файла электронной почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="38b56-104">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="38b56-105">Файл электронной почты может быть EML-файлом.</span><span class="sxs-lookup"><span data-stu-id="38b56-105">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="38b56-106">Методы</span><span class="sxs-lookup"><span data-stu-id="38b56-106">Methods</span></span>

| <span data-ttu-id="38b56-107">Метод</span><span class="sxs-lookup"><span data-stu-id="38b56-107">Method</span></span>       | <span data-ttu-id="38b56-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38b56-108">Return Type</span></span> | <span data-ttu-id="38b56-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38b56-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="38b56-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="38b56-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="38b56-111">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="38b56-111">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="38b56-112">Создайте новый запрос на оценку файлов электронной почты, опубликовав объект **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="38b56-112">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="38b56-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="38b56-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="38b56-114">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="38b56-114">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="38b56-115">Чтение свойств и связей объекта **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="38b56-115">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="38b56-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="38b56-116">Properties</span></span>

| <span data-ttu-id="38b56-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="38b56-117">Property</span></span>     | <span data-ttu-id="38b56-118">Тип</span><span class="sxs-lookup"><span data-stu-id="38b56-118">Type</span></span>        | <span data-ttu-id="38b56-119">Описание</span><span class="sxs-lookup"><span data-stu-id="38b56-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38b56-120">contentData</span><span class="sxs-lookup"><span data-stu-id="38b56-120">contentData</span></span>|<span data-ttu-id="38b56-121">String</span><span class="sxs-lookup"><span data-stu-id="38b56-121">String</span></span>|<span data-ttu-id="38b56-122">Содержимое eml-файла электронной почты в коде Base64.</span><span class="sxs-lookup"><span data-stu-id="38b56-122">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="38b56-123">Содержимое файла не может получить обратно, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="38b56-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="38b56-124">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="38b56-124">destinationRoutingReason</span></span>|[<span data-ttu-id="38b56-125">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="38b56-125">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="38b56-126">Причина перенаправления почты в место назначения.</span><span class="sxs-lookup"><span data-stu-id="38b56-126">The reason for mail routed to its destination.</span></span> <span data-ttu-id="38b56-127">Возможные значения: `none` , , , , , , , `mailFlowRule` , , `safeSender` , `blockedSender` `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` . `junk`</span><span class="sxs-lookup"><span data-stu-id="38b56-127">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="38b56-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="38b56-128">recipientEmail</span></span>|<span data-ttu-id="38b56-129">String</span><span class="sxs-lookup"><span data-stu-id="38b56-129">String</span></span>|<span data-ttu-id="38b56-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="38b56-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="38b56-131">category</span><span class="sxs-lookup"><span data-stu-id="38b56-131">category</span></span>|[<span data-ttu-id="38b56-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="38b56-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="38b56-133">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="38b56-133">The threat category.</span></span> <span data-ttu-id="38b56-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="38b56-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="38b56-135">contentType</span><span class="sxs-lookup"><span data-stu-id="38b56-135">contentType</span></span>|[<span data-ttu-id="38b56-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="38b56-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="38b56-137">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="38b56-137">The content type of threat assessment.</span></span> <span data-ttu-id="38b56-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="38b56-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="38b56-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="38b56-139">createdBy</span></span>|[<span data-ttu-id="38b56-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="38b56-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="38b56-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="38b56-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="38b56-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38b56-142">createdDateTime</span></span>|<span data-ttu-id="38b56-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38b56-143">DateTimeOffset</span></span>|<span data-ttu-id="38b56-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="38b56-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38b56-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="38b56-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="38b56-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="38b56-146">expectedAssessment</span></span>|[<span data-ttu-id="38b56-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="38b56-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="38b56-148">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="38b56-148">The expected assessment from submitter.</span></span> <span data-ttu-id="38b56-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="38b56-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="38b56-150">id</span><span class="sxs-lookup"><span data-stu-id="38b56-150">id</span></span>|<span data-ttu-id="38b56-151">String</span><span class="sxs-lookup"><span data-stu-id="38b56-151">String</span></span>|<span data-ttu-id="38b56-152">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="38b56-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="38b56-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="38b56-153">requestSource</span></span>|[<span data-ttu-id="38b56-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="38b56-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="38b56-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="38b56-155">The source of threat assessment request.</span></span> <span data-ttu-id="38b56-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="38b56-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="38b56-157">status</span><span class="sxs-lookup"><span data-stu-id="38b56-157">status</span></span>|[<span data-ttu-id="38b56-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="38b56-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="38b56-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="38b56-159">The assessment process status.</span></span> <span data-ttu-id="38b56-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="38b56-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38b56-161">Связи</span><span class="sxs-lookup"><span data-stu-id="38b56-161">Relationships</span></span>

| <span data-ttu-id="38b56-162">Связь</span><span class="sxs-lookup"><span data-stu-id="38b56-162">Relationship</span></span> | <span data-ttu-id="38b56-163">Тип</span><span class="sxs-lookup"><span data-stu-id="38b56-163">Type</span></span>        | <span data-ttu-id="38b56-164">Описание</span><span class="sxs-lookup"><span data-stu-id="38b56-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38b56-165">results</span><span class="sxs-lookup"><span data-stu-id="38b56-165">results</span></span>|<span data-ttu-id="38b56-166">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="38b56-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="38b56-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="38b56-167">A collection of threat assessment results.</span></span> <span data-ttu-id="38b56-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="38b56-168">Read-only.</span></span> <span data-ttu-id="38b56-169">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="38b56-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38b56-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38b56-170">JSON representation</span></span>

<span data-ttu-id="38b56-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38b56-171">The following is a JSON representation of the resource.</span></span>

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

