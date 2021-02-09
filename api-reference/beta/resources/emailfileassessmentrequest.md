---
title: Тип ресурса emailFileAssessmentRequest
description: Используется для создания и извлечения оценки угрозы файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1aa31301c4283d1adf6bfeb352eeaea7474823a6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159145"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="5e188-103">Тип ресурса emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5e188-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="5e188-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e188-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e188-105">Используется для создания и извлечения оценки угрозы файла электронной почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5e188-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="5e188-106">Файл электронной почты может быть EML-файлом.</span><span class="sxs-lookup"><span data-stu-id="5e188-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="5e188-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5e188-107">Methods</span></span>

| <span data-ttu-id="5e188-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5e188-108">Method</span></span>       | <span data-ttu-id="5e188-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5e188-109">Return Type</span></span> | <span data-ttu-id="5e188-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5e188-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5e188-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5e188-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5e188-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5e188-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="5e188-113">Создайте новый запрос на оценку файлов электронной почты, опубликовав объект **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5e188-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="5e188-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5e188-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5e188-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5e188-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="5e188-116">Чтение свойств и связей объекта **emailFileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5e188-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5e188-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e188-117">Properties</span></span>

| <span data-ttu-id="5e188-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e188-118">Property</span></span>     | <span data-ttu-id="5e188-119">Тип</span><span class="sxs-lookup"><span data-stu-id="5e188-119">Type</span></span>        | <span data-ttu-id="5e188-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5e188-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e188-121">contentData</span><span class="sxs-lookup"><span data-stu-id="5e188-121">contentData</span></span>|<span data-ttu-id="5e188-122">String</span><span class="sxs-lookup"><span data-stu-id="5e188-122">String</span></span>|<span data-ttu-id="5e188-123">Содержимое eml-файла электронной почты в коде Base64.</span><span class="sxs-lookup"><span data-stu-id="5e188-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="5e188-124">Содержимое файла не может получить обратно, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="5e188-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="5e188-125">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5e188-125">destinationRoutingReason</span></span>|[<span data-ttu-id="5e188-126">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="5e188-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="5e188-127">Причина перенаправления почты в место назначения.</span><span class="sxs-lookup"><span data-stu-id="5e188-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="5e188-128">Возможные значения: `none` , , , , , , , `mailFlowRule` , , `safeSender` , `blockedSender` `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` . `junk`</span><span class="sxs-lookup"><span data-stu-id="5e188-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="5e188-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="5e188-129">recipientEmail</span></span>|<span data-ttu-id="5e188-130">String</span><span class="sxs-lookup"><span data-stu-id="5e188-130">String</span></span>|<span data-ttu-id="5e188-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="5e188-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="5e188-132">category</span><span class="sxs-lookup"><span data-stu-id="5e188-132">category</span></span>|[<span data-ttu-id="5e188-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="5e188-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5e188-134">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="5e188-134">The threat category.</span></span> <span data-ttu-id="5e188-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5e188-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5e188-136">contentType</span><span class="sxs-lookup"><span data-stu-id="5e188-136">contentType</span></span>|[<span data-ttu-id="5e188-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="5e188-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5e188-138">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5e188-138">The content type of threat assessment.</span></span> <span data-ttu-id="5e188-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5e188-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5e188-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e188-140">createdBy</span></span>|[<span data-ttu-id="5e188-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e188-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="5e188-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5e188-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5e188-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e188-143">createdDateTime</span></span>|<span data-ttu-id="5e188-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e188-144">DateTimeOffset</span></span>|<span data-ttu-id="5e188-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5e188-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e188-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e188-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5e188-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5e188-147">expectedAssessment</span></span>|[<span data-ttu-id="5e188-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5e188-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5e188-149">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="5e188-149">The expected assessment from submitter.</span></span> <span data-ttu-id="5e188-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5e188-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5e188-151">id</span><span class="sxs-lookup"><span data-stu-id="5e188-151">id</span></span>|<span data-ttu-id="5e188-152">String</span><span class="sxs-lookup"><span data-stu-id="5e188-152">String</span></span>|<span data-ttu-id="5e188-153">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="5e188-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5e188-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="5e188-154">requestSource</span></span>|[<span data-ttu-id="5e188-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="5e188-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5e188-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5e188-156">The source of threat assessment request.</span></span> <span data-ttu-id="5e188-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5e188-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5e188-158">status</span><span class="sxs-lookup"><span data-stu-id="5e188-158">status</span></span>|[<span data-ttu-id="5e188-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="5e188-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5e188-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5e188-160">The assessment process status.</span></span> <span data-ttu-id="5e188-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5e188-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e188-162">Связи</span><span class="sxs-lookup"><span data-stu-id="5e188-162">Relationships</span></span>

| <span data-ttu-id="5e188-163">Связь</span><span class="sxs-lookup"><span data-stu-id="5e188-163">Relationship</span></span> | <span data-ttu-id="5e188-164">Тип</span><span class="sxs-lookup"><span data-stu-id="5e188-164">Type</span></span>        | <span data-ttu-id="5e188-165">Описание</span><span class="sxs-lookup"><span data-stu-id="5e188-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e188-166">results</span><span class="sxs-lookup"><span data-stu-id="5e188-166">results</span></span>|<span data-ttu-id="5e188-167">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5e188-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5e188-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5e188-168">A collection of threat assessment results.</span></span> <span data-ttu-id="5e188-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e188-169">Read-only.</span></span> <span data-ttu-id="5e188-170">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="5e188-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e188-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e188-171">JSON representation</span></span>

<span data-ttu-id="5e188-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e188-172">The following is a JSON representation of the resource.</span></span>

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


