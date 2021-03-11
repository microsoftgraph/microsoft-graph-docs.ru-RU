---
title: тип ресурса urlAssessmentRequest
description: Используется для создания и получения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 226e4fff9114fbf13bc0e8bcdc9290180cc487f4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720961"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="20dd7-103">тип ресурса urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="20dd7-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="20dd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20dd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20dd7-105">Используется для создания и получения оценки угроз URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="20dd7-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="20dd7-106">Методы</span><span class="sxs-lookup"><span data-stu-id="20dd7-106">Methods</span></span>

| <span data-ttu-id="20dd7-107">Метод</span><span class="sxs-lookup"><span data-stu-id="20dd7-107">Method</span></span>       | <span data-ttu-id="20dd7-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="20dd7-108">Return Type</span></span> | <span data-ttu-id="20dd7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="20dd7-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="20dd7-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="20dd7-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="20dd7-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="20dd7-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="20dd7-112">Создайте новый запрос на оценку URL-адресов, разместив **объект urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="20dd7-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="20dd7-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="20dd7-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="20dd7-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="20dd7-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="20dd7-115">Ознакомьтесь с свойствами и отношениями объекта **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="20dd7-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="20dd7-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="20dd7-116">Properties</span></span>

| <span data-ttu-id="20dd7-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="20dd7-117">Property</span></span>     | <span data-ttu-id="20dd7-118">Тип</span><span class="sxs-lookup"><span data-stu-id="20dd7-118">Type</span></span>        | <span data-ttu-id="20dd7-119">Описание</span><span class="sxs-lookup"><span data-stu-id="20dd7-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20dd7-120">url</span><span class="sxs-lookup"><span data-stu-id="20dd7-120">url</span></span>|<span data-ttu-id="20dd7-121">String</span><span class="sxs-lookup"><span data-stu-id="20dd7-121">String</span></span>|<span data-ttu-id="20dd7-122">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="20dd7-122">The URL string.</span></span>|
|<span data-ttu-id="20dd7-123">category</span><span class="sxs-lookup"><span data-stu-id="20dd7-123">category</span></span>|[<span data-ttu-id="20dd7-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="20dd7-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="20dd7-125">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="20dd7-125">The threat category.</span></span> <span data-ttu-id="20dd7-126">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="20dd7-127">contentType</span><span class="sxs-lookup"><span data-stu-id="20dd7-127">contentType</span></span>|[<span data-ttu-id="20dd7-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="20dd7-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="20dd7-129">Тип контента оценки угрозы.</span><span class="sxs-lookup"><span data-stu-id="20dd7-129">The content type of the threat assessment.</span></span> <span data-ttu-id="20dd7-130">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="20dd7-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="20dd7-131">createdBy</span></span>|[<span data-ttu-id="20dd7-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="20dd7-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="20dd7-133">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="20dd7-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="20dd7-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20dd7-134">createdDateTime</span></span>|<span data-ttu-id="20dd7-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20dd7-135">DateTimeOffset</span></span>|<span data-ttu-id="20dd7-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="20dd7-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="20dd7-137">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="20dd7-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="20dd7-138">expectedAssessment</span></span>|[<span data-ttu-id="20dd7-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="20dd7-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="20dd7-140">Ожидаемая оценка от ubmitter.</span><span class="sxs-lookup"><span data-stu-id="20dd7-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="20dd7-141">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="20dd7-142">id</span><span class="sxs-lookup"><span data-stu-id="20dd7-142">id</span></span>|<span data-ttu-id="20dd7-143">String</span><span class="sxs-lookup"><span data-stu-id="20dd7-143">String</span></span>|<span data-ttu-id="20dd7-144">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="20dd7-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="20dd7-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="20dd7-145">requestSource</span></span>|[<span data-ttu-id="20dd7-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="20dd7-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="20dd7-147">Источник запроса на оценку угрозы.</span><span class="sxs-lookup"><span data-stu-id="20dd7-147">The source of the threat assessment request.</span></span> <span data-ttu-id="20dd7-148">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="20dd7-149">status</span><span class="sxs-lookup"><span data-stu-id="20dd7-149">status</span></span>|[<span data-ttu-id="20dd7-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="20dd7-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="20dd7-151">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="20dd7-151">The assessment process status.</span></span> <span data-ttu-id="20dd7-152">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="20dd7-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20dd7-153">Связи</span><span class="sxs-lookup"><span data-stu-id="20dd7-153">Relationships</span></span>

| <span data-ttu-id="20dd7-154">Связь</span><span class="sxs-lookup"><span data-stu-id="20dd7-154">Relationship</span></span> | <span data-ttu-id="20dd7-155">Тип</span><span class="sxs-lookup"><span data-stu-id="20dd7-155">Type</span></span>        | <span data-ttu-id="20dd7-156">Описание</span><span class="sxs-lookup"><span data-stu-id="20dd7-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="20dd7-157">results</span><span class="sxs-lookup"><span data-stu-id="20dd7-157">results</span></span>|<span data-ttu-id="20dd7-158">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="20dd7-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="20dd7-159">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="20dd7-159">A collection of threat assessment results.</span></span> <span data-ttu-id="20dd7-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="20dd7-160">Read-only.</span></span> <span data-ttu-id="20dd7-161">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="20dd7-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="20dd7-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="20dd7-162">JSON representation</span></span>

<span data-ttu-id="20dd7-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20dd7-163">The following is a JSON representation of the resource.</span></span>

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


