---
title: Тип ресурса threatAssessmentRequest
description: Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e316591f4f9db189b1b21dc2d9c3b8d83358c5da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158963"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="114ad-103">Тип ресурса threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="114ad-104">Абстрактный тип повторного использования, используемый для представления элемента запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="114ad-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="114ad-105">Запрос на оценку угроз может быть одним из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="114ad-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="114ad-106">Mail ([ресурс mailAssessmentRequest)](mailAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="114ad-107">Файл электронной почты[(ресурс emailFileAssessmentRequest)](emailFileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="114ad-108">File ([ресурс fileAssessmentRequest)](fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="114ad-109">URL ([ресурс urlAssessmentRequest)](urlAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="114ad-110">Методы</span><span class="sxs-lookup"><span data-stu-id="114ad-110">Methods</span></span>

| <span data-ttu-id="114ad-111">Метод</span><span class="sxs-lookup"><span data-stu-id="114ad-111">Method</span></span>       | <span data-ttu-id="114ad-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="114ad-112">Return Type</span></span> | <span data-ttu-id="114ad-113">Описание</span><span class="sxs-lookup"><span data-stu-id="114ad-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="114ad-114">Перечисление объектов threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="114ad-115">[Коллекция threatAssessmentRequest](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="114ad-116">Список всех запросов на оценку угроз в клиенте.</span><span class="sxs-lookup"><span data-stu-id="114ad-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="114ad-117">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="114ad-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="114ad-119">Создайте запрос на оценку угроз, опубликовав производный тип ресурса: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="114ad-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="114ad-120">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="114ad-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="114ad-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="114ad-122">Извлечение свойств и связей указанного **ресурса threatAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="114ad-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="114ad-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="114ad-123">Properties</span></span>

| <span data-ttu-id="114ad-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="114ad-124">Property</span></span>     | <span data-ttu-id="114ad-125">Тип</span><span class="sxs-lookup"><span data-stu-id="114ad-125">Type</span></span>        | <span data-ttu-id="114ad-126">Описание</span><span class="sxs-lookup"><span data-stu-id="114ad-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="114ad-127">category</span><span class="sxs-lookup"><span data-stu-id="114ad-127">category</span></span>|[<span data-ttu-id="114ad-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="114ad-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="114ad-129">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="114ad-129">The threat category.</span></span> <span data-ttu-id="114ad-130">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="114ad-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="114ad-131">contentType</span><span class="sxs-lookup"><span data-stu-id="114ad-131">contentType</span></span>|[<span data-ttu-id="114ad-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="114ad-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="114ad-133">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="114ad-133">The content type of threat assessment.</span></span> <span data-ttu-id="114ad-134">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="114ad-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="114ad-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="114ad-135">createdBy</span></span>|[<span data-ttu-id="114ad-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="114ad-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="114ad-137">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="114ad-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="114ad-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="114ad-138">createdDateTime</span></span>|<span data-ttu-id="114ad-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="114ad-139">DateTimeOffset</span></span>|<span data-ttu-id="114ad-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="114ad-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="114ad-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="114ad-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="114ad-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="114ad-142">expectedAssessment</span></span>|[<span data-ttu-id="114ad-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="114ad-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="114ad-144">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="114ad-144">The expected assessment from submitter.</span></span> <span data-ttu-id="114ad-145">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="114ad-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="114ad-146">id</span><span class="sxs-lookup"><span data-stu-id="114ad-146">id</span></span>|<span data-ttu-id="114ad-147">String</span><span class="sxs-lookup"><span data-stu-id="114ad-147">String</span></span>|<span data-ttu-id="114ad-148">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="114ad-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="114ad-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="114ad-149">requestSource</span></span>|[<span data-ttu-id="114ad-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="114ad-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="114ad-151">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="114ad-151">The source of the threat assessment request.</span></span> <span data-ttu-id="114ad-152">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="114ad-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="114ad-153">status</span><span class="sxs-lookup"><span data-stu-id="114ad-153">status</span></span>|[<span data-ttu-id="114ad-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="114ad-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="114ad-155">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="114ad-155">The assessment process status.</span></span> <span data-ttu-id="114ad-156">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="114ad-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="114ad-157">Связи</span><span class="sxs-lookup"><span data-stu-id="114ad-157">Relationships</span></span>

| <span data-ttu-id="114ad-158">Связь</span><span class="sxs-lookup"><span data-stu-id="114ad-158">Relationship</span></span> | <span data-ttu-id="114ad-159">Тип</span><span class="sxs-lookup"><span data-stu-id="114ad-159">Type</span></span>        | <span data-ttu-id="114ad-160">Описание</span><span class="sxs-lookup"><span data-stu-id="114ad-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="114ad-161">results</span><span class="sxs-lookup"><span data-stu-id="114ad-161">results</span></span>|<span data-ttu-id="114ad-162">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="114ad-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="114ad-163">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="114ad-163">A collection of threat assessment results.</span></span> <span data-ttu-id="114ad-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="114ad-164">Read-only.</span></span> <span data-ttu-id="114ad-165">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="114ad-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="114ad-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="114ad-166">JSON representation</span></span>

<span data-ttu-id="114ad-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="114ad-167">The following is a JSON representation of the resource.</span></span>

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

