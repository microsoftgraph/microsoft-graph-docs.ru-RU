---
title: тип ресурса fileAssessmentRequest
description: Используется для создания и получения оценки угрозы файла.
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 36ace43254e440b4777609ff31378621cffa25fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952524"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="8e664-103">тип ресурса fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e664-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="8e664-104">Используется для создания и получения оценки угрозы файлов, полученной из [threatAssessmentRequest.](threatAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="8e664-104">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="8e664-105">Файл может быть текстовым файлом или документом Word или двоичным файлом, полученным в вложении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8e664-105">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="8e664-106">Методы</span><span class="sxs-lookup"><span data-stu-id="8e664-106">Methods</span></span>

| <span data-ttu-id="8e664-107">Метод</span><span class="sxs-lookup"><span data-stu-id="8e664-107">Method</span></span>       | <span data-ttu-id="8e664-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8e664-108">Return Type</span></span> | <span data-ttu-id="8e664-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8e664-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8e664-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e664-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="8e664-111">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e664-111">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="8e664-112">Создайте новый запрос на оценку файлов, разместив объект **fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="8e664-112">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="8e664-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e664-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="8e664-114">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="8e664-114">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="8e664-115">Ознакомьтесь с свойствами и отношениями объекта **fileAssessmentRequest.**</span><span class="sxs-lookup"><span data-stu-id="8e664-115">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8e664-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e664-116">Properties</span></span>

| <span data-ttu-id="8e664-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e664-117">Property</span></span>     | <span data-ttu-id="8e664-118">Тип</span><span class="sxs-lookup"><span data-stu-id="8e664-118">Type</span></span>        | <span data-ttu-id="8e664-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8e664-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e664-120">contentData</span><span class="sxs-lookup"><span data-stu-id="8e664-120">contentData</span></span>|<span data-ttu-id="8e664-121">String</span><span class="sxs-lookup"><span data-stu-id="8e664-121">String</span></span>|<span data-ttu-id="8e664-122">Кодированное содержимое файла Base64.</span><span class="sxs-lookup"><span data-stu-id="8e664-122">Base64 encoded file content.</span></span> <span data-ttu-id="8e664-123">Содержимое файла не может получить обратно, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="8e664-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="8e664-124">fileName</span><span class="sxs-lookup"><span data-stu-id="8e664-124">fileName</span></span>|<span data-ttu-id="8e664-125">String</span><span class="sxs-lookup"><span data-stu-id="8e664-125">String</span></span>|<span data-ttu-id="8e664-126">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="8e664-126">The file name.</span></span>|
|<span data-ttu-id="8e664-127">category</span><span class="sxs-lookup"><span data-stu-id="8e664-127">category</span></span>|[<span data-ttu-id="8e664-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="8e664-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="8e664-129">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="8e664-129">The threat category.</span></span> <span data-ttu-id="8e664-130">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="8e664-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="8e664-131">contentType</span><span class="sxs-lookup"><span data-stu-id="8e664-131">contentType</span></span>|[<span data-ttu-id="8e664-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="8e664-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="8e664-133">Тип оценки угрозы контента.</span><span class="sxs-lookup"><span data-stu-id="8e664-133">The content type of threat assessment.</span></span> <span data-ttu-id="8e664-134">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="8e664-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="8e664-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="8e664-135">createdBy</span></span>|[<span data-ttu-id="8e664-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="8e664-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="8e664-137">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="8e664-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="8e664-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e664-138">createdDateTime</span></span>|<span data-ttu-id="8e664-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e664-139">DateTimeOffset</span></span>|<span data-ttu-id="8e664-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="8e664-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8e664-141">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="8e664-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="8e664-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="8e664-142">expectedAssessment</span></span>|[<span data-ttu-id="8e664-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="8e664-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="8e664-144">Ожидаемая оценка от подавщика.</span><span class="sxs-lookup"><span data-stu-id="8e664-144">The expected assessment from submitter.</span></span> <span data-ttu-id="8e664-145">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="8e664-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="8e664-146">id</span><span class="sxs-lookup"><span data-stu-id="8e664-146">id</span></span>|<span data-ttu-id="8e664-147">String</span><span class="sxs-lookup"><span data-stu-id="8e664-147">String</span></span>|<span data-ttu-id="8e664-148">Идентификатор запроса на оценку угрозы — это уникальный идентификатор глобального идентификатора (GUID).</span><span class="sxs-lookup"><span data-stu-id="8e664-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="8e664-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="8e664-149">requestSource</span></span>|[<span data-ttu-id="8e664-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="8e664-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="8e664-151">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="8e664-151">The source of threat assessment request.</span></span> <span data-ttu-id="8e664-152">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="8e664-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="8e664-153">status</span><span class="sxs-lookup"><span data-stu-id="8e664-153">status</span></span>|[<span data-ttu-id="8e664-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="8e664-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="8e664-155">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="8e664-155">The assessment process status.</span></span> <span data-ttu-id="8e664-156">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="8e664-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e664-157">Связи</span><span class="sxs-lookup"><span data-stu-id="8e664-157">Relationships</span></span>

| <span data-ttu-id="8e664-158">Связь</span><span class="sxs-lookup"><span data-stu-id="8e664-158">Relationship</span></span> | <span data-ttu-id="8e664-159">Тип</span><span class="sxs-lookup"><span data-stu-id="8e664-159">Type</span></span>        | <span data-ttu-id="8e664-160">Описание</span><span class="sxs-lookup"><span data-stu-id="8e664-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8e664-161">results</span><span class="sxs-lookup"><span data-stu-id="8e664-161">results</span></span>|<span data-ttu-id="8e664-162">[коллекция threatAssessmentResult](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="8e664-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="8e664-163">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="8e664-163">A collection of threat assessment results.</span></span> <span data-ttu-id="8e664-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8e664-164">Read-only.</span></span> <span data-ttu-id="8e664-165">По умолчанию это `GET /threatAssessmentRequests/{id}` свойство не возвращается, если оно не `$expand` применяется.</span><span class="sxs-lookup"><span data-stu-id="8e664-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e664-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e664-166">JSON representation</span></span>

<span data-ttu-id="8e664-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e664-167">The following is a JSON representation of the resource.</span></span>

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

