---
title: тип ресурса threatAssessmentRequest
description: Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угрозы.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: aeb3733ed3c93896d701851a928e216a2b9c7c7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952503"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="90532-103">тип ресурса threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="90532-104">Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="90532-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="90532-105">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="90532-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="90532-106">Почта[(ресурс mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="90532-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="90532-107">Файл электронной почты[(ресурс emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="90532-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="90532-108">Файл[(ресурс fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="90532-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="90532-109">[URL-адрес (ресурс urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="90532-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="90532-110">Методы</span><span class="sxs-lookup"><span data-stu-id="90532-110">Methods</span></span>

| <span data-ttu-id="90532-111">Метод</span><span class="sxs-lookup"><span data-stu-id="90532-111">Method</span></span>       | <span data-ttu-id="90532-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90532-112">Return Type</span></span> | <span data-ttu-id="90532-113">Описание</span><span class="sxs-lookup"><span data-stu-id="90532-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="90532-114">Перечисление объектов threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="90532-115">[коллекция threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="90532-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="90532-116">Список всех запросов на оценку угроз в клиенте.</span><span class="sxs-lookup"><span data-stu-id="90532-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="90532-117">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="90532-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="90532-119">Создайте новый запрос на оценку угрозы, разместив производный тип ресурса: [mailAssessmentRequest,](../resources/mailAssessmentRequest.md) [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="90532-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="90532-120">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="90532-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="90532-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="90532-122">Извлечение свойств и связей указанного ресурса **threatAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="90532-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="90532-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="90532-123">Properties</span></span>

| <span data-ttu-id="90532-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="90532-124">Property</span></span>     | <span data-ttu-id="90532-125">Тип</span><span class="sxs-lookup"><span data-stu-id="90532-125">Type</span></span>        | <span data-ttu-id="90532-126">Описание</span><span class="sxs-lookup"><span data-stu-id="90532-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="90532-127">category</span><span class="sxs-lookup"><span data-stu-id="90532-127">category</span></span>|[<span data-ttu-id="90532-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="90532-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="90532-129">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="90532-129">The threat category.</span></span> <span data-ttu-id="90532-130">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="90532-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="90532-131">contentType</span><span class="sxs-lookup"><span data-stu-id="90532-131">contentType</span></span>|[<span data-ttu-id="90532-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="90532-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="90532-133">Тип оценки угрозы контента.</span><span class="sxs-lookup"><span data-stu-id="90532-133">The content type of threat assessment.</span></span> <span data-ttu-id="90532-134">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="90532-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="90532-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="90532-135">createdBy</span></span>|[<span data-ttu-id="90532-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="90532-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="90532-137">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="90532-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="90532-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90532-138">createdDateTime</span></span>|<span data-ttu-id="90532-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90532-139">DateTimeOffset</span></span>|<span data-ttu-id="90532-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="90532-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90532-141">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="90532-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="90532-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="90532-142">expectedAssessment</span></span>|[<span data-ttu-id="90532-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="90532-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="90532-144">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="90532-144">The expected assessment from submitter.</span></span> <span data-ttu-id="90532-145">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="90532-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="90532-146">id</span><span class="sxs-lookup"><span data-stu-id="90532-146">id</span></span>|<span data-ttu-id="90532-147">String</span><span class="sxs-lookup"><span data-stu-id="90532-147">String</span></span>|<span data-ttu-id="90532-148">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="90532-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="90532-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="90532-149">requestSource</span></span>|[<span data-ttu-id="90532-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="90532-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="90532-151">Источник запроса на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="90532-151">The source of the threat assessment request.</span></span> <span data-ttu-id="90532-152">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="90532-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="90532-153">status</span><span class="sxs-lookup"><span data-stu-id="90532-153">status</span></span>|[<span data-ttu-id="90532-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="90532-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="90532-155">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="90532-155">The assessment process status.</span></span> <span data-ttu-id="90532-156">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="90532-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90532-157">Связи</span><span class="sxs-lookup"><span data-stu-id="90532-157">Relationships</span></span>

| <span data-ttu-id="90532-158">Связь</span><span class="sxs-lookup"><span data-stu-id="90532-158">Relationship</span></span> | <span data-ttu-id="90532-159">Тип</span><span class="sxs-lookup"><span data-stu-id="90532-159">Type</span></span>        | <span data-ttu-id="90532-160">Описание</span><span class="sxs-lookup"><span data-stu-id="90532-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="90532-161">results</span><span class="sxs-lookup"><span data-stu-id="90532-161">results</span></span>|<span data-ttu-id="90532-162">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="90532-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="90532-163">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="90532-163">A collection of threat assessment results.</span></span> <span data-ttu-id="90532-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="90532-164">Read-only.</span></span> <span data-ttu-id="90532-165">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="90532-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90532-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90532-166">JSON representation</span></span>

<span data-ttu-id="90532-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90532-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
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
  "description": "threatAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

