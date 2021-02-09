---
title: Тип ресурса mailAssessmentRequest
description: Используется для создания и извлечения оценки угрозы почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9ea2a227b414317942b0c0ea48109f0056543a60
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161434"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="4be73-103">Тип ресурса mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4be73-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="4be73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4be73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4be73-105">Используется для создания и извлечения оценки угрозы почты, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="4be73-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="4be73-106">При создании запроса на оценку угроз почты сообщение должно быть получено указанным `recipientEmail` пользователем.</span><span class="sxs-lookup"><span data-stu-id="4be73-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="4be73-107">Делегированная почта разрешений (Mail.Read или Mail.Read.Shared) повторно приравнивается для доступа к почте, полученной пользователем или другим пользователем. [](/graph/permissions-reference#mail-permissions)</span><span class="sxs-lookup"><span data-stu-id="4be73-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="4be73-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4be73-108">Methods</span></span>

| <span data-ttu-id="4be73-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4be73-109">Method</span></span>       | <span data-ttu-id="4be73-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4be73-110">Return Type</span></span> | <span data-ttu-id="4be73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4be73-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4be73-112">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4be73-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="4be73-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4be73-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="4be73-114">Создайте новый запрос на оценку почты, опубликовав объект **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="4be73-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="4be73-115">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4be73-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="4be73-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="4be73-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="4be73-117">Чтение свойств и связей объекта **mailAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="4be73-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4be73-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="4be73-118">Properties</span></span>

| <span data-ttu-id="4be73-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="4be73-119">Property</span></span>     | <span data-ttu-id="4be73-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4be73-120">Type</span></span>        | <span data-ttu-id="4be73-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4be73-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4be73-122">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="4be73-122">destinationRoutingReason</span></span>|[<span data-ttu-id="4be73-123">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="4be73-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="4be73-124">Причина перенаправления почты в место назначения.</span><span class="sxs-lookup"><span data-stu-id="4be73-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="4be73-125">Возможные значения: `none` , , , , , , , `mailFlowRule` , , `safeSender` , `blockedSender` `advancedSpamFiltering` , `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` . `junk`</span><span class="sxs-lookup"><span data-stu-id="4be73-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="4be73-126">messageUri</span><span class="sxs-lookup"><span data-stu-id="4be73-126">messageUri</span></span>|<span data-ttu-id="4be73-127">String</span><span class="sxs-lookup"><span data-stu-id="4be73-127">String</span></span>|<span data-ttu-id="4be73-128">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="4be73-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="4be73-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="4be73-129">recipientEmail</span></span>|<span data-ttu-id="4be73-130">String</span><span class="sxs-lookup"><span data-stu-id="4be73-130">String</span></span>|<span data-ttu-id="4be73-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="4be73-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="4be73-132">category</span><span class="sxs-lookup"><span data-stu-id="4be73-132">category</span></span>|[<span data-ttu-id="4be73-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="4be73-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="4be73-134">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="4be73-134">The threat category.</span></span> <span data-ttu-id="4be73-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="4be73-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="4be73-136">contentType</span><span class="sxs-lookup"><span data-stu-id="4be73-136">contentType</span></span>|[<span data-ttu-id="4be73-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="4be73-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="4be73-138">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="4be73-138">The content type of threat assessment.</span></span> <span data-ttu-id="4be73-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="4be73-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="4be73-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="4be73-140">createdBy</span></span>|[<span data-ttu-id="4be73-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="4be73-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="4be73-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="4be73-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="4be73-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4be73-143">createdDateTime</span></span>|<span data-ttu-id="4be73-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4be73-144">DateTimeOffset</span></span>|<span data-ttu-id="4be73-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4be73-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4be73-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4be73-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="4be73-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="4be73-147">expectedAssessment</span></span>|[<span data-ttu-id="4be73-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="4be73-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="4be73-149">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="4be73-149">The expected assessment from submitter.</span></span> <span data-ttu-id="4be73-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="4be73-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="4be73-151">id</span><span class="sxs-lookup"><span data-stu-id="4be73-151">id</span></span>|<span data-ttu-id="4be73-152">String</span><span class="sxs-lookup"><span data-stu-id="4be73-152">String</span></span>|<span data-ttu-id="4be73-153">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="4be73-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="4be73-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="4be73-154">requestSource</span></span>|[<span data-ttu-id="4be73-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="4be73-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="4be73-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="4be73-156">The source of threat assessment request.</span></span> <span data-ttu-id="4be73-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="4be73-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="4be73-158">status</span><span class="sxs-lookup"><span data-stu-id="4be73-158">status</span></span>|[<span data-ttu-id="4be73-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="4be73-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="4be73-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="4be73-160">The assessment process status.</span></span> <span data-ttu-id="4be73-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="4be73-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4be73-162">Связи</span><span class="sxs-lookup"><span data-stu-id="4be73-162">Relationships</span></span>

| <span data-ttu-id="4be73-163">Связь</span><span class="sxs-lookup"><span data-stu-id="4be73-163">Relationship</span></span> | <span data-ttu-id="4be73-164">Тип</span><span class="sxs-lookup"><span data-stu-id="4be73-164">Type</span></span>        | <span data-ttu-id="4be73-165">Описание</span><span class="sxs-lookup"><span data-stu-id="4be73-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4be73-166">results</span><span class="sxs-lookup"><span data-stu-id="4be73-166">results</span></span>|<span data-ttu-id="4be73-167">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="4be73-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="4be73-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="4be73-168">A collection of threat assessment results.</span></span> <span data-ttu-id="4be73-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4be73-169">Read-only.</span></span> <span data-ttu-id="4be73-170">По умолчанию объект a `GET /threatAssessmentRequests/{id}` не возвращает это свойство, если к этому свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="4be73-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4be73-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4be73-171">JSON representation</span></span>

<span data-ttu-id="4be73-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4be73-172">The following is a JSON representation of the resource.</span></span>

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


