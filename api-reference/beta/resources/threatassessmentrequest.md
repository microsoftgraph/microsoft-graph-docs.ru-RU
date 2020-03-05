---
title: Тип ресурса Среатассессментрекуест
description: Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1a6a8f0f1448522d624b9c9e97bb2fab426b6988
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519780"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="52864-103">Тип ресурса Среатассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="52864-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="52864-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="52864-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52864-105">Абстрактный тип ресурсов, используемый для представления элемента запроса оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="52864-106">Запрос на оценку угроз может иметь один из следующих типов:</span><span class="sxs-lookup"><span data-stu-id="52864-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="52864-107">Почта (ресурс[маилассессментрекуест](mailAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="52864-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="52864-108">Файл электронной почты (ресурс[емаилфилеассессментрекуест](emailFileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="52864-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="52864-109">Файл (ресурс[филеассессментрекуест](fileAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="52864-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="52864-110">URL-адрес (ресурс[урлассессментрекуест](urlAssessmentRequest.md) )</span><span class="sxs-lookup"><span data-stu-id="52864-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="52864-111">Методы</span><span class="sxs-lookup"><span data-stu-id="52864-111">Methods</span></span>

| <span data-ttu-id="52864-112">Метод</span><span class="sxs-lookup"><span data-stu-id="52864-112">Method</span></span>       | <span data-ttu-id="52864-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52864-113">Return Type</span></span> | <span data-ttu-id="52864-114">Описание</span><span class="sxs-lookup"><span data-stu-id="52864-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="52864-115">Перечисление объектов threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="52864-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="52864-116">Коллекция [среатассессментрекуест](threatassessmentrequest.md)</span><span class="sxs-lookup"><span data-stu-id="52864-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="52864-117">Список всех запросов оценки угроз в клиенте.</span><span class="sxs-lookup"><span data-stu-id="52864-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="52864-118">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="52864-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="52864-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="52864-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="52864-120">Создание запроса на оценку угроз путем отправки производного типа ресурса: [маилассессментрекуест](../resources/mailAssessmentRequest.md), [емаилфилеассессментрекуест](../resources/emailFileAssessmentRequest.md), [филеассессментрекуест](../resources/fileAssessmentRequest.md), [урлассессментрекуест](../resources/urlAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="52864-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="52864-121">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="52864-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="52864-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="52864-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="52864-123">Получение свойств и связей указанного ресурса **среатассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="52864-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="52864-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="52864-124">Properties</span></span>

| <span data-ttu-id="52864-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="52864-125">Property</span></span>     | <span data-ttu-id="52864-126">Тип</span><span class="sxs-lookup"><span data-stu-id="52864-126">Type</span></span>        | <span data-ttu-id="52864-127">Описание</span><span class="sxs-lookup"><span data-stu-id="52864-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="52864-128">category</span><span class="sxs-lookup"><span data-stu-id="52864-128">category</span></span>|[<span data-ttu-id="52864-129">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="52864-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="52864-130">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-130">The threat category.</span></span> <span data-ttu-id="52864-131">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="52864-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="52864-132">contentType</span><span class="sxs-lookup"><span data-stu-id="52864-132">contentType</span></span>|[<span data-ttu-id="52864-133">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="52864-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="52864-134">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-134">The content type of threat assessment.</span></span> <span data-ttu-id="52864-135">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="52864-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="52864-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="52864-136">createdBy</span></span>|[<span data-ttu-id="52864-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="52864-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="52864-138">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="52864-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52864-139">createdDateTime</span></span>|<span data-ttu-id="52864-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52864-140">DateTimeOffset</span></span>|<span data-ttu-id="52864-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="52864-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="52864-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="52864-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="52864-143">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="52864-143">expectedAssessment</span></span>|[<span data-ttu-id="52864-144">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="52864-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="52864-145">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="52864-145">The expected assessment from submitter.</span></span> <span data-ttu-id="52864-146">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="52864-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="52864-147">id</span><span class="sxs-lookup"><span data-stu-id="52864-147">id</span></span>|<span data-ttu-id="52864-148">String</span><span class="sxs-lookup"><span data-stu-id="52864-148">String</span></span>|<span data-ttu-id="52864-149">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="52864-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="52864-150">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="52864-150">requestSource</span></span>|[<span data-ttu-id="52864-151">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="52864-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="52864-152">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-152">The source of the threat assessment request.</span></span> <span data-ttu-id="52864-153">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="52864-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="52864-154">status</span><span class="sxs-lookup"><span data-stu-id="52864-154">status</span></span>|[<span data-ttu-id="52864-155">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="52864-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="52864-156">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="52864-156">The assessment process status.</span></span> <span data-ttu-id="52864-157">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="52864-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52864-158">Связи</span><span class="sxs-lookup"><span data-stu-id="52864-158">Relationships</span></span>

| <span data-ttu-id="52864-159">Связь</span><span class="sxs-lookup"><span data-stu-id="52864-159">Relationship</span></span> | <span data-ttu-id="52864-160">Тип</span><span class="sxs-lookup"><span data-stu-id="52864-160">Type</span></span>        | <span data-ttu-id="52864-161">Описание</span><span class="sxs-lookup"><span data-stu-id="52864-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52864-162">results</span><span class="sxs-lookup"><span data-stu-id="52864-162">results</span></span>|<span data-ttu-id="52864-163">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="52864-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="52864-164">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="52864-164">A collection of threat assessment results.</span></span> <span data-ttu-id="52864-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="52864-165">Read-only.</span></span> <span data-ttu-id="52864-166">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="52864-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52864-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52864-167">JSON representation</span></span>

<span data-ttu-id="52864-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52864-168">The following is a JSON representation of the resource.</span></span>

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
