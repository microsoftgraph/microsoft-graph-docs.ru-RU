---
title: Тип ресурса threatAssessmentRequest
description: Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1896123151680bfc6b69075d7f8888ccaa64b9ee
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155526"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="5b248-103">Тип ресурса threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="5b248-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b248-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b248-105">Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5b248-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="5b248-106">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="5b248-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="5b248-107">Mail ([ресурс mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5b248-108">Файл электронной почты[(ресурс emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5b248-109">File ([ресурс fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5b248-110">URL ([ресурс urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="5b248-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5b248-111">Methods</span></span>

| <span data-ttu-id="5b248-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5b248-112">Method</span></span>       | <span data-ttu-id="5b248-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5b248-113">Return Type</span></span> | <span data-ttu-id="5b248-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5b248-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5b248-115">Перечисление объектов threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="5b248-116">[Коллекция threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="5b248-117">Список всех запросов на оценку угроз в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5b248-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="5b248-118">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5b248-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="5b248-120">Создайте запрос на оценку угроз, опубликовав производный тип ресурса: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="5b248-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="5b248-121">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5b248-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5b248-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="5b248-123">Извлечение свойств и связей указанного **ресурса threatAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="5b248-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b248-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b248-124">Properties</span></span>

| <span data-ttu-id="5b248-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b248-125">Property</span></span>     | <span data-ttu-id="5b248-126">Тип</span><span class="sxs-lookup"><span data-stu-id="5b248-126">Type</span></span>        | <span data-ttu-id="5b248-127">Описание</span><span class="sxs-lookup"><span data-stu-id="5b248-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="5b248-128">category</span><span class="sxs-lookup"><span data-stu-id="5b248-128">category</span></span>|[<span data-ttu-id="5b248-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="5b248-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5b248-130">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="5b248-130">The threat category.</span></span> <span data-ttu-id="5b248-131">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5b248-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5b248-132">contentType</span><span class="sxs-lookup"><span data-stu-id="5b248-132">contentType</span></span>|[<span data-ttu-id="5b248-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="5b248-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5b248-134">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5b248-134">The content type of threat assessment.</span></span> <span data-ttu-id="5b248-135">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5b248-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5b248-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="5b248-136">createdBy</span></span>|[<span data-ttu-id="5b248-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="5b248-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="5b248-138">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5b248-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5b248-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b248-139">createdDateTime</span></span>|<span data-ttu-id="5b248-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b248-140">DateTimeOffset</span></span>|<span data-ttu-id="5b248-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5b248-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b248-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5b248-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5b248-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5b248-143">expectedAssessment</span></span>|[<span data-ttu-id="5b248-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="5b248-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5b248-145">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="5b248-145">The expected assessment from submitter.</span></span> <span data-ttu-id="5b248-146">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5b248-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5b248-147">id</span><span class="sxs-lookup"><span data-stu-id="5b248-147">id</span></span>|<span data-ttu-id="5b248-148">String</span><span class="sxs-lookup"><span data-stu-id="5b248-148">String</span></span>|<span data-ttu-id="5b248-149">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="5b248-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5b248-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="5b248-150">requestSource</span></span>|[<span data-ttu-id="5b248-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="5b248-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5b248-152">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5b248-152">The source of the threat assessment request.</span></span> <span data-ttu-id="5b248-153">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5b248-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5b248-154">status</span><span class="sxs-lookup"><span data-stu-id="5b248-154">status</span></span>|[<span data-ttu-id="5b248-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="5b248-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5b248-156">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5b248-156">The assessment process status.</span></span> <span data-ttu-id="5b248-157">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5b248-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b248-158">Связи</span><span class="sxs-lookup"><span data-stu-id="5b248-158">Relationships</span></span>

| <span data-ttu-id="5b248-159">Связь</span><span class="sxs-lookup"><span data-stu-id="5b248-159">Relationship</span></span> | <span data-ttu-id="5b248-160">Тип</span><span class="sxs-lookup"><span data-stu-id="5b248-160">Type</span></span>        | <span data-ttu-id="5b248-161">Описание</span><span class="sxs-lookup"><span data-stu-id="5b248-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5b248-162">results</span><span class="sxs-lookup"><span data-stu-id="5b248-162">results</span></span>|<span data-ttu-id="5b248-163">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5b248-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5b248-164">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5b248-164">A collection of threat assessment results.</span></span> <span data-ttu-id="5b248-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b248-165">Read-only.</span></span> <span data-ttu-id="5b248-166">По умолчанию объект a `GET /threatAssessmentRequests/{id}` не возвращает это свойство, если к этому свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="5b248-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b248-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b248-167">JSON representation</span></span>

<span data-ttu-id="5b248-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b248-168">The following is a JSON representation of the resource.</span></span>

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


