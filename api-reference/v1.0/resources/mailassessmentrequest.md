---
title: Тип ресурса mailAssessmentRequest
description: Используется для создания и извлечения оценки угрозы почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 90909c244c25658f976c9a0d756ec1ea89dbaedc
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154196"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="ef316-103">Тип ресурса mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ef316-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="ef316-104">Используется для создания и извлечения оценки угрозы почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="ef316-104">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="ef316-105">При создании запроса на оценку угроз почты сообщение должно быть получено указанным `recipientEmail` пользователем.</span><span class="sxs-lookup"><span data-stu-id="ef316-105">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="ef316-106">Делегированная почта разрешений (Mail.Read или Mail.Read.Shared) повторно приравнивается для доступа к почте, полученной пользователем или другим пользователем. [](/graph/permissions-reference#mail-permissions)</span><span class="sxs-lookup"><span data-stu-id="ef316-106">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="ef316-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ef316-107">Methods</span></span>

| <span data-ttu-id="ef316-108">Метод</span><span class="sxs-lookup"><span data-stu-id="ef316-108">Method</span></span>       | <span data-ttu-id="ef316-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ef316-109">Return Type</span></span> | <span data-ttu-id="ef316-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ef316-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ef316-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ef316-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="ef316-112">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ef316-112">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="ef316-113">Создайте новый запрос на оценку почты, опубликовав объект **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="ef316-113">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="ef316-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ef316-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="ef316-115">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ef316-115">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="ef316-116">Чтение свойств и связей объекта **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="ef316-116">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="ef316-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef316-117">Properties</span></span>

| <span data-ttu-id="ef316-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef316-118">Property</span></span>     | <span data-ttu-id="ef316-119">Тип</span><span class="sxs-lookup"><span data-stu-id="ef316-119">Type</span></span>        | <span data-ttu-id="ef316-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ef316-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ef316-121">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="ef316-121">destinationRoutingReason</span></span>|[<span data-ttu-id="ef316-122">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="ef316-122">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="ef316-123">Причина перенаправления почты в место назначения.</span><span class="sxs-lookup"><span data-stu-id="ef316-123">The reason for mail routed to its destination.</span></span> <span data-ttu-id="ef316-124">Возможные значения: `none` , , , , , , , `mailFlowRule` , , `safeSender` , `blockedSender` `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` . `junk`</span><span class="sxs-lookup"><span data-stu-id="ef316-124">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="ef316-125">messageUri</span><span class="sxs-lookup"><span data-stu-id="ef316-125">messageUri</span></span>|<span data-ttu-id="ef316-126">String</span><span class="sxs-lookup"><span data-stu-id="ef316-126">String</span></span>|<span data-ttu-id="ef316-127">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="ef316-127">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="ef316-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="ef316-128">recipientEmail</span></span>|<span data-ttu-id="ef316-129">String</span><span class="sxs-lookup"><span data-stu-id="ef316-129">String</span></span>|<span data-ttu-id="ef316-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="ef316-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="ef316-131">category</span><span class="sxs-lookup"><span data-stu-id="ef316-131">category</span></span>|[<span data-ttu-id="ef316-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="ef316-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="ef316-133">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="ef316-133">The threat category.</span></span> <span data-ttu-id="ef316-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="ef316-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="ef316-135">contentType</span><span class="sxs-lookup"><span data-stu-id="ef316-135">contentType</span></span>|[<span data-ttu-id="ef316-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="ef316-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="ef316-137">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="ef316-137">The content type of threat assessment.</span></span> <span data-ttu-id="ef316-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="ef316-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="ef316-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="ef316-139">createdBy</span></span>|[<span data-ttu-id="ef316-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef316-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="ef316-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="ef316-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="ef316-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef316-142">createdDateTime</span></span>|<span data-ttu-id="ef316-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef316-143">DateTimeOffset</span></span>|<span data-ttu-id="ef316-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ef316-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ef316-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ef316-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ef316-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="ef316-146">expectedAssessment</span></span>|[<span data-ttu-id="ef316-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="ef316-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="ef316-148">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="ef316-148">The expected assessment from submitter.</span></span> <span data-ttu-id="ef316-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="ef316-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="ef316-150">id</span><span class="sxs-lookup"><span data-stu-id="ef316-150">id</span></span>|<span data-ttu-id="ef316-151">String</span><span class="sxs-lookup"><span data-stu-id="ef316-151">String</span></span>|<span data-ttu-id="ef316-152">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="ef316-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="ef316-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="ef316-153">requestSource</span></span>|[<span data-ttu-id="ef316-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="ef316-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="ef316-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="ef316-155">The source of threat assessment request.</span></span> <span data-ttu-id="ef316-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="ef316-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="ef316-157">status</span><span class="sxs-lookup"><span data-stu-id="ef316-157">status</span></span>|[<span data-ttu-id="ef316-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="ef316-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="ef316-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="ef316-159">The assessment process status.</span></span> <span data-ttu-id="ef316-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="ef316-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef316-161">Связи</span><span class="sxs-lookup"><span data-stu-id="ef316-161">Relationships</span></span>

| <span data-ttu-id="ef316-162">Связь</span><span class="sxs-lookup"><span data-stu-id="ef316-162">Relationship</span></span> | <span data-ttu-id="ef316-163">Тип</span><span class="sxs-lookup"><span data-stu-id="ef316-163">Type</span></span>        | <span data-ttu-id="ef316-164">Описание</span><span class="sxs-lookup"><span data-stu-id="ef316-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ef316-165">results</span><span class="sxs-lookup"><span data-stu-id="ef316-165">results</span></span>|<span data-ttu-id="ef316-166">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="ef316-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="ef316-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="ef316-167">A collection of threat assessment results.</span></span> <span data-ttu-id="ef316-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef316-168">Read-only.</span></span> <span data-ttu-id="ef316-169">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="ef316-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef316-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef316-170">JSON representation</span></span>

<span data-ttu-id="ef316-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef316-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
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
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

