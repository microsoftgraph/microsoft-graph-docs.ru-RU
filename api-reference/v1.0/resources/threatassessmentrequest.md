---
title: Тип ресурса Среатассессментрекуест
description: Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df3f501ad281bcfced2e476b90e95b663fedef58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090895"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="5884d-103">Тип ресурса Среатассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="5884d-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="5884d-104">Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="5884d-105">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="5884d-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="5884d-106">Почта (ресурс[маилассессментрекуест](mailAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="5884d-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5884d-107">Файл электронной почты (ресурс[емаилфилеассессментрекуест](emailFileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="5884d-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5884d-108">Файл (ресурс[филеассессментрекуест](fileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="5884d-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="5884d-109">URL-адрес (ресурс[урлассессментрекуест](urlAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="5884d-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="5884d-110">Методы</span><span class="sxs-lookup"><span data-stu-id="5884d-110">Methods</span></span>

| <span data-ttu-id="5884d-111">Метод</span><span class="sxs-lookup"><span data-stu-id="5884d-111">Method</span></span>       | <span data-ttu-id="5884d-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5884d-112">Return Type</span></span> | <span data-ttu-id="5884d-113">Описание</span><span class="sxs-lookup"><span data-stu-id="5884d-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5884d-114">Перечисление объектов threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5884d-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="5884d-115">Коллекция [среатассессментрекуест](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="5884d-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="5884d-116">Список всех запросов оценки угроз в клиенте.</span><span class="sxs-lookup"><span data-stu-id="5884d-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="5884d-117">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5884d-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5884d-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5884d-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="5884d-119">Создание запроса на оценку угроз путем отправки производного типа ресурса: [маилассессментрекуест](../resources/mailAssessmentRequest.md), [емаилфилеассессментрекуест](../resources/emailFileAssessmentRequest.md), [филеассессментрекуест](../resources/fileAssessmentRequest.md), [урлассессментрекуест](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="5884d-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="5884d-120">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5884d-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5884d-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5884d-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="5884d-122">Получение свойств и связей указанного ресурса **среатассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="5884d-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="5884d-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="5884d-123">Properties</span></span>

| <span data-ttu-id="5884d-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="5884d-124">Property</span></span>     | <span data-ttu-id="5884d-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5884d-125">Type</span></span>        | <span data-ttu-id="5884d-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5884d-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="5884d-127">category</span><span class="sxs-lookup"><span data-stu-id="5884d-127">category</span></span>|[<span data-ttu-id="5884d-128">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="5884d-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5884d-129">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-129">The threat category.</span></span> <span data-ttu-id="5884d-130">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5884d-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5884d-131">contentType</span><span class="sxs-lookup"><span data-stu-id="5884d-131">contentType</span></span>|[<span data-ttu-id="5884d-132">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="5884d-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5884d-133">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-133">The content type of threat assessment.</span></span> <span data-ttu-id="5884d-134">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5884d-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5884d-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="5884d-135">createdBy</span></span>|[<span data-ttu-id="5884d-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="5884d-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="5884d-137">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5884d-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5884d-138">createdDateTime</span></span>|<span data-ttu-id="5884d-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5884d-139">DateTimeOffset</span></span>|<span data-ttu-id="5884d-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5884d-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5884d-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5884d-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5884d-142">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="5884d-142">expectedAssessment</span></span>|[<span data-ttu-id="5884d-143">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="5884d-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5884d-144">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="5884d-144">The expected assessment from submitter.</span></span> <span data-ttu-id="5884d-145">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5884d-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5884d-146">id</span><span class="sxs-lookup"><span data-stu-id="5884d-146">id</span></span>|<span data-ttu-id="5884d-147">Строка</span><span class="sxs-lookup"><span data-stu-id="5884d-147">String</span></span>|<span data-ttu-id="5884d-148">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="5884d-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5884d-149">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="5884d-149">requestSource</span></span>|[<span data-ttu-id="5884d-150">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="5884d-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5884d-151">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-151">The source of the threat assessment request.</span></span> <span data-ttu-id="5884d-152">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5884d-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5884d-153">status</span><span class="sxs-lookup"><span data-stu-id="5884d-153">status</span></span>|[<span data-ttu-id="5884d-154">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="5884d-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5884d-155">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5884d-155">The assessment process status.</span></span> <span data-ttu-id="5884d-156">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5884d-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5884d-157">Связи</span><span class="sxs-lookup"><span data-stu-id="5884d-157">Relationships</span></span>

| <span data-ttu-id="5884d-158">Связь</span><span class="sxs-lookup"><span data-stu-id="5884d-158">Relationship</span></span> | <span data-ttu-id="5884d-159">Тип</span><span class="sxs-lookup"><span data-stu-id="5884d-159">Type</span></span>        | <span data-ttu-id="5884d-160">Описание</span><span class="sxs-lookup"><span data-stu-id="5884d-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5884d-161">results</span><span class="sxs-lookup"><span data-stu-id="5884d-161">results</span></span>|<span data-ttu-id="5884d-162">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5884d-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5884d-163">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5884d-163">A collection of threat assessment results.</span></span> <span data-ttu-id="5884d-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5884d-164">Read-only.</span></span> <span data-ttu-id="5884d-165">По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.</span><span class="sxs-lookup"><span data-stu-id="5884d-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5884d-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5884d-166">JSON representation</span></span>

<span data-ttu-id="5884d-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5884d-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "",
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

