---
title: Тип ресурса Маилассессментрекуест
description: Используется для создания и получения оценки угроз электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c684694ac2af189698c74935ca58f70aa4a8cf9f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083080"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="11cac-103">Тип ресурса Маилассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="11cac-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="11cac-104">Используется для создания и получения оценки угроз электронной почты, производных от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="11cac-104">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="11cac-105">Когда вы создаете запрос оценки угроз для электронной почты, сообщение должно быть получено пользователем, указанным в `recipientEmail` .</span><span class="sxs-lookup"><span data-stu-id="11cac-105">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="11cac-106">Делегированные [разрешения на почту](/graph/permissions-reference#mail-permissions) (mail. Read или mail. Read. shared) — рекуриед для доступа к почте, полученной пользователем или предоставленных другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="11cac-106">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="11cac-107">Методы</span><span class="sxs-lookup"><span data-stu-id="11cac-107">Methods</span></span>

| <span data-ttu-id="11cac-108">Метод</span><span class="sxs-lookup"><span data-stu-id="11cac-108">Method</span></span>       | <span data-ttu-id="11cac-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="11cac-109">Return Type</span></span> | <span data-ttu-id="11cac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="11cac-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="11cac-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="11cac-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="11cac-112">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="11cac-112">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="11cac-113">Создание запроса на оценку почты путем отправки объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="11cac-113">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="11cac-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="11cac-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="11cac-115">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="11cac-115">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="11cac-116">Чтение свойств и связей объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="11cac-116">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="11cac-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="11cac-117">Properties</span></span>

| <span data-ttu-id="11cac-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="11cac-118">Property</span></span>     | <span data-ttu-id="11cac-119">Тип</span><span class="sxs-lookup"><span data-stu-id="11cac-119">Type</span></span>        | <span data-ttu-id="11cac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11cac-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11cac-121">дестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="11cac-121">destinationRoutingReason</span></span>|[<span data-ttu-id="11cac-122">маилдестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="11cac-122">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="11cac-123">Причина, по которой почта перенаправляется в назначение.</span><span class="sxs-lookup"><span data-stu-id="11cac-123">The reason for mail routed to its destination.</span></span> <span data-ttu-id="11cac-124">Возможные значения: `none` , `mailFlowRule` ,,,,, `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` ,,, `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` , `autoPurgeToJunk` , `autoPurgeToDeleted` , `outbound` , `notJunk` , `junk` .</span><span class="sxs-lookup"><span data-stu-id="11cac-124">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="11cac-125">мессажеури</span><span class="sxs-lookup"><span data-stu-id="11cac-125">messageUri</span></span>|<span data-ttu-id="11cac-126">Строка</span><span class="sxs-lookup"><span data-stu-id="11cac-126">String</span></span>|<span data-ttu-id="11cac-127">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="11cac-127">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="11cac-128">реЦипиентемаил</span><span class="sxs-lookup"><span data-stu-id="11cac-128">recipientEmail</span></span>|<span data-ttu-id="11cac-129">Строка</span><span class="sxs-lookup"><span data-stu-id="11cac-129">String</span></span>|<span data-ttu-id="11cac-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="11cac-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="11cac-131">category</span><span class="sxs-lookup"><span data-stu-id="11cac-131">category</span></span>|[<span data-ttu-id="11cac-132">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="11cac-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="11cac-133">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="11cac-133">The threat category.</span></span> <span data-ttu-id="11cac-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="11cac-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="11cac-135">contentType</span><span class="sxs-lookup"><span data-stu-id="11cac-135">contentType</span></span>|[<span data-ttu-id="11cac-136">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="11cac-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="11cac-137">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="11cac-137">The content type of threat assessment.</span></span> <span data-ttu-id="11cac-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="11cac-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="11cac-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="11cac-139">createdBy</span></span>|[<span data-ttu-id="11cac-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="11cac-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="11cac-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="11cac-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="11cac-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11cac-142">createdDateTime</span></span>|<span data-ttu-id="11cac-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11cac-143">DateTimeOffset</span></span>|<span data-ttu-id="11cac-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="11cac-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11cac-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11cac-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="11cac-146">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="11cac-146">expectedAssessment</span></span>|[<span data-ttu-id="11cac-147">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="11cac-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="11cac-148">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="11cac-148">The expected assessment from submitter.</span></span> <span data-ttu-id="11cac-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="11cac-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="11cac-150">id</span><span class="sxs-lookup"><span data-stu-id="11cac-150">id</span></span>|<span data-ttu-id="11cac-151">Строка</span><span class="sxs-lookup"><span data-stu-id="11cac-151">String</span></span>|<span data-ttu-id="11cac-152">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="11cac-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="11cac-153">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="11cac-153">requestSource</span></span>|[<span data-ttu-id="11cac-154">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="11cac-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="11cac-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="11cac-155">The source of threat assessment request.</span></span> <span data-ttu-id="11cac-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="11cac-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="11cac-157">status</span><span class="sxs-lookup"><span data-stu-id="11cac-157">status</span></span>|[<span data-ttu-id="11cac-158">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="11cac-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="11cac-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="11cac-159">The assessment process status.</span></span> <span data-ttu-id="11cac-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="11cac-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11cac-161">Связи</span><span class="sxs-lookup"><span data-stu-id="11cac-161">Relationships</span></span>

| <span data-ttu-id="11cac-162">Связь</span><span class="sxs-lookup"><span data-stu-id="11cac-162">Relationship</span></span> | <span data-ttu-id="11cac-163">Тип</span><span class="sxs-lookup"><span data-stu-id="11cac-163">Type</span></span>        | <span data-ttu-id="11cac-164">Описание</span><span class="sxs-lookup"><span data-stu-id="11cac-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="11cac-165">results</span><span class="sxs-lookup"><span data-stu-id="11cac-165">results</span></span>|<span data-ttu-id="11cac-166">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="11cac-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="11cac-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="11cac-167">A collection of threat assessment results.</span></span> <span data-ttu-id="11cac-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11cac-168">Read-only.</span></span> <span data-ttu-id="11cac-169">По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.</span><span class="sxs-lookup"><span data-stu-id="11cac-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11cac-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11cac-170">JSON representation</span></span>

<span data-ttu-id="11cac-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11cac-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
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

