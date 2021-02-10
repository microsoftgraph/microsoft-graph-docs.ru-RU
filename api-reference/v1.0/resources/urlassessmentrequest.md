---
title: Тип ресурса urlAssessmentRequest
description: Используется для создания и извлечения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7046d322a351834a6271d4349c3964607312af85
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156653"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="13e33-103">Тип ресурса urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="13e33-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="13e33-104">Используется для создания и извлечения оценки угрозы URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="13e33-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="13e33-105">Методы</span><span class="sxs-lookup"><span data-stu-id="13e33-105">Methods</span></span>

| <span data-ttu-id="13e33-106">Метод</span><span class="sxs-lookup"><span data-stu-id="13e33-106">Method</span></span>       | <span data-ttu-id="13e33-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="13e33-107">Return Type</span></span> | <span data-ttu-id="13e33-108">Описание</span><span class="sxs-lookup"><span data-stu-id="13e33-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="13e33-109">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="13e33-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="13e33-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="13e33-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="13e33-111">Создайте новый запрос на оценку URL-адреса, опубликовав объект **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="13e33-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="13e33-112">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="13e33-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="13e33-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="13e33-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="13e33-114">Чтение свойств и связей объекта **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="13e33-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="13e33-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="13e33-115">Properties</span></span>

| <span data-ttu-id="13e33-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="13e33-116">Property</span></span>     | <span data-ttu-id="13e33-117">Тип</span><span class="sxs-lookup"><span data-stu-id="13e33-117">Type</span></span>        | <span data-ttu-id="13e33-118">Описание</span><span class="sxs-lookup"><span data-stu-id="13e33-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13e33-119">url</span><span class="sxs-lookup"><span data-stu-id="13e33-119">url</span></span>|<span data-ttu-id="13e33-120">String</span><span class="sxs-lookup"><span data-stu-id="13e33-120">String</span></span>|<span data-ttu-id="13e33-121">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="13e33-121">The URL string.</span></span>|
|<span data-ttu-id="13e33-122">category</span><span class="sxs-lookup"><span data-stu-id="13e33-122">category</span></span>|[<span data-ttu-id="13e33-123">threatCategory</span><span class="sxs-lookup"><span data-stu-id="13e33-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="13e33-124">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="13e33-124">The threat category.</span></span> <span data-ttu-id="13e33-125">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="13e33-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="13e33-126">contentType</span><span class="sxs-lookup"><span data-stu-id="13e33-126">contentType</span></span>|[<span data-ttu-id="13e33-127">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="13e33-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="13e33-128">Тип контента оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="13e33-128">The content type of the threat assessment.</span></span> <span data-ttu-id="13e33-129">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="13e33-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="13e33-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="13e33-130">createdBy</span></span>|[<span data-ttu-id="13e33-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="13e33-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="13e33-132">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="13e33-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="13e33-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="13e33-133">createdDateTime</span></span>|<span data-ttu-id="13e33-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13e33-134">DateTimeOffset</span></span>|<span data-ttu-id="13e33-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="13e33-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="13e33-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="13e33-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="13e33-137">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="13e33-137">expectedAssessment</span></span>|[<span data-ttu-id="13e33-138">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="13e33-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="13e33-139">Ожидаемая оценка от ubmitter.</span><span class="sxs-lookup"><span data-stu-id="13e33-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="13e33-140">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="13e33-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="13e33-141">id</span><span class="sxs-lookup"><span data-stu-id="13e33-141">id</span></span>|<span data-ttu-id="13e33-142">String</span><span class="sxs-lookup"><span data-stu-id="13e33-142">String</span></span>|<span data-ttu-id="13e33-143">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="13e33-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="13e33-144">requestSource</span><span class="sxs-lookup"><span data-stu-id="13e33-144">requestSource</span></span>|[<span data-ttu-id="13e33-145">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="13e33-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="13e33-146">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="13e33-146">The source of the threat assessment request.</span></span> <span data-ttu-id="13e33-147">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="13e33-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="13e33-148">status</span><span class="sxs-lookup"><span data-stu-id="13e33-148">status</span></span>|[<span data-ttu-id="13e33-149">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="13e33-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="13e33-150">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="13e33-150">The assessment process status.</span></span> <span data-ttu-id="13e33-151">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="13e33-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13e33-152">Связи</span><span class="sxs-lookup"><span data-stu-id="13e33-152">Relationships</span></span>

| <span data-ttu-id="13e33-153">Связь</span><span class="sxs-lookup"><span data-stu-id="13e33-153">Relationship</span></span> | <span data-ttu-id="13e33-154">Тип</span><span class="sxs-lookup"><span data-stu-id="13e33-154">Type</span></span>        | <span data-ttu-id="13e33-155">Описание</span><span class="sxs-lookup"><span data-stu-id="13e33-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="13e33-156">results</span><span class="sxs-lookup"><span data-stu-id="13e33-156">results</span></span>|<span data-ttu-id="13e33-157">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="13e33-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="13e33-158">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="13e33-158">A collection of threat assessment results.</span></span> <span data-ttu-id="13e33-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="13e33-159">Read-only.</span></span> <span data-ttu-id="13e33-160">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="13e33-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13e33-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13e33-161">JSON representation</span></span>

<span data-ttu-id="13e33-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13e33-162">The following is a JSON representation of the resource.</span></span>

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

