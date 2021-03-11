---
title: тип ресурса mailAssessmentRequest
description: Используется для создания и получения оценки угроз почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 012450bdc57c1c0f944a3dfbfa492320eb6f6d13
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721740"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="4ff4f-103">тип ресурса mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ff4f-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="4ff4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ff4f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff4f-105">Используется для создания и получения оценки угроз почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="4ff4f-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="4ff4f-106">При создании запроса на оценку угрозы почты почта должна быть получена пользователем, указанным в `recipientEmail` .</span><span class="sxs-lookup"><span data-stu-id="4ff4f-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="4ff4f-107">[Делегированная](/graph/permissions-reference#mail-permissions) почта разрешений (Mail.Read или Mail.Read.Shared) переквалифицироваться для доступа к почте, полученной пользователем или общим кем-то еще.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="4ff4f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4ff4f-108">Methods</span></span>

| <span data-ttu-id="4ff4f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4ff4f-109">Method</span></span>       | <span data-ttu-id="4ff4f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ff4f-110">Return Type</span></span> | <span data-ttu-id="4ff4f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff4f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4ff4f-112">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ff4f-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="4ff4f-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ff4f-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="4ff4f-114">Создайте новый запрос на оценку почты, разместив объект **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="4ff4f-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="4ff4f-115">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ff4f-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="4ff4f-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4ff4f-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="4ff4f-117">Ознакомьтесь с свойствами и отношениями объекта **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="4ff4f-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4ff4f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ff4f-118">Properties</span></span>

| <span data-ttu-id="4ff4f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ff4f-119">Property</span></span>     | <span data-ttu-id="4ff4f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4ff4f-120">Type</span></span>        | <span data-ttu-id="4ff4f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff4f-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ff4f-122">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="4ff4f-122">destinationRoutingReason</span></span>|[<span data-ttu-id="4ff4f-123">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="4ff4f-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="4ff4f-124">Причина направления почты в пункт назначения.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="4ff4f-125">Возможные значения: `none` `mailFlowRule` , , , , , `safeSender` , `blockedSender` , `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` , `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` , .</span><span class="sxs-lookup"><span data-stu-id="4ff4f-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="4ff4f-126">messageUri</span><span class="sxs-lookup"><span data-stu-id="4ff4f-126">messageUri</span></span>|<span data-ttu-id="4ff4f-127">String</span><span class="sxs-lookup"><span data-stu-id="4ff4f-127">String</span></span>|<span data-ttu-id="4ff4f-128">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="4ff4f-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="4ff4f-129">recipientEmail</span></span>|<span data-ttu-id="4ff4f-130">String</span><span class="sxs-lookup"><span data-stu-id="4ff4f-130">String</span></span>|<span data-ttu-id="4ff4f-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="4ff4f-132">category</span><span class="sxs-lookup"><span data-stu-id="4ff4f-132">category</span></span>|[<span data-ttu-id="4ff4f-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="4ff4f-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="4ff4f-134">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-134">The threat category.</span></span> <span data-ttu-id="4ff4f-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="4ff4f-136">contentType</span><span class="sxs-lookup"><span data-stu-id="4ff4f-136">contentType</span></span>|[<span data-ttu-id="4ff4f-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="4ff4f-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="4ff4f-138">Тип оценки угрозы контента.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-138">The content type of threat assessment.</span></span> <span data-ttu-id="4ff4f-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="4ff4f-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="4ff4f-140">createdBy</span></span>|[<span data-ttu-id="4ff4f-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="4ff4f-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="4ff4f-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="4ff4f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ff4f-143">createdDateTime</span></span>|<span data-ttu-id="4ff4f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ff4f-144">DateTimeOffset</span></span>|<span data-ttu-id="4ff4f-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4ff4f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4ff4f-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="4ff4f-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="4ff4f-147">expectedAssessment</span></span>|[<span data-ttu-id="4ff4f-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="4ff4f-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="4ff4f-149">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-149">The expected assessment from submitter.</span></span> <span data-ttu-id="4ff4f-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="4ff4f-151">id</span><span class="sxs-lookup"><span data-stu-id="4ff4f-151">id</span></span>|<span data-ttu-id="4ff4f-152">String</span><span class="sxs-lookup"><span data-stu-id="4ff4f-152">String</span></span>|<span data-ttu-id="4ff4f-153">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="4ff4f-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="4ff4f-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="4ff4f-154">requestSource</span></span>|[<span data-ttu-id="4ff4f-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="4ff4f-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="4ff4f-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-156">The source of threat assessment request.</span></span> <span data-ttu-id="4ff4f-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="4ff4f-158">status</span><span class="sxs-lookup"><span data-stu-id="4ff4f-158">status</span></span>|[<span data-ttu-id="4ff4f-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="4ff4f-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="4ff4f-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-160">The assessment process status.</span></span> <span data-ttu-id="4ff4f-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ff4f-162">Связи</span><span class="sxs-lookup"><span data-stu-id="4ff4f-162">Relationships</span></span>

| <span data-ttu-id="4ff4f-163">Связь</span><span class="sxs-lookup"><span data-stu-id="4ff4f-163">Relationship</span></span> | <span data-ttu-id="4ff4f-164">Тип</span><span class="sxs-lookup"><span data-stu-id="4ff4f-164">Type</span></span>        | <span data-ttu-id="4ff4f-165">Описание</span><span class="sxs-lookup"><span data-stu-id="4ff4f-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ff4f-166">results</span><span class="sxs-lookup"><span data-stu-id="4ff4f-166">results</span></span>|<span data-ttu-id="4ff4f-167">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="4ff4f-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="4ff4f-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-168">A collection of threat assessment results.</span></span> <span data-ttu-id="4ff4f-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-169">Read-only.</span></span> <span data-ttu-id="4ff4f-170">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ff4f-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ff4f-171">JSON representation</span></span>

<span data-ttu-id="4ff4f-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ff4f-172">The following is a JSON representation of the resource.</span></span>

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


