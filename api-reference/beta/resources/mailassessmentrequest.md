---
title: Тип ресурса Маилассессментрекуест
description: Используется для создания и получения оценки угроз электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 959c9a15fe96012dd586ef8fa67daa07626a76d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095027"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="e7943-103">Тип ресурса Маилассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="e7943-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="e7943-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7943-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7943-105">Используется для создания и получения оценки угроз электронной почты, производных от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="e7943-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="e7943-106">Когда вы создаете запрос оценки угроз для электронной почты, сообщение должно быть получено пользователем, указанным в `recipientEmail` .</span><span class="sxs-lookup"><span data-stu-id="e7943-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="e7943-107">Делегированные [разрешения на почту](/graph/permissions-reference#mail-permissions) (mail. Read или mail. Read. shared) — рекуриед для доступа к почте, полученной пользователем или предоставленных другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="e7943-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="e7943-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e7943-108">Methods</span></span>

| <span data-ttu-id="e7943-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e7943-109">Method</span></span>       | <span data-ttu-id="e7943-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e7943-110">Return Type</span></span> | <span data-ttu-id="e7943-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7943-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e7943-112">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e7943-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="e7943-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e7943-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="e7943-114">Создание запроса на оценку почты путем отправки объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="e7943-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="e7943-115">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e7943-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="e7943-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e7943-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="e7943-117">Чтение свойств и связей объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="e7943-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="e7943-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7943-118">Properties</span></span>

| <span data-ttu-id="e7943-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7943-119">Property</span></span>     | <span data-ttu-id="e7943-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e7943-120">Type</span></span>        | <span data-ttu-id="e7943-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e7943-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7943-122">дестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="e7943-122">destinationRoutingReason</span></span>|[<span data-ttu-id="e7943-123">маилдестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="e7943-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="e7943-124">Причина, по которой почта перенаправляется в назначение.</span><span class="sxs-lookup"><span data-stu-id="e7943-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="e7943-125">Возможные значения: `none` , `mailFlowRule` ,,,,, `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` ,,, `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` , `autoPurgeToJunk` , `autoPurgeToDeleted` , `outbound` , `notJunk` , `junk` .</span><span class="sxs-lookup"><span data-stu-id="e7943-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="e7943-126">мессажеури</span><span class="sxs-lookup"><span data-stu-id="e7943-126">messageUri</span></span>|<span data-ttu-id="e7943-127">Строка</span><span class="sxs-lookup"><span data-stu-id="e7943-127">String</span></span>|<span data-ttu-id="e7943-128">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="e7943-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="e7943-129">реЦипиентемаил</span><span class="sxs-lookup"><span data-stu-id="e7943-129">recipientEmail</span></span>|<span data-ttu-id="e7943-130">Строка</span><span class="sxs-lookup"><span data-stu-id="e7943-130">String</span></span>|<span data-ttu-id="e7943-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="e7943-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="e7943-132">category</span><span class="sxs-lookup"><span data-stu-id="e7943-132">category</span></span>|[<span data-ttu-id="e7943-133">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="e7943-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="e7943-134">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="e7943-134">The threat category.</span></span> <span data-ttu-id="e7943-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="e7943-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="e7943-136">contentType</span><span class="sxs-lookup"><span data-stu-id="e7943-136">contentType</span></span>|[<span data-ttu-id="e7943-137">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="e7943-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="e7943-138">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="e7943-138">The content type of threat assessment.</span></span> <span data-ttu-id="e7943-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="e7943-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="e7943-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="e7943-140">createdBy</span></span>|[<span data-ttu-id="e7943-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="e7943-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="e7943-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e7943-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="e7943-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7943-143">createdDateTime</span></span>|<span data-ttu-id="e7943-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7943-144">DateTimeOffset</span></span>|<span data-ttu-id="e7943-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e7943-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e7943-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e7943-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e7943-147">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="e7943-147">expectedAssessment</span></span>|[<span data-ttu-id="e7943-148">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="e7943-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="e7943-149">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="e7943-149">The expected assessment from submitter.</span></span> <span data-ttu-id="e7943-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="e7943-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="e7943-151">id</span><span class="sxs-lookup"><span data-stu-id="e7943-151">id</span></span>|<span data-ttu-id="e7943-152">Строка</span><span class="sxs-lookup"><span data-stu-id="e7943-152">String</span></span>|<span data-ttu-id="e7943-153">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="e7943-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e7943-154">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="e7943-154">requestSource</span></span>|[<span data-ttu-id="e7943-155">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="e7943-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="e7943-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e7943-156">The source of threat assessment request.</span></span> <span data-ttu-id="e7943-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e7943-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="e7943-158">status</span><span class="sxs-lookup"><span data-stu-id="e7943-158">status</span></span>|[<span data-ttu-id="e7943-159">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="e7943-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="e7943-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="e7943-160">The assessment process status.</span></span> <span data-ttu-id="e7943-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="e7943-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7943-162">Связи</span><span class="sxs-lookup"><span data-stu-id="e7943-162">Relationships</span></span>

| <span data-ttu-id="e7943-163">Связь</span><span class="sxs-lookup"><span data-stu-id="e7943-163">Relationship</span></span> | <span data-ttu-id="e7943-164">Тип</span><span class="sxs-lookup"><span data-stu-id="e7943-164">Type</span></span>        | <span data-ttu-id="e7943-165">Описание</span><span class="sxs-lookup"><span data-stu-id="e7943-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e7943-166">results</span><span class="sxs-lookup"><span data-stu-id="e7943-166">results</span></span>|<span data-ttu-id="e7943-167">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="e7943-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="e7943-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="e7943-168">A collection of threat assessment results.</span></span> <span data-ttu-id="e7943-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e7943-169">Read-only.</span></span> <span data-ttu-id="e7943-170">По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.</span><span class="sxs-lookup"><span data-stu-id="e7943-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7943-171">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7943-171">JSON representation</span></span>

<span data-ttu-id="e7943-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7943-172">The following is a JSON representation of the resource.</span></span>

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


