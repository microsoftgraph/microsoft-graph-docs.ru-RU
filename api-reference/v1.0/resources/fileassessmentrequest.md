---
title: Тип ресурса Филеассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для файлов.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8f436ad2fb519f84ce4d4b59ba7cf5d24fa56066
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591434"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="5a3c8-103">Тип ресурса Филеассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="5a3c8-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="5a3c8-104">Используется для создания и извлечения средства оценки угроз файлов, производных от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="5a3c8-104">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="5a3c8-105">Файл может быть текстовым файлом или документом Word или двоичным файлом, полученным во вложении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-105">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="5a3c8-106">Методы</span><span class="sxs-lookup"><span data-stu-id="5a3c8-106">Methods</span></span>

| <span data-ttu-id="5a3c8-107">Метод</span><span class="sxs-lookup"><span data-stu-id="5a3c8-107">Method</span></span>       | <span data-ttu-id="5a3c8-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a3c8-108">Return Type</span></span> | <span data-ttu-id="5a3c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a3c8-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5a3c8-110">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a3c8-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="5a3c8-111">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a3c8-111">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="5a3c8-112">Создание нового запроса на оценку файла путем отправки объекта **филеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="5a3c8-112">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="5a3c8-113">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a3c8-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="5a3c8-114">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="5a3c8-114">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="5a3c8-115">Чтение свойств и связей объекта **филеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="5a3c8-115">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a3c8-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a3c8-116">Properties</span></span>

| <span data-ttu-id="5a3c8-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a3c8-117">Property</span></span>     | <span data-ttu-id="5a3c8-118">Тип</span><span class="sxs-lookup"><span data-stu-id="5a3c8-118">Type</span></span>        | <span data-ttu-id="5a3c8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5a3c8-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a3c8-120">контентдата</span><span class="sxs-lookup"><span data-stu-id="5a3c8-120">contentData</span></span>|<span data-ttu-id="5a3c8-121">String</span><span class="sxs-lookup"><span data-stu-id="5a3c8-121">String</span></span>|<span data-ttu-id="5a3c8-122">Содержимое файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-122">Base64 encoded file content.</span></span> <span data-ttu-id="5a3c8-123">Не удается вернуть содержимое файла, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="5a3c8-124">fileName</span><span class="sxs-lookup"><span data-stu-id="5a3c8-124">fileName</span></span>|<span data-ttu-id="5a3c8-125">String</span><span class="sxs-lookup"><span data-stu-id="5a3c8-125">String</span></span>|<span data-ttu-id="5a3c8-126">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-126">The file name.</span></span>|
|<span data-ttu-id="5a3c8-127">category</span><span class="sxs-lookup"><span data-stu-id="5a3c8-127">category</span></span>|[<span data-ttu-id="5a3c8-128">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="5a3c8-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="5a3c8-129">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-129">The threat category.</span></span> <span data-ttu-id="5a3c8-130">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="5a3c8-131">contentType</span><span class="sxs-lookup"><span data-stu-id="5a3c8-131">contentType</span></span>|[<span data-ttu-id="5a3c8-132">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="5a3c8-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="5a3c8-133">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-133">The content type of threat assessment.</span></span> <span data-ttu-id="5a3c8-134">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="5a3c8-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="5a3c8-135">createdBy</span></span>|[<span data-ttu-id="5a3c8-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a3c8-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="5a3c8-137">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="5a3c8-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a3c8-138">createdDateTime</span></span>|<span data-ttu-id="5a3c8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a3c8-139">DateTimeOffset</span></span>|<span data-ttu-id="5a3c8-140">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5a3c8-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5a3c8-141">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5a3c8-142">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="5a3c8-142">expectedAssessment</span></span>|[<span data-ttu-id="5a3c8-143">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="5a3c8-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="5a3c8-144">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-144">The expected assessment from submitter.</span></span> <span data-ttu-id="5a3c8-145">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="5a3c8-146">id</span><span class="sxs-lookup"><span data-stu-id="5a3c8-146">id</span></span>|<span data-ttu-id="5a3c8-147">String</span><span class="sxs-lookup"><span data-stu-id="5a3c8-147">String</span></span>|<span data-ttu-id="5a3c8-148">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="5a3c8-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="5a3c8-149">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="5a3c8-149">requestSource</span></span>|[<span data-ttu-id="5a3c8-150">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="5a3c8-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="5a3c8-151">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-151">The source of threat assessment request.</span></span> <span data-ttu-id="5a3c8-152">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="5a3c8-153">status</span><span class="sxs-lookup"><span data-stu-id="5a3c8-153">status</span></span>|[<span data-ttu-id="5a3c8-154">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="5a3c8-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="5a3c8-155">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-155">The assessment process status.</span></span> <span data-ttu-id="5a3c8-156">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a3c8-157">Связи</span><span class="sxs-lookup"><span data-stu-id="5a3c8-157">Relationships</span></span>

| <span data-ttu-id="5a3c8-158">Связь</span><span class="sxs-lookup"><span data-stu-id="5a3c8-158">Relationship</span></span> | <span data-ttu-id="5a3c8-159">Тип</span><span class="sxs-lookup"><span data-stu-id="5a3c8-159">Type</span></span>        | <span data-ttu-id="5a3c8-160">Описание</span><span class="sxs-lookup"><span data-stu-id="5a3c8-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a3c8-161">results</span><span class="sxs-lookup"><span data-stu-id="5a3c8-161">results</span></span>|<span data-ttu-id="5a3c8-162">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="5a3c8-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="5a3c8-163">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-163">A collection of threat assessment results.</span></span> <span data-ttu-id="5a3c8-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-164">Read-only.</span></span> <span data-ttu-id="5a3c8-165">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a3c8-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a3c8-166">JSON representation</span></span>

<span data-ttu-id="5a3c8-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a3c8-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
  "baseType": "",
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
