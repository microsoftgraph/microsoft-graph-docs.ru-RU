---
title: тип ресурса urlAssessmentRequest
description: Используется для создания и получения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3d206e14f61bf273f8764a34e3d5ef6cbd154190
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950256"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="a9c92-103">тип ресурса urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9c92-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="a9c92-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9c92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9c92-105">Используется для создания и получения оценки угроз URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="a9c92-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a9c92-106">Методы</span><span class="sxs-lookup"><span data-stu-id="a9c92-106">Methods</span></span>

| <span data-ttu-id="a9c92-107">Метод</span><span class="sxs-lookup"><span data-stu-id="a9c92-107">Method</span></span>       | <span data-ttu-id="a9c92-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a9c92-108">Return Type</span></span> | <span data-ttu-id="a9c92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a9c92-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a9c92-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9c92-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="a9c92-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9c92-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="a9c92-112">Создайте новый запрос на оценку URL-адресов, разместив **объект urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="a9c92-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="a9c92-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9c92-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="a9c92-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a9c92-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="a9c92-115">Ознакомьтесь с свойствами и отношениями объекта **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="a9c92-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a9c92-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9c92-116">Properties</span></span>

| <span data-ttu-id="a9c92-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9c92-117">Property</span></span>     | <span data-ttu-id="a9c92-118">Тип</span><span class="sxs-lookup"><span data-stu-id="a9c92-118">Type</span></span>        | <span data-ttu-id="a9c92-119">Описание</span><span class="sxs-lookup"><span data-stu-id="a9c92-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9c92-120">url</span><span class="sxs-lookup"><span data-stu-id="a9c92-120">url</span></span>|<span data-ttu-id="a9c92-121">String</span><span class="sxs-lookup"><span data-stu-id="a9c92-121">String</span></span>|<span data-ttu-id="a9c92-122">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="a9c92-122">The URL string.</span></span>|
|<span data-ttu-id="a9c92-123">category</span><span class="sxs-lookup"><span data-stu-id="a9c92-123">category</span></span>|[<span data-ttu-id="a9c92-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="a9c92-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="a9c92-125">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="a9c92-125">The threat category.</span></span> <span data-ttu-id="a9c92-126">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="a9c92-127">contentType</span><span class="sxs-lookup"><span data-stu-id="a9c92-127">contentType</span></span>|[<span data-ttu-id="a9c92-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="a9c92-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="a9c92-129">Тип контента оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="a9c92-129">The content type of the threat assessment.</span></span> <span data-ttu-id="a9c92-130">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="a9c92-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="a9c92-131">createdBy</span></span>|[<span data-ttu-id="a9c92-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9c92-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="a9c92-133">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="a9c92-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="a9c92-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9c92-134">createdDateTime</span></span>|<span data-ttu-id="a9c92-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9c92-135">DateTimeOffset</span></span>|<span data-ttu-id="a9c92-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a9c92-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a9c92-137">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="a9c92-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="a9c92-138">expectedAssessment</span></span>|[<span data-ttu-id="a9c92-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="a9c92-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="a9c92-140">Ожидаемая оценка от ubmitter.</span><span class="sxs-lookup"><span data-stu-id="a9c92-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="a9c92-141">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="a9c92-142">id</span><span class="sxs-lookup"><span data-stu-id="a9c92-142">id</span></span>|<span data-ttu-id="a9c92-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a9c92-143">String</span></span>|<span data-ttu-id="a9c92-144">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="a9c92-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="a9c92-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="a9c92-145">requestSource</span></span>|[<span data-ttu-id="a9c92-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="a9c92-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="a9c92-147">Источник запроса на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="a9c92-147">The source of the threat assessment request.</span></span> <span data-ttu-id="a9c92-148">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="a9c92-149">status</span><span class="sxs-lookup"><span data-stu-id="a9c92-149">status</span></span>|[<span data-ttu-id="a9c92-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="a9c92-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="a9c92-151">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="a9c92-151">The assessment process status.</span></span> <span data-ttu-id="a9c92-152">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="a9c92-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9c92-153">Связи</span><span class="sxs-lookup"><span data-stu-id="a9c92-153">Relationships</span></span>

| <span data-ttu-id="a9c92-154">Связь</span><span class="sxs-lookup"><span data-stu-id="a9c92-154">Relationship</span></span> | <span data-ttu-id="a9c92-155">Тип</span><span class="sxs-lookup"><span data-stu-id="a9c92-155">Type</span></span>        | <span data-ttu-id="a9c92-156">Описание</span><span class="sxs-lookup"><span data-stu-id="a9c92-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a9c92-157">results</span><span class="sxs-lookup"><span data-stu-id="a9c92-157">results</span></span>|<span data-ttu-id="a9c92-158">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="a9c92-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="a9c92-159">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="a9c92-159">A collection of threat assessment results.</span></span> <span data-ttu-id="a9c92-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a9c92-160">Read-only.</span></span> <span data-ttu-id="a9c92-161">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="a9c92-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9c92-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9c92-162">JSON representation</span></span>

<span data-ttu-id="a9c92-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9c92-163">The following is a JSON representation of the resource.</span></span>

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


