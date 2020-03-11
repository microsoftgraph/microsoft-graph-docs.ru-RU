---
title: Тип ресурса Маилассессментрекуест
description: Используется для создания и получения оценки угроз электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bfd9dbcb7084759350161c947a1ba4759ca0e185
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591476"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="51224-103">Тип ресурса Маилассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="51224-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="51224-104">Используется для создания и получения оценки угроз электронной почты, производных от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="51224-104">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="51224-105">Когда вы создаете запрос оценки угроз для электронной почты, сообщение должно быть получено пользователем, указанным `recipientEmail`в.</span><span class="sxs-lookup"><span data-stu-id="51224-105">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="51224-106">Делегированные [разрешения на почту](/graph/permissions-reference#mail-permissions) (mail. Read или mail. Read. shared) — рекуриед для доступа к почте, полученной пользователем или предоставленных другим пользователем.</span><span class="sxs-lookup"><span data-stu-id="51224-106">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="51224-107">Методы</span><span class="sxs-lookup"><span data-stu-id="51224-107">Methods</span></span>

| <span data-ttu-id="51224-108">Метод</span><span class="sxs-lookup"><span data-stu-id="51224-108">Method</span></span>       | <span data-ttu-id="51224-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="51224-109">Return Type</span></span> | <span data-ttu-id="51224-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51224-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="51224-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="51224-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="51224-112">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="51224-112">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="51224-113">Создание запроса на оценку почты путем отправки объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="51224-113">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="51224-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="51224-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="51224-115">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="51224-115">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="51224-116">Чтение свойств и связей объекта **маилассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="51224-116">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="51224-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="51224-117">Properties</span></span>

| <span data-ttu-id="51224-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="51224-118">Property</span></span>     | <span data-ttu-id="51224-119">Тип</span><span class="sxs-lookup"><span data-stu-id="51224-119">Type</span></span>        | <span data-ttu-id="51224-120">Описание</span><span class="sxs-lookup"><span data-stu-id="51224-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51224-121">дестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="51224-121">destinationRoutingReason</span></span>|[<span data-ttu-id="51224-122">маилдестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="51224-122">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="51224-123">Причина, по которой почта перенаправляется в назначение.</span><span class="sxs-lookup"><span data-stu-id="51224-123">The reason for mail routed to its destination.</span></span> <span data-ttu-id="51224-124">Возможные значения: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`,. `junk`</span><span class="sxs-lookup"><span data-stu-id="51224-124">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="51224-125">мессажеури</span><span class="sxs-lookup"><span data-stu-id="51224-125">messageUri</span></span>|<span data-ttu-id="51224-126">String</span><span class="sxs-lookup"><span data-stu-id="51224-126">String</span></span>|<span data-ttu-id="51224-127">URI ресурса почтового сообщения для оценки.</span><span class="sxs-lookup"><span data-stu-id="51224-127">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="51224-128">реЦипиентемаил</span><span class="sxs-lookup"><span data-stu-id="51224-128">recipientEmail</span></span>|<span data-ttu-id="51224-129">String</span><span class="sxs-lookup"><span data-stu-id="51224-129">String</span></span>|<span data-ttu-id="51224-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="51224-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="51224-131">category</span><span class="sxs-lookup"><span data-stu-id="51224-131">category</span></span>|[<span data-ttu-id="51224-132">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="51224-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="51224-133">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="51224-133">The threat category.</span></span> <span data-ttu-id="51224-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="51224-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="51224-135">contentType</span><span class="sxs-lookup"><span data-stu-id="51224-135">contentType</span></span>|[<span data-ttu-id="51224-136">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="51224-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="51224-137">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="51224-137">The content type of threat assessment.</span></span> <span data-ttu-id="51224-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="51224-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="51224-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="51224-139">createdBy</span></span>|[<span data-ttu-id="51224-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="51224-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="51224-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="51224-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="51224-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51224-142">createdDateTime</span></span>|<span data-ttu-id="51224-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51224-143">DateTimeOffset</span></span>|<span data-ttu-id="51224-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="51224-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="51224-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="51224-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="51224-146">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="51224-146">expectedAssessment</span></span>|[<span data-ttu-id="51224-147">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="51224-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="51224-148">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="51224-148">The expected assessment from submitter.</span></span> <span data-ttu-id="51224-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="51224-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="51224-150">id</span><span class="sxs-lookup"><span data-stu-id="51224-150">id</span></span>|<span data-ttu-id="51224-151">String</span><span class="sxs-lookup"><span data-stu-id="51224-151">String</span></span>|<span data-ttu-id="51224-152">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="51224-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="51224-153">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="51224-153">requestSource</span></span>|[<span data-ttu-id="51224-154">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="51224-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="51224-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="51224-155">The source of threat assessment request.</span></span> <span data-ttu-id="51224-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="51224-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="51224-157">status</span><span class="sxs-lookup"><span data-stu-id="51224-157">status</span></span>|[<span data-ttu-id="51224-158">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="51224-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="51224-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="51224-159">The assessment process status.</span></span> <span data-ttu-id="51224-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="51224-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51224-161">Связи</span><span class="sxs-lookup"><span data-stu-id="51224-161">Relationships</span></span>

| <span data-ttu-id="51224-162">Связь</span><span class="sxs-lookup"><span data-stu-id="51224-162">Relationship</span></span> | <span data-ttu-id="51224-163">Тип</span><span class="sxs-lookup"><span data-stu-id="51224-163">Type</span></span>        | <span data-ttu-id="51224-164">Описание</span><span class="sxs-lookup"><span data-stu-id="51224-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51224-165">results</span><span class="sxs-lookup"><span data-stu-id="51224-165">results</span></span>|<span data-ttu-id="51224-166">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="51224-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="51224-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="51224-167">A collection of threat assessment results.</span></span> <span data-ttu-id="51224-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="51224-168">Read-only.</span></span> <span data-ttu-id="51224-169">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="51224-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51224-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51224-170">JSON representation</span></span>

<span data-ttu-id="51224-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51224-171">The following is a JSON representation of the resource.</span></span>

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
