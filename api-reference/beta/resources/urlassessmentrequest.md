---
title: Тип ресурса urlAssessmentRequest
description: Используется для создания и извлечения оценки угрозы URL-адреса.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 68df999766bd7fd1b548e0db7e96a8819c04c75a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156674"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="aaa63-103">Тип ресурса urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="aaa63-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="aaa63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaa63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaa63-105">Используется для создания и извлечения оценки угрозы URL-адреса, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="aaa63-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="aaa63-106">Методы</span><span class="sxs-lookup"><span data-stu-id="aaa63-106">Methods</span></span>

| <span data-ttu-id="aaa63-107">Метод</span><span class="sxs-lookup"><span data-stu-id="aaa63-107">Method</span></span>       | <span data-ttu-id="aaa63-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aaa63-108">Return Type</span></span> | <span data-ttu-id="aaa63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa63-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="aaa63-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="aaa63-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="aaa63-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="aaa63-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="aaa63-112">Создайте новый запрос на оценку URL-адреса, опубликовав объект **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="aaa63-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="aaa63-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="aaa63-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="aaa63-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="aaa63-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="aaa63-115">Чтение свойств и связей объекта **urlAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="aaa63-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aaa63-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="aaa63-116">Properties</span></span>

| <span data-ttu-id="aaa63-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="aaa63-117">Property</span></span>     | <span data-ttu-id="aaa63-118">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa63-118">Type</span></span>        | <span data-ttu-id="aaa63-119">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa63-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aaa63-120">url</span><span class="sxs-lookup"><span data-stu-id="aaa63-120">url</span></span>|<span data-ttu-id="aaa63-121">String</span><span class="sxs-lookup"><span data-stu-id="aaa63-121">String</span></span>|<span data-ttu-id="aaa63-122">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="aaa63-122">The URL string.</span></span>|
|<span data-ttu-id="aaa63-123">category</span><span class="sxs-lookup"><span data-stu-id="aaa63-123">category</span></span>|[<span data-ttu-id="aaa63-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="aaa63-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="aaa63-125">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="aaa63-125">The threat category.</span></span> <span data-ttu-id="aaa63-126">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="aaa63-127">contentType</span><span class="sxs-lookup"><span data-stu-id="aaa63-127">contentType</span></span>|[<span data-ttu-id="aaa63-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="aaa63-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="aaa63-129">Тип контента оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="aaa63-129">The content type of the threat assessment.</span></span> <span data-ttu-id="aaa63-130">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="aaa63-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="aaa63-131">createdBy</span></span>|[<span data-ttu-id="aaa63-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="aaa63-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="aaa63-133">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="aaa63-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="aaa63-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa63-134">createdDateTime</span></span>|<span data-ttu-id="aaa63-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa63-135">DateTimeOffset</span></span>|<span data-ttu-id="aaa63-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="aaa63-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aaa63-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aaa63-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="aaa63-138">expectedAssessment</span></span>|[<span data-ttu-id="aaa63-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="aaa63-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="aaa63-140">Ожидаемая оценка от ubmitter.</span><span class="sxs-lookup"><span data-stu-id="aaa63-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="aaa63-141">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="aaa63-142">id</span><span class="sxs-lookup"><span data-stu-id="aaa63-142">id</span></span>|<span data-ttu-id="aaa63-143">String</span><span class="sxs-lookup"><span data-stu-id="aaa63-143">String</span></span>|<span data-ttu-id="aaa63-144">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="aaa63-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="aaa63-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="aaa63-145">requestSource</span></span>|[<span data-ttu-id="aaa63-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="aaa63-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="aaa63-147">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="aaa63-147">The source of the threat assessment request.</span></span> <span data-ttu-id="aaa63-148">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="aaa63-149">status</span><span class="sxs-lookup"><span data-stu-id="aaa63-149">status</span></span>|[<span data-ttu-id="aaa63-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="aaa63-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="aaa63-151">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="aaa63-151">The assessment process status.</span></span> <span data-ttu-id="aaa63-152">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="aaa63-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aaa63-153">Связи</span><span class="sxs-lookup"><span data-stu-id="aaa63-153">Relationships</span></span>

| <span data-ttu-id="aaa63-154">Связь</span><span class="sxs-lookup"><span data-stu-id="aaa63-154">Relationship</span></span> | <span data-ttu-id="aaa63-155">Тип</span><span class="sxs-lookup"><span data-stu-id="aaa63-155">Type</span></span>        | <span data-ttu-id="aaa63-156">Описание</span><span class="sxs-lookup"><span data-stu-id="aaa63-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="aaa63-157">results</span><span class="sxs-lookup"><span data-stu-id="aaa63-157">results</span></span>|<span data-ttu-id="aaa63-158">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="aaa63-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="aaa63-159">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="aaa63-159">A collection of threat assessment results.</span></span> <span data-ttu-id="aaa63-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="aaa63-160">Read-only.</span></span> <span data-ttu-id="aaa63-161">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="aaa63-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaa63-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aaa63-162">JSON representation</span></span>

<span data-ttu-id="aaa63-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aaa63-163">The following is a JSON representation of the resource.</span></span>

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


