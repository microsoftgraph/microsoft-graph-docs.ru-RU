---
title: тип ресурса urlAssessmentRequest
description: Используется для создания и получения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: e180d09c2e76b817d2022a7de993b7a98db48d3d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941388"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="5a11d-103">тип ресурса urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a11d-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="5a11d-104">Используется для создания и получения оценки угроз URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5a11d-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5a11d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="5a11d-105">Methods</span></span>

| <span data-ttu-id="5a11d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="5a11d-106">Method</span></span>       | <span data-ttu-id="5a11d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a11d-107">Return Type</span></span> | <span data-ttu-id="5a11d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5a11d-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5a11d-109">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a11d-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5a11d-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a11d-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="5a11d-111">Создайте новый запрос на оценку URL-адресов, разместив **объект urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5a11d-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="5a11d-112">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a11d-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5a11d-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a11d-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="5a11d-114">Ознакомьтесь с свойствами и отношениями объекта **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5a11d-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a11d-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a11d-115">Properties</span></span>

| <span data-ttu-id="5a11d-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a11d-116">Property</span></span>     | <span data-ttu-id="5a11d-117">Тип</span><span class="sxs-lookup"><span data-stu-id="5a11d-117">Type</span></span>        | <span data-ttu-id="5a11d-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5a11d-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a11d-119">url</span><span class="sxs-lookup"><span data-stu-id="5a11d-119">url</span></span>|<span data-ttu-id="5a11d-120">String</span><span class="sxs-lookup"><span data-stu-id="5a11d-120">String</span></span>|<span data-ttu-id="5a11d-121">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="5a11d-121">The URL string.</span></span>|
|<span data-ttu-id="5a11d-122">category</span><span class="sxs-lookup"><span data-stu-id="5a11d-122">category</span></span>|[<span data-ttu-id="5a11d-123">threatCategory</span><span class="sxs-lookup"><span data-stu-id="5a11d-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5a11d-124">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="5a11d-124">The threat category.</span></span> <span data-ttu-id="5a11d-125">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5a11d-126">contentType</span><span class="sxs-lookup"><span data-stu-id="5a11d-126">contentType</span></span>|[<span data-ttu-id="5a11d-127">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="5a11d-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5a11d-128">Тип контента оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="5a11d-128">The content type of the threat assessment.</span></span> <span data-ttu-id="5a11d-129">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5a11d-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a11d-130">createdBy</span></span>|[<span data-ttu-id="5a11d-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a11d-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="5a11d-132">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5a11d-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5a11d-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a11d-133">createdDateTime</span></span>|<span data-ttu-id="5a11d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a11d-134">DateTimeOffset</span></span>|<span data-ttu-id="5a11d-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5a11d-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a11d-136">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="5a11d-137">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5a11d-137">expectedAssessment</span></span>|[<span data-ttu-id="5a11d-138">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5a11d-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5a11d-139">Ожидаемая оценка от ubmitter.</span><span class="sxs-lookup"><span data-stu-id="5a11d-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="5a11d-140">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5a11d-141">id</span><span class="sxs-lookup"><span data-stu-id="5a11d-141">id</span></span>|<span data-ttu-id="5a11d-142">Строка</span><span class="sxs-lookup"><span data-stu-id="5a11d-142">String</span></span>|<span data-ttu-id="5a11d-143">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="5a11d-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5a11d-144">requestSource</span><span class="sxs-lookup"><span data-stu-id="5a11d-144">requestSource</span></span>|[<span data-ttu-id="5a11d-145">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="5a11d-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5a11d-146">Источник запроса на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="5a11d-146">The source of the threat assessment request.</span></span> <span data-ttu-id="5a11d-147">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5a11d-148">status</span><span class="sxs-lookup"><span data-stu-id="5a11d-148">status</span></span>|[<span data-ttu-id="5a11d-149">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="5a11d-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5a11d-150">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5a11d-150">The assessment process status.</span></span> <span data-ttu-id="5a11d-151">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5a11d-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a11d-152">Связи</span><span class="sxs-lookup"><span data-stu-id="5a11d-152">Relationships</span></span>

| <span data-ttu-id="5a11d-153">Связь</span><span class="sxs-lookup"><span data-stu-id="5a11d-153">Relationship</span></span> | <span data-ttu-id="5a11d-154">Тип</span><span class="sxs-lookup"><span data-stu-id="5a11d-154">Type</span></span>        | <span data-ttu-id="5a11d-155">Описание</span><span class="sxs-lookup"><span data-stu-id="5a11d-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a11d-156">results</span><span class="sxs-lookup"><span data-stu-id="5a11d-156">results</span></span>|<span data-ttu-id="5a11d-157">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a11d-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5a11d-158">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5a11d-158">A collection of threat assessment results.</span></span> <span data-ttu-id="5a11d-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a11d-159">Read-only.</span></span> <span data-ttu-id="5a11d-160">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="5a11d-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a11d-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a11d-161">JSON representation</span></span>

<span data-ttu-id="5a11d-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a11d-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "url": "String",
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
  "description": "urlAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

