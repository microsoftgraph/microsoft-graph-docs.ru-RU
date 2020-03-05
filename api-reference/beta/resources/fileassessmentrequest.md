---
title: Тип ресурса Филеассессментрекуест
description: Используется для создания и извлечения средства оценки угроз для файлов.
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a7b0b4d83b68acf90aacf71c83169881a2ecdde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498338"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="3dfc2-103">Тип ресурса Филеассессментрекуест</span><span class="sxs-lookup"><span data-stu-id="3dfc2-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="3dfc2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3dfc2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3dfc2-105">Используется для создания и извлечения средства оценки угроз файлов, производных от [среатассессментрекуест](threatAssessmentRequest.md).</span><span class="sxs-lookup"><span data-stu-id="3dfc2-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="3dfc2-106">Файл может быть текстовым файлом или документом Word или двоичным файлом, полученным во вложении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="3dfc2-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3dfc2-107">Methods</span></span>

| <span data-ttu-id="3dfc2-108">Метод</span><span class="sxs-lookup"><span data-stu-id="3dfc2-108">Method</span></span>       | <span data-ttu-id="3dfc2-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3dfc2-109">Return Type</span></span> | <span data-ttu-id="3dfc2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3dfc2-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3dfc2-111">Создание объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3dfc2-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="3dfc2-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3dfc2-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="3dfc2-113">Создание нового запроса на оценку файла путем отправки объекта **филеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="3dfc2-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="3dfc2-114">Получение объекта threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3dfc2-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="3dfc2-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="3dfc2-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="3dfc2-116">Чтение свойств и связей объекта **филеассессментрекуест** .</span><span class="sxs-lookup"><span data-stu-id="3dfc2-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3dfc2-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="3dfc2-117">Properties</span></span>

| <span data-ttu-id="3dfc2-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dfc2-118">Property</span></span>     | <span data-ttu-id="3dfc2-119">Тип</span><span class="sxs-lookup"><span data-stu-id="3dfc2-119">Type</span></span>        | <span data-ttu-id="3dfc2-120">Описание</span><span class="sxs-lookup"><span data-stu-id="3dfc2-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3dfc2-121">контентдата</span><span class="sxs-lookup"><span data-stu-id="3dfc2-121">contentData</span></span>|<span data-ttu-id="3dfc2-122">String</span><span class="sxs-lookup"><span data-stu-id="3dfc2-122">String</span></span>|<span data-ttu-id="3dfc2-123">Содержимое файла в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-123">Base64 encoded file content.</span></span> <span data-ttu-id="3dfc2-124">Не удается вернуть содержимое файла, так как оно не хранится.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="3dfc2-125">fileName</span><span class="sxs-lookup"><span data-stu-id="3dfc2-125">fileName</span></span>|<span data-ttu-id="3dfc2-126">String</span><span class="sxs-lookup"><span data-stu-id="3dfc2-126">String</span></span>|<span data-ttu-id="3dfc2-127">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-127">The file name.</span></span>|
|<span data-ttu-id="3dfc2-128">category</span><span class="sxs-lookup"><span data-stu-id="3dfc2-128">category</span></span>|[<span data-ttu-id="3dfc2-129">среаткатегори</span><span class="sxs-lookup"><span data-stu-id="3dfc2-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="3dfc2-130">Категория угроз.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-130">The threat category.</span></span> <span data-ttu-id="3dfc2-131">Возможные значения: `spam`, `phishing`, `malware`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="3dfc2-132">contentType</span><span class="sxs-lookup"><span data-stu-id="3dfc2-132">contentType</span></span>|[<span data-ttu-id="3dfc2-133">среатассессментконтенттипе</span><span class="sxs-lookup"><span data-stu-id="3dfc2-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="3dfc2-134">Тип контента для оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-134">The content type of threat assessment.</span></span> <span data-ttu-id="3dfc2-135">Возможные значения: `mail`, `url`, `file`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="3dfc2-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="3dfc2-136">createdBy</span></span>|[<span data-ttu-id="3dfc2-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="3dfc2-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="3dfc2-138">Создатель запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="3dfc2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfc2-139">createdDateTime</span></span>|<span data-ttu-id="3dfc2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfc2-140">DateTimeOffset</span></span>|<span data-ttu-id="3dfc2-141">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="3dfc2-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3dfc2-142">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="3dfc2-143">експектедассессмент</span><span class="sxs-lookup"><span data-stu-id="3dfc2-143">expectedAssessment</span></span>|[<span data-ttu-id="3dfc2-144">среатекспектедассессмент</span><span class="sxs-lookup"><span data-stu-id="3dfc2-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="3dfc2-145">Ожидаемая Оценка от отправителя.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-145">The expected assessment from submitter.</span></span> <span data-ttu-id="3dfc2-146">Возможные значения: `block`, `unblock`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="3dfc2-147">id</span><span class="sxs-lookup"><span data-stu-id="3dfc2-147">id</span></span>|<span data-ttu-id="3dfc2-148">String</span><span class="sxs-lookup"><span data-stu-id="3dfc2-148">String</span></span>|<span data-ttu-id="3dfc2-149">Идентификатор запроса оценки угроз — это глобальный уникальный идентификатор (GUID).</span><span class="sxs-lookup"><span data-stu-id="3dfc2-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="3dfc2-150">рекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="3dfc2-150">requestSource</span></span>|[<span data-ttu-id="3dfc2-151">среатассессментрекуестсаурце</span><span class="sxs-lookup"><span data-stu-id="3dfc2-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="3dfc2-152">Источник запроса на оценку угроз.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-152">The source of threat assessment request.</span></span> <span data-ttu-id="3dfc2-153">Возможные значения: `user`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="3dfc2-154">status</span><span class="sxs-lookup"><span data-stu-id="3dfc2-154">status</span></span>|[<span data-ttu-id="3dfc2-155">среатассессментстатус</span><span class="sxs-lookup"><span data-stu-id="3dfc2-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="3dfc2-156">Состояние процесса оценки.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-156">The assessment process status.</span></span> <span data-ttu-id="3dfc2-157">Возможные значения: `pending`, `completed`.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3dfc2-158">Связи</span><span class="sxs-lookup"><span data-stu-id="3dfc2-158">Relationships</span></span>

| <span data-ttu-id="3dfc2-159">Связь</span><span class="sxs-lookup"><span data-stu-id="3dfc2-159">Relationship</span></span> | <span data-ttu-id="3dfc2-160">Тип</span><span class="sxs-lookup"><span data-stu-id="3dfc2-160">Type</span></span>        | <span data-ttu-id="3dfc2-161">Описание</span><span class="sxs-lookup"><span data-stu-id="3dfc2-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3dfc2-162">results</span><span class="sxs-lookup"><span data-stu-id="3dfc2-162">results</span></span>|<span data-ttu-id="3dfc2-163">Коллекция [среатассессментресулт](threatassessmentresult.md)</span><span class="sxs-lookup"><span data-stu-id="3dfc2-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="3dfc2-164">Коллекция результатов оценки угроз.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-164">A collection of threat assessment results.</span></span> <span data-ttu-id="3dfc2-165">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-165">Read-only.</span></span> <span data-ttu-id="3dfc2-166">По умолчанию объект `GET /threatAssessmentRequests/{id}` a не возвращает это свойство, пока не `$expand` применено к нему.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3dfc2-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3dfc2-167">JSON representation</span></span>

<span data-ttu-id="3dfc2-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3dfc2-168">The following is a JSON representation of the resource.</span></span>

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
