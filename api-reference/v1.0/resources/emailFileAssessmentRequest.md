---
title: Тип ресурса Емаилфилеассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 29cb2f2f573f735504d2b54d4449109f82541f95
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591462"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="cd7a9-103">Тип ресурса Емаилфилеассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="cd7a9-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="cd7a9-104">Используется для создания и извлечения средства оценки угроз для файла электронной почты, производного от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="cd7a9-104">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="cd7a9-105">Файл электронной почты может иметь тип EML.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-105">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="cd7a9-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cd7a9-106">Methods</span></span>

| <span data-ttu-id="cd7a9-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cd7a9-107">Method</span></span>       | <span data-ttu-id="cd7a9-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cd7a9-108">Return Type</span></span> | <span data-ttu-id="cd7a9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cd7a9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cd7a9-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd7a9-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="cd7a9-111">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd7a9-111">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="cd7a9-112">Создание нового запроса на оценку файла электронной почты путем отправки объекта **емаилфилеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="cd7a9-112">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="cd7a9-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd7a9-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="cd7a9-114">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="cd7a9-114">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="cd7a9-115">Чтение свойств и связей объекта **емаилфилеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="cd7a9-115">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cd7a9-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd7a9-116">Properties</span></span>

| <span data-ttu-id="cd7a9-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd7a9-117">Property</span></span>     | <span data-ttu-id="cd7a9-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cd7a9-118">Type</span></span>        | <span data-ttu-id="cd7a9-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cd7a9-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd7a9-120">контентдата</span><span class="sxs-lookup"><span data-stu-id="cd7a9-120">contentData</span></span>|<span data-ttu-id="cd7a9-121">String</span><span class="sxs-lookup"><span data-stu-id="cd7a9-121">String</span></span>|<span data-ttu-id="cd7a9-122">Содержимое файла электронной почты в кодировке Base64. EML.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-122">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="cd7a9-123">Не удается вернуть содержимое файла, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="cd7a9-124">дестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="cd7a9-124">destinationRoutingReason</span></span>|[<span data-ttu-id="cd7a9-125">маилдестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="cd7a9-125">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="cd7a9-126">Причина, по которой почта перенаправляется в назначение.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-126">The reason for mail routed to its destination.</span></span> <span data-ttu-id="cd7a9-127">Возможные значения: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`,. `junk`</span><span class="sxs-lookup"><span data-stu-id="cd7a9-127">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="cd7a9-128">реЦипиентемаил</span><span class="sxs-lookup"><span data-stu-id="cd7a9-128">recipientEmail</span></span>|<span data-ttu-id="cd7a9-129">String</span><span class="sxs-lookup"><span data-stu-id="cd7a9-129">String</span></span>|<span data-ttu-id="cd7a9-130">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="cd7a9-131">category</span><span class="sxs-lookup"><span data-stu-id="cd7a9-131">category</span></span>|[<span data-ttu-id="cd7a9-132">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="cd7a9-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="cd7a9-133">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-133">The threat category.</span></span> <span data-ttu-id="cd7a9-134">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="cd7a9-135">contentType</span><span class="sxs-lookup"><span data-stu-id="cd7a9-135">contentType</span></span>|[<span data-ttu-id="cd7a9-136">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="cd7a9-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="cd7a9-137">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-137">The content type of threat assessment.</span></span> <span data-ttu-id="cd7a9-138">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="cd7a9-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="cd7a9-139">createdBy</span></span>|[<span data-ttu-id="cd7a9-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="cd7a9-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="cd7a9-141">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="cd7a9-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cd7a9-142">createdDateTime</span></span>|<span data-ttu-id="cd7a9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cd7a9-143">DateTimeOffset</span></span>|<span data-ttu-id="cd7a9-144">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="cd7a9-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cd7a9-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="cd7a9-146">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="cd7a9-146">expectedAssessment</span></span>|[<span data-ttu-id="cd7a9-147">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="cd7a9-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="cd7a9-148">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-148">The expected assessment from submitter.</span></span> <span data-ttu-id="cd7a9-149">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="cd7a9-150">id</span><span class="sxs-lookup"><span data-stu-id="cd7a9-150">id</span></span>|<span data-ttu-id="cd7a9-151">String</span><span class="sxs-lookup"><span data-stu-id="cd7a9-151">String</span></span>|<span data-ttu-id="cd7a9-152">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="cd7a9-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="cd7a9-153">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="cd7a9-153">requestSource</span></span>|[<span data-ttu-id="cd7a9-154">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="cd7a9-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="cd7a9-155">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-155">The source of threat assessment request.</span></span> <span data-ttu-id="cd7a9-156">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="cd7a9-157">status</span><span class="sxs-lookup"><span data-stu-id="cd7a9-157">status</span></span>|[<span data-ttu-id="cd7a9-158">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="cd7a9-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="cd7a9-159">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-159">The assessment process status.</span></span> <span data-ttu-id="cd7a9-160">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd7a9-161">Связи</span><span class="sxs-lookup"><span data-stu-id="cd7a9-161">Relationships</span></span>

| <span data-ttu-id="cd7a9-162">Связь</span><span class="sxs-lookup"><span data-stu-id="cd7a9-162">Relationship</span></span> | <span data-ttu-id="cd7a9-163">Тип</span><span class="sxs-lookup"><span data-stu-id="cd7a9-163">Type</span></span>        | <span data-ttu-id="cd7a9-164">Описание</span><span class="sxs-lookup"><span data-stu-id="cd7a9-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cd7a9-165">results</span><span class="sxs-lookup"><span data-stu-id="cd7a9-165">results</span></span>|<span data-ttu-id="cd7a9-166">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="cd7a9-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="cd7a9-167">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-167">A collection of threat assessment results.</span></span> <span data-ttu-id="cd7a9-168">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-168">Read-only.</span></span> <span data-ttu-id="cd7a9-169">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd7a9-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd7a9-170">JSON representation</span></span>

<span data-ttu-id="cd7a9-171">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd7a9-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "",
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
