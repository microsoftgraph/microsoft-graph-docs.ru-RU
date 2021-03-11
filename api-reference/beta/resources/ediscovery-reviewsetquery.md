---
title: reviewSetQuery resource type
description: Представляет запрос набора обзоров, который используется для запроса и отсеить данные, хранимые в обзоре eDiscoverySet.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8eb674ed70eac47d4e29d127ebfc9f48b7b988a1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720321"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="9ee16-103">reviewSetQuery resource type</span><span class="sxs-lookup"><span data-stu-id="9ee16-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="9ee16-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9ee16-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ee16-105">Представляет запрос набора обзоров, который используется для запроса и отсеить данные, хранимые в обзоре [eDiscoverySet.](ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="9ee16-105">Represents a review set query, which is used to query and cull data stored in an eDiscovery [reviewSet](ediscovery-reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9ee16-106">Методы</span><span class="sxs-lookup"><span data-stu-id="9ee16-106">Methods</span></span>

| <span data-ttu-id="9ee16-107">Метод</span><span class="sxs-lookup"><span data-stu-id="9ee16-107">Method</span></span>       | <span data-ttu-id="9ee16-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ee16-108">Return Type</span></span> | <span data-ttu-id="9ee16-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9ee16-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9ee16-110">Запросы списка</span><span class="sxs-lookup"><span data-stu-id="9ee16-110">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md) | <span data-ttu-id="9ee16-111">[коллекция microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="9ee16-111">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span> | <span data-ttu-id="9ee16-112">Список запросов набора отзывов в наборе обзоров.</span><span class="sxs-lookup"><span data-stu-id="9ee16-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="9ee16-113">Создание запросов</span><span class="sxs-lookup"><span data-stu-id="9ee16-113">Create queries</span></span>](../api/ediscovery-reviewsetquery-post.md) | [<span data-ttu-id="9ee16-114">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="9ee16-114">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="9ee16-115">Создайте новый запрос набора обзоров.</span><span class="sxs-lookup"><span data-stu-id="9ee16-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="9ee16-116">Получить запросы</span><span class="sxs-lookup"><span data-stu-id="9ee16-116">Get queries</span></span>](../api/ediscovery-reviewsetquery-get.md) | [<span data-ttu-id="9ee16-117">microsoft.graph.ediscovery.reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="9ee16-117">microsoft.graph.ediscovery.reviewSetQuery</span></span>](ediscovery-reviewsetquery.md) | <span data-ttu-id="9ee16-118">Ознакомьтесь с свойствами и отношениями объекта **reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="9ee16-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="9ee16-119">Обновление обзораSetQuery</span><span class="sxs-lookup"><span data-stu-id="9ee16-119">Update reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-update.md) | <span data-ttu-id="9ee16-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9ee16-120">None</span></span> | <span data-ttu-id="9ee16-121">Обновление запроса набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="9ee16-121">Update a review set query.</span></span> |
| [<span data-ttu-id="9ee16-122">Удаление просмотретьSetQuery</span><span class="sxs-lookup"><span data-stu-id="9ee16-122">Delete reviewSetQuery</span></span>](../api/ediscovery-reviewsetquery-delete.md) | <span data-ttu-id="9ee16-123">Нет</span><span class="sxs-lookup"><span data-stu-id="9ee16-123">None</span></span> | <span data-ttu-id="9ee16-124">Удаление запроса набора обзоров.</span><span class="sxs-lookup"><span data-stu-id="9ee16-124">Delete review set query.</span></span> |
| [<span data-ttu-id="9ee16-125">applyTags</span><span class="sxs-lookup"><span data-stu-id="9ee16-125">applyTags</span></span>](../api/ediscovery-reviewsetquery-applytags.md)|<span data-ttu-id="9ee16-126">Нет</span><span class="sxs-lookup"><span data-stu-id="9ee16-126">None</span></span>|<span data-ttu-id="9ee16-127">Применяйте теги к документам, которые соответствуют указанному запросу.</span><span class="sxs-lookup"><span data-stu-id="9ee16-127">Apply tags to documents that match the specified query.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ee16-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ee16-128">Properties</span></span>

| <span data-ttu-id="9ee16-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ee16-129">Property</span></span>     | <span data-ttu-id="9ee16-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9ee16-130">Type</span></span>        | <span data-ttu-id="9ee16-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9ee16-131">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9ee16-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="9ee16-132">createdBy</span></span> | [<span data-ttu-id="9ee16-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="9ee16-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="9ee16-134">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="9ee16-134">The user who created the query.</span></span> |
| <span data-ttu-id="9ee16-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee16-135">createdDateTime</span></span> |<span data-ttu-id="9ee16-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee16-136">DateTimeOffset</span></span>| <span data-ttu-id="9ee16-137">Время и дата создания запроса.</span><span class="sxs-lookup"><span data-stu-id="9ee16-137">The time and date when the query was created.</span></span> <span data-ttu-id="9ee16-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9ee16-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9ee16-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9ee16-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
| <span data-ttu-id="9ee16-140">displayName</span><span class="sxs-lookup"><span data-stu-id="9ee16-140">displayName</span></span> | <span data-ttu-id="9ee16-141">String</span><span class="sxs-lookup"><span data-stu-id="9ee16-141">String</span></span> | <span data-ttu-id="9ee16-142">Имя запроса.</span><span class="sxs-lookup"><span data-stu-id="9ee16-142">The name of the query.</span></span>|
| <span data-ttu-id="9ee16-143">id</span><span class="sxs-lookup"><span data-stu-id="9ee16-143">id</span></span> |<span data-ttu-id="9ee16-144">String</span><span class="sxs-lookup"><span data-stu-id="9ee16-144">String</span></span>| <span data-ttu-id="9ee16-145">Уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="9ee16-145">The unique identifier of the query.</span></span> <span data-ttu-id="9ee16-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ee16-146">Read-only.</span></span>|
| <span data-ttu-id="9ee16-147">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="9ee16-147">lastModifiedBy</span></span> | [<span data-ttu-id="9ee16-148">identitySet</span><span class="sxs-lookup"><span data-stu-id="9ee16-148">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="9ee16-149">Пользователь, который в последний раз изменил запрос.</span><span class="sxs-lookup"><span data-stu-id="9ee16-149">The user who last modified the query.</span></span> |
| <span data-ttu-id="9ee16-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ee16-150">lastModifiedDateTime</span></span> |<span data-ttu-id="9ee16-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ee16-151">DateTimeOffset</span></span> | <span data-ttu-id="9ee16-152">Дата и время последнего изменения запроса.</span><span class="sxs-lookup"><span data-stu-id="9ee16-152">The date and time the query was last modified.</span></span> <span data-ttu-id="9ee16-153">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9ee16-153">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9ee16-154">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9ee16-154">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
| <span data-ttu-id="9ee16-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ee16-155">query</span></span> | <span data-ttu-id="9ee16-156">String</span><span class="sxs-lookup"><span data-stu-id="9ee16-156">String</span></span> | <span data-ttu-id="9ee16-157">Строка запроса в запросе KQL (Язык запросов ключевых слов).</span><span class="sxs-lookup"><span data-stu-id="9ee16-157">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="9ee16-158">Дополнительные сведения см. [в материале Поля метаданных документа в advanced eDiscovery.](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="9ee16-158">For details, see [Document metadata fields in Advanced eDiscovery](/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="9ee16-159">Это поле совмещеется непосредственно с условием ключевых слов.</span><span class="sxs-lookup"><span data-stu-id="9ee16-159">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="9ee16-160">Поиск можно уточнить с помощью  полей, перечисленных в имени поля поиска в паре со значениями; например, *subject:"Quarterly Financials" And Date>=06/01/2016 and Date<=07/01/2016*.</span><span class="sxs-lookup"><span data-stu-id="9ee16-160">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9ee16-161">Связи</span><span class="sxs-lookup"><span data-stu-id="9ee16-161">Relationships</span></span>

<span data-ttu-id="9ee16-162">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9ee16-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ee16-163">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9ee16-163">JSON representation</span></span>

<span data-ttu-id="9ee16-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ee16-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSetQuery",
  "query": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSetQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
