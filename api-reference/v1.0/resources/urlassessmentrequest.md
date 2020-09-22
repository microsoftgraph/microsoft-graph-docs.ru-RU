---
title: Тип ресурса Урлассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для URL-адресов.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6723e2c4ce080555bf9932bb5c75012110d7b754
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090608"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="ca883-103">Тип ресурса Урлассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="ca883-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="ca883-104">Используется для создания и извлечения средства оценки угроз URL-адресов, производного от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="ca883-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ca883-105">Методы</span><span class="sxs-lookup"><span data-stu-id="ca883-105">Methods</span></span>

| <span data-ttu-id="ca883-106">Метод</span><span class="sxs-lookup"><span data-stu-id="ca883-106">Method</span></span>       | <span data-ttu-id="ca883-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ca883-107">Return Type</span></span> | <span data-ttu-id="ca883-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ca883-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ca883-109">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ca883-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="ca883-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ca883-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="ca883-111">Создание нового запроса на оценку URL-адреса путем отправки объекта **урлассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="ca883-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="ca883-112">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ca883-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="ca883-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="ca883-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="ca883-114">Чтение свойств и связей объекта **урлассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="ca883-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ca883-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca883-115">Properties</span></span>

| <span data-ttu-id="ca883-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca883-116">Property</span></span>     | <span data-ttu-id="ca883-117">Тип</span><span class="sxs-lookup"><span data-stu-id="ca883-117">Type</span></span>        | <span data-ttu-id="ca883-118">Описание</span><span class="sxs-lookup"><span data-stu-id="ca883-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca883-119">url</span><span class="sxs-lookup"><span data-stu-id="ca883-119">url</span></span>|<span data-ttu-id="ca883-120">String</span><span class="sxs-lookup"><span data-stu-id="ca883-120">String</span></span>|<span data-ttu-id="ca883-121">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="ca883-121">The URL string.</span></span>|
|<span data-ttu-id="ca883-122">category</span><span class="sxs-lookup"><span data-stu-id="ca883-122">category</span></span>|[<span data-ttu-id="ca883-123">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="ca883-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="ca883-124">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="ca883-124">The threat category.</span></span> <span data-ttu-id="ca883-125">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="ca883-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="ca883-126">contentType</span><span class="sxs-lookup"><span data-stu-id="ca883-126">contentType</span></span>|[<span data-ttu-id="ca883-127">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="ca883-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="ca883-128">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="ca883-128">The content type of the threat assessment.</span></span> <span data-ttu-id="ca883-129">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="ca883-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="ca883-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="ca883-130">createdBy</span></span>|[<span data-ttu-id="ca883-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="ca883-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="ca883-132">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="ca883-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="ca883-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ca883-133">createdDateTime</span></span>|<span data-ttu-id="ca883-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca883-134">DateTimeOffset</span></span>|<span data-ttu-id="ca883-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ca883-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca883-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ca883-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="ca883-137">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="ca883-137">expectedAssessment</span></span>|[<span data-ttu-id="ca883-138">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="ca883-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="ca883-139">Ожидаемая Оценка из убмиттер.</span><span class="sxs-lookup"><span data-stu-id="ca883-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="ca883-140">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="ca883-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="ca883-141">id</span><span class="sxs-lookup"><span data-stu-id="ca883-141">id</span></span>|<span data-ttu-id="ca883-142">Строка</span><span class="sxs-lookup"><span data-stu-id="ca883-142">String</span></span>|<span data-ttu-id="ca883-143">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="ca883-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="ca883-144">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="ca883-144">requestSource</span></span>|[<span data-ttu-id="ca883-145">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="ca883-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="ca883-146">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="ca883-146">The source of the threat assessment request.</span></span> <span data-ttu-id="ca883-147">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="ca883-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="ca883-148">status</span><span class="sxs-lookup"><span data-stu-id="ca883-148">status</span></span>|[<span data-ttu-id="ca883-149">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="ca883-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="ca883-150">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="ca883-150">The assessment process status.</span></span> <span data-ttu-id="ca883-151">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="ca883-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca883-152">Связи</span><span class="sxs-lookup"><span data-stu-id="ca883-152">Relationships</span></span>

| <span data-ttu-id="ca883-153">Связь</span><span class="sxs-lookup"><span data-stu-id="ca883-153">Relationship</span></span> | <span data-ttu-id="ca883-154">Тип</span><span class="sxs-lookup"><span data-stu-id="ca883-154">Type</span></span>        | <span data-ttu-id="ca883-155">Описание</span><span class="sxs-lookup"><span data-stu-id="ca883-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ca883-156">results</span><span class="sxs-lookup"><span data-stu-id="ca883-156">results</span></span>|<span data-ttu-id="ca883-157">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="ca883-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="ca883-158">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="ca883-158">A collection of threat assessment results.</span></span> <span data-ttu-id="ca883-159">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ca883-159">Read-only.</span></span> <span data-ttu-id="ca883-160">По умолчанию объект a не `GET /threatAssessmentRequests/{id}` возвращает это свойство, пока не применено `$expand` к нему.</span><span class="sxs-lookup"><span data-stu-id="ca883-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca883-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca883-161">JSON representation</span></span>

<span data-ttu-id="ca883-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca883-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "baseType": "",
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

