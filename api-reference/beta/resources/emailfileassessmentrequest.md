---
title: Тип ресурса Емаилфилеассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для файла электронной почты.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 848ba0e1d7bfae16270f12d5acb153c083ca1d06
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989572"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="6acae-103">Тип ресурса Емаилфилеассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="6acae-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="6acae-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6acae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6acae-105">Используется для создания и извлечения средства оценки угроз для файла электронной почты, производного от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="6acae-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="6acae-106">Файл электронной почты может иметь тип EML.</span><span class="sxs-lookup"><span data-stu-id="6acae-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="6acae-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6acae-107">Methods</span></span>

| <span data-ttu-id="6acae-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6acae-108">Method</span></span>       | <span data-ttu-id="6acae-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6acae-109">Return Type</span></span> | <span data-ttu-id="6acae-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6acae-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6acae-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6acae-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="6acae-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6acae-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="6acae-113">Создание нового запроса на оценку файла электронной почты путем отправки объекта **емаилфилеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="6acae-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="6acae-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6acae-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="6acae-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="6acae-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="6acae-116">Чтение свойств и связей объекта **емаилфилеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="6acae-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6acae-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6acae-117">Properties</span></span>

| <span data-ttu-id="6acae-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="6acae-118">Property</span></span>     | <span data-ttu-id="6acae-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6acae-119">Type</span></span>        | <span data-ttu-id="6acae-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6acae-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6acae-121">контентдата</span><span class="sxs-lookup"><span data-stu-id="6acae-121">contentData</span></span>|<span data-ttu-id="6acae-122">String</span><span class="sxs-lookup"><span data-stu-id="6acae-122">String</span></span>|<span data-ttu-id="6acae-123">Содержимое файла электронной почты в кодировке Base64. EML.</span><span class="sxs-lookup"><span data-stu-id="6acae-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="6acae-124">Не удается вернуть содержимое файла, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="6acae-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="6acae-125">дестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="6acae-125">destinationRoutingReason</span></span>|[<span data-ttu-id="6acae-126">маилдестинатионраутингреасон</span><span class="sxs-lookup"><span data-stu-id="6acae-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="6acae-127">Причина, по которой почта перенаправляется в назначение.</span><span class="sxs-lookup"><span data-stu-id="6acae-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="6acae-128">Возможные значения: `none` , `mailFlowRule` ,,,,, `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` ,,, `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` , `autoPurgeToJunk` , `autoPurgeToDeleted` , `outbound` , `notJunk` , `junk` .</span><span class="sxs-lookup"><span data-stu-id="6acae-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="6acae-129">реЦипиентемаил</span><span class="sxs-lookup"><span data-stu-id="6acae-129">recipientEmail</span></span>|<span data-ttu-id="6acae-130">String</span><span class="sxs-lookup"><span data-stu-id="6acae-130">String</span></span>|<span data-ttu-id="6acae-131">Получатель почты, политики которого используются для оценки почты.</span><span class="sxs-lookup"><span data-stu-id="6acae-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="6acae-132">category</span><span class="sxs-lookup"><span data-stu-id="6acae-132">category</span></span>|[<span data-ttu-id="6acae-133">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="6acae-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="6acae-134">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="6acae-134">The threat category.</span></span> <span data-ttu-id="6acae-135">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="6acae-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="6acae-136">contentType</span><span class="sxs-lookup"><span data-stu-id="6acae-136">contentType</span></span>|[<span data-ttu-id="6acae-137">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="6acae-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="6acae-138">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="6acae-138">The content type of threat assessment.</span></span> <span data-ttu-id="6acae-139">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="6acae-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="6acae-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="6acae-140">createdBy</span></span>|[<span data-ttu-id="6acae-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="6acae-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="6acae-142">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="6acae-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="6acae-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6acae-143">createdDateTime</span></span>|<span data-ttu-id="6acae-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6acae-144">DateTimeOffset</span></span>|<span data-ttu-id="6acae-145">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="6acae-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6acae-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="6acae-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="6acae-147">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="6acae-147">expectedAssessment</span></span>|[<span data-ttu-id="6acae-148">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="6acae-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="6acae-149">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="6acae-149">The expected assessment from submitter.</span></span> <span data-ttu-id="6acae-150">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="6acae-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="6acae-151">id</span><span class="sxs-lookup"><span data-stu-id="6acae-151">id</span></span>|<span data-ttu-id="6acae-152">String</span><span class="sxs-lookup"><span data-stu-id="6acae-152">String</span></span>|<span data-ttu-id="6acae-153">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="6acae-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="6acae-154">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="6acae-154">requestSource</span></span>|[<span data-ttu-id="6acae-155">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="6acae-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="6acae-156">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="6acae-156">The source of threat assessment request.</span></span> <span data-ttu-id="6acae-157">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="6acae-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="6acae-158">status</span><span class="sxs-lookup"><span data-stu-id="6acae-158">status</span></span>|[<span data-ttu-id="6acae-159">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="6acae-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="6acae-160">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="6acae-160">The assessment process status.</span></span> <span data-ttu-id="6acae-161">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="6acae-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6acae-162">Связи</span><span class="sxs-lookup"><span data-stu-id="6acae-162">Relationships</span></span>

| <span data-ttu-id="6acae-163">Связь</span><span class="sxs-lookup"><span data-stu-id="6acae-163">Relationship</span></span> | <span data-ttu-id="6acae-164">Тип</span><span class="sxs-lookup"><span data-stu-id="6acae-164">Type</span></span>        | <span data-ttu-id="6acae-165">Описание</span><span class="sxs-lookup"><span data-stu-id="6acae-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6acae-166">results</span><span class="sxs-lookup"><span data-stu-id="6acae-166">results</span></span>|<span data-ttu-id="6acae-167">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="6acae-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="6acae-168">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="6acae-168">A collection of threat assessment results.</span></span> <span data-ttu-id="6acae-169">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6acae-169">Read-only.</span></span> <span data-ttu-id="6acae-170">По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.</span><span class="sxs-lookup"><span data-stu-id="6acae-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6acae-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6acae-171">JSON representation</span></span>

<span data-ttu-id="6acae-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6acae-172">The following is a JSON representation of the resource.</span></span>

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


