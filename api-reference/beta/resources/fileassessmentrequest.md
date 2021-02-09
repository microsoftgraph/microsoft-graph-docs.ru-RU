---
title: Тип ресурса fileAssessmentRequest
description: Используется для создания и извлечения оценки угрозы файла.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b61fadf340371b800e1dc093be012ba67f3eaf1b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154952"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="c0f1c-103">Тип ресурса fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="c0f1c-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="c0f1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f1c-105">Используется для создания и извлечения оценки угроз файлов, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="c0f1c-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="c0f1c-106">Это может быть текстовый файл, документ Word или двоичный файл, полученный во вложенном сообщении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="c0f1c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c0f1c-107">Methods</span></span>

| <span data-ttu-id="c0f1c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c0f1c-108">Method</span></span>       | <span data-ttu-id="c0f1c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c0f1c-109">Return Type</span></span> | <span data-ttu-id="c0f1c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f1c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c0f1c-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="c0f1c-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="c0f1c-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="c0f1c-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="c0f1c-113">Создайте запрос на оценку файла, опубликовав объект **fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="c0f1c-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="c0f1c-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="c0f1c-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="c0f1c-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="c0f1c-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="c0f1c-116">Чтение свойств и связей объекта **fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="c0f1c-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0f1c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0f1c-117">Properties</span></span>

| <span data-ttu-id="c0f1c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0f1c-118">Property</span></span>     | <span data-ttu-id="c0f1c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="c0f1c-119">Type</span></span>        | <span data-ttu-id="c0f1c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f1c-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0f1c-121">contentData</span><span class="sxs-lookup"><span data-stu-id="c0f1c-121">contentData</span></span>|<span data-ttu-id="c0f1c-122">String</span><span class="sxs-lookup"><span data-stu-id="c0f1c-122">String</span></span>|<span data-ttu-id="c0f1c-123">Содержимое файла в кодированном коде Base64.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-123">Base64 encoded file content.</span></span> <span data-ttu-id="c0f1c-124">Содержимое файла не может быть извлечено, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="c0f1c-125">fileName</span><span class="sxs-lookup"><span data-stu-id="c0f1c-125">fileName</span></span>|<span data-ttu-id="c0f1c-126">String</span><span class="sxs-lookup"><span data-stu-id="c0f1c-126">String</span></span>|<span data-ttu-id="c0f1c-127">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-127">The file name.</span></span>|
|<span data-ttu-id="c0f1c-128">category</span><span class="sxs-lookup"><span data-stu-id="c0f1c-128">category</span></span>|[<span data-ttu-id="c0f1c-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="c0f1c-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="c0f1c-130">Категория угрозы.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-130">The threat category.</span></span> <span data-ttu-id="c0f1c-131">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="c0f1c-132">contentType</span><span class="sxs-lookup"><span data-stu-id="c0f1c-132">contentType</span></span>|[<span data-ttu-id="c0f1c-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="c0f1c-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="c0f1c-134">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-134">The content type of threat assessment.</span></span> <span data-ttu-id="c0f1c-135">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="c0f1c-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="c0f1c-136">createdBy</span></span>|[<span data-ttu-id="c0f1c-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="c0f1c-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="c0f1c-138">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="c0f1c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c0f1c-139">createdDateTime</span></span>|<span data-ttu-id="c0f1c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0f1c-140">DateTimeOffset</span></span>|<span data-ttu-id="c0f1c-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="c0f1c-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c0f1c-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="c0f1c-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="c0f1c-143">expectedAssessment</span></span>|[<span data-ttu-id="c0f1c-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="c0f1c-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="c0f1c-145">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-145">The expected assessment from submitter.</span></span> <span data-ttu-id="c0f1c-146">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="c0f1c-147">id</span><span class="sxs-lookup"><span data-stu-id="c0f1c-147">id</span></span>|<span data-ttu-id="c0f1c-148">String</span><span class="sxs-lookup"><span data-stu-id="c0f1c-148">String</span></span>|<span data-ttu-id="c0f1c-149">Идентификатор запроса на оценку угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="c0f1c-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="c0f1c-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="c0f1c-150">requestSource</span></span>|[<span data-ttu-id="c0f1c-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="c0f1c-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="c0f1c-152">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-152">The source of threat assessment request.</span></span> <span data-ttu-id="c0f1c-153">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="c0f1c-154">status</span><span class="sxs-lookup"><span data-stu-id="c0f1c-154">status</span></span>|[<span data-ttu-id="c0f1c-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="c0f1c-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="c0f1c-156">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-156">The assessment process status.</span></span> <span data-ttu-id="c0f1c-157">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0f1c-158">Связи</span><span class="sxs-lookup"><span data-stu-id="c0f1c-158">Relationships</span></span>

| <span data-ttu-id="c0f1c-159">Связь</span><span class="sxs-lookup"><span data-stu-id="c0f1c-159">Relationship</span></span> | <span data-ttu-id="c0f1c-160">Тип</span><span class="sxs-lookup"><span data-stu-id="c0f1c-160">Type</span></span>        | <span data-ttu-id="c0f1c-161">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f1c-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0f1c-162">results</span><span class="sxs-lookup"><span data-stu-id="c0f1c-162">results</span></span>|<span data-ttu-id="c0f1c-163">[Коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="c0f1c-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="c0f1c-164">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-164">A collection of threat assessment results.</span></span> <span data-ttu-id="c0f1c-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-165">Read-only.</span></span> <span data-ttu-id="c0f1c-166">По умолчанию объект a не возвращает это свойство, если к этому `GET /threatAssessmentRequests/{id}` свойству не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0f1c-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0f1c-167">JSON representation</span></span>

<span data-ttu-id="c0f1c-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0f1c-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "fileName": "String",
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
  "description": "fileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


