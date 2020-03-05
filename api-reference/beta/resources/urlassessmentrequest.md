---
title: Тип ресурса Урлассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для URL-адресов.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2eb3372b92a3665129bb0b4eb4d0f27bc77884f3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519570"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="e588f-103">Тип ресурса Урлассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="e588f-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="e588f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e588f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e588f-105">Используется для создания и извлечения средства оценки угроз URL-адресов, производного от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="e588f-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e588f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="e588f-106">Methods</span></span>

| <span data-ttu-id="e588f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="e588f-107">Method</span></span>       | <span data-ttu-id="e588f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e588f-108">Return Type</span></span> | <span data-ttu-id="e588f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e588f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e588f-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e588f-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="e588f-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e588f-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="e588f-112">Создание нового запроса на оценку URL-адреса путем отправки объекта **урлассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="e588f-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="e588f-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e588f-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="e588f-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e588f-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="e588f-115">Чтение свойств и связей объекта **урлассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="e588f-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e588f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="e588f-116">Properties</span></span>

| <span data-ttu-id="e588f-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="e588f-117">Property</span></span>     | <span data-ttu-id="e588f-118">Тип</span><span class="sxs-lookup"><span data-stu-id="e588f-118">Type</span></span>        | <span data-ttu-id="e588f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="e588f-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e588f-120">url</span><span class="sxs-lookup"><span data-stu-id="e588f-120">url</span></span>|<span data-ttu-id="e588f-121">String</span><span class="sxs-lookup"><span data-stu-id="e588f-121">String</span></span>|<span data-ttu-id="e588f-122">Строка URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="e588f-122">The URL string.</span></span>|
|<span data-ttu-id="e588f-123">category</span><span class="sxs-lookup"><span data-stu-id="e588f-123">category</span></span>|[<span data-ttu-id="e588f-124">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="e588f-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="e588f-125">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="e588f-125">The threat category.</span></span> <span data-ttu-id="e588f-126">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="e588f-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="e588f-127">contentType</span><span class="sxs-lookup"><span data-stu-id="e588f-127">contentType</span></span>|[<span data-ttu-id="e588f-128">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="e588f-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="e588f-129">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="e588f-129">The content type of the threat assessment.</span></span> <span data-ttu-id="e588f-130">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="e588f-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="e588f-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="e588f-131">createdBy</span></span>|[<span data-ttu-id="e588f-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="e588f-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="e588f-133">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e588f-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="e588f-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e588f-134">createdDateTime</span></span>|<span data-ttu-id="e588f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e588f-135">DateTimeOffset</span></span>|<span data-ttu-id="e588f-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="e588f-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e588f-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e588f-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e588f-138">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="e588f-138">expectedAssessment</span></span>|[<span data-ttu-id="e588f-139">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="e588f-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="e588f-140">Ожидаемая Оценка из убмиттер.</span><span class="sxs-lookup"><span data-stu-id="e588f-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="e588f-141">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="e588f-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="e588f-142">id</span><span class="sxs-lookup"><span data-stu-id="e588f-142">id</span></span>|<span data-ttu-id="e588f-143">String</span><span class="sxs-lookup"><span data-stu-id="e588f-143">String</span></span>|<span data-ttu-id="e588f-144">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="e588f-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e588f-145">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="e588f-145">requestSource</span></span>|[<span data-ttu-id="e588f-146">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="e588f-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="e588f-147">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="e588f-147">The source of the threat assessment request.</span></span> <span data-ttu-id="e588f-148">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="e588f-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="e588f-149">status</span><span class="sxs-lookup"><span data-stu-id="e588f-149">status</span></span>|[<span data-ttu-id="e588f-150">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="e588f-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="e588f-151">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="e588f-151">The assessment process status.</span></span> <span data-ttu-id="e588f-152">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="e588f-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e588f-153">Связи</span><span class="sxs-lookup"><span data-stu-id="e588f-153">Relationships</span></span>

| <span data-ttu-id="e588f-154">Связь</span><span class="sxs-lookup"><span data-stu-id="e588f-154">Relationship</span></span> | <span data-ttu-id="e588f-155">Тип</span><span class="sxs-lookup"><span data-stu-id="e588f-155">Type</span></span>        | <span data-ttu-id="e588f-156">Описание</span><span class="sxs-lookup"><span data-stu-id="e588f-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e588f-157">results</span><span class="sxs-lookup"><span data-stu-id="e588f-157">results</span></span>|<span data-ttu-id="e588f-158">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="e588f-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="e588f-159">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="e588f-159">A collection of threat assessment results.</span></span> <span data-ttu-id="e588f-160">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e588f-160">Read-only.</span></span> <span data-ttu-id="e588f-161">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="e588f-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e588f-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e588f-162">JSON representation</span></span>

<span data-ttu-id="e588f-163">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e588f-163">The following is a JSON representation of the resource.</span></span>

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
