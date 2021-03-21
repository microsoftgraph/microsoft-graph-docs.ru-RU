---
title: тип ресурса emailFileAssessmentRequest
description: Используется для создания и получения оценки угрозы файлов электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 77c95b18056487f94a5cb75b946d0ee8f75e46f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960448"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="5553d-103">тип ресурса emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5553d-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="5553d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5553d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5553d-105">Используется для создания и получения оценки угрозы файлов электронной почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5553d-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="5553d-106">Файл электронной почты может быть типом файла .eml.</span><span class="sxs-lookup"><span data-stu-id="5553d-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="5553d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5553d-107">Methods</span></span>

| <span data-ttu-id="5553d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5553d-108">Method</span></span>       | <span data-ttu-id="5553d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5553d-109">Return Type</span></span> | <span data-ttu-id="5553d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5553d-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5553d-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5553d-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5553d-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5553d-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="5553d-113">Создайте новый запрос на оценку файлов электронной почты, разместив объект **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5553d-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="5553d-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5553d-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5553d-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5553d-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="5553d-116">Ознакомьтесь с свойствами и отношениями объекта **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5553d-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5553d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5553d-117">Properties</span></span>

| <span data-ttu-id="5553d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5553d-118">Property</span></span>     | <span data-ttu-id="5553d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5553d-119">Type</span></span>        | <span data-ttu-id="5553d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5553d-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5553d-121">contentData</span><span class="sxs-lookup"><span data-stu-id="5553d-121">contentData</span></span>|<span data-ttu-id="5553d-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5553d-122">String</span></span>|<span data-ttu-id="5553d-123">Base64 закодированное содержимое файлов электронной почты .eml.</span><span class="sxs-lookup"><span data-stu-id="5553d-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="5553d-124">Содержимое файла не может получить обратно, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="5553d-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="5553d-125">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5553d-125">destinationRoutingReason</span></span>|[<span data-ttu-id="5553d-126">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5553d-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="5553d-127">Причина направления почты в пункт назначения.</span><span class="sxs-lookup"><span data-stu-id="5553d-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="5553d-128">Возможные значения: `none` `mailFlowRule` , , , , , `safeSender` , `blockedSender` , `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` , `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` , .</span><span class="sxs-lookup"><span data-stu-id="5553d-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="5553d-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="5553d-129">recipientEmail</span></span>|<span data-ttu-id="5553d-130">Строка</span><span class="sxs-lookup"><span data-stu-id="5553d-130">String</span></span>|<span data-ttu-id="5553d-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="5553d-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="5553d-132">category</span><span class="sxs-lookup"><span data-stu-id="5553d-132">category</span></span>|[<span data-ttu-id="5553d-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="5553d-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5553d-134">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="5553d-134">The threat category.</span></span> <span data-ttu-id="5553d-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5553d-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5553d-136">contentType</span><span class="sxs-lookup"><span data-stu-id="5553d-136">contentType</span></span>|[<span data-ttu-id="5553d-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="5553d-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5553d-138">Тип оценки угрозы контента.</span><span class="sxs-lookup"><span data-stu-id="5553d-138">The content type of threat assessment.</span></span> <span data-ttu-id="5553d-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5553d-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5553d-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="5553d-140">createdBy</span></span>|[<span data-ttu-id="5553d-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="5553d-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="5553d-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5553d-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5553d-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5553d-143">createdDateTime</span></span>|<span data-ttu-id="5553d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5553d-144">DateTimeOffset</span></span>|<span data-ttu-id="5553d-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5553d-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5553d-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5553d-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5553d-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5553d-147">expectedAssessment</span></span>|[<span data-ttu-id="5553d-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5553d-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5553d-149">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="5553d-149">The expected assessment from submitter.</span></span> <span data-ttu-id="5553d-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5553d-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5553d-151">id</span><span class="sxs-lookup"><span data-stu-id="5553d-151">id</span></span>|<span data-ttu-id="5553d-152">Строка</span><span class="sxs-lookup"><span data-stu-id="5553d-152">String</span></span>|<span data-ttu-id="5553d-153">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="5553d-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5553d-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="5553d-154">requestSource</span></span>|[<span data-ttu-id="5553d-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="5553d-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5553d-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5553d-156">The source of threat assessment request.</span></span> <span data-ttu-id="5553d-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5553d-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5553d-158">status</span><span class="sxs-lookup"><span data-stu-id="5553d-158">status</span></span>|[<span data-ttu-id="5553d-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="5553d-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5553d-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5553d-160">The assessment process status.</span></span> <span data-ttu-id="5553d-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5553d-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5553d-162">Связи</span><span class="sxs-lookup"><span data-stu-id="5553d-162">Relationships</span></span>

| <span data-ttu-id="5553d-163">Связь</span><span class="sxs-lookup"><span data-stu-id="5553d-163">Relationship</span></span> | <span data-ttu-id="5553d-164">Тип</span><span class="sxs-lookup"><span data-stu-id="5553d-164">Type</span></span>        | <span data-ttu-id="5553d-165">Описание</span><span class="sxs-lookup"><span data-stu-id="5553d-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5553d-166">results</span><span class="sxs-lookup"><span data-stu-id="5553d-166">results</span></span>|<span data-ttu-id="5553d-167">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5553d-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5553d-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5553d-168">A collection of threat assessment results.</span></span> <span data-ttu-id="5553d-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5553d-169">Read-only.</span></span> <span data-ttu-id="5553d-170">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="5553d-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5553d-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5553d-171">JSON representation</span></span>

<span data-ttu-id="5553d-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5553d-172">The following is a JSON representation of the resource.</span></span>

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


