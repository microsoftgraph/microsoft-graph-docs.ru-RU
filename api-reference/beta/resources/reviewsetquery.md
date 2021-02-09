---
title: Тип ресурса reviewSetQuery
description: Запросы набора для проверки используются для запроса и кэша данных, хранимые в наборе отзывов eDiscovery
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f622f79c9103e704be93ffd97af37c1d188736f6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153489"
---
# <a name="reviewsetquery-resource-type"></a><span data-ttu-id="70190-103">Тип ресурса reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="70190-103">reviewSetQuery resource type</span></span>

<span data-ttu-id="70190-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70190-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70190-105">Запросы набора для проверки используются для запроса и кэш сбор данных, хранимые в наборе отзывов eDiscovery. [](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="70190-105">Review set queries are used to query and cull data stored in an eDiscovery [reviewSet](reviewset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="70190-106">Методы</span><span class="sxs-lookup"><span data-stu-id="70190-106">Methods</span></span>

| <span data-ttu-id="70190-107">Метод</span><span class="sxs-lookup"><span data-stu-id="70190-107">Method</span></span>       | <span data-ttu-id="70190-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70190-108">Return Type</span></span> | <span data-ttu-id="70190-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70190-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="70190-110">Список запросов</span><span class="sxs-lookup"><span data-stu-id="70190-110">List queries</span></span>](../api/reviewsetquery-list.md) | <span data-ttu-id="70190-111">[Коллекция reviewSetQuery](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="70190-111">[reviewSetQuery](reviewsetquery.md) collection</span></span> | <span data-ttu-id="70190-112">Список запросов набора для проверки в наборе для проверки.</span><span class="sxs-lookup"><span data-stu-id="70190-112">List the review set queries in a review set.</span></span> |
| [<span data-ttu-id="70190-113">Создание запросов</span><span class="sxs-lookup"><span data-stu-id="70190-113">Create queries</span></span>](../api/reviewsetquery-post.md) | [<span data-ttu-id="70190-114">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="70190-114">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="70190-115">Создайте запрос набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="70190-115">Create a new review set query.</span></span> |
| [<span data-ttu-id="70190-116">Получить запросы</span><span class="sxs-lookup"><span data-stu-id="70190-116">Get queries</span></span>](../api/reviewsetquery-get.md) | [<span data-ttu-id="70190-117">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="70190-117">reviewSetQuery</span></span>](reviewsetquery.md) | <span data-ttu-id="70190-118">Чтение свойств и связей объекта **reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="70190-118">Read the properties and relationships of a **reviewSetQuery** object.</span></span> |
| [<span data-ttu-id="70190-119">Обновление запросов</span><span class="sxs-lookup"><span data-stu-id="70190-119">Update queries</span></span>](../api/reviewsetquery-update.md) | <span data-ttu-id="70190-120">Нет</span><span class="sxs-lookup"><span data-stu-id="70190-120">None</span></span> | <span data-ttu-id="70190-121">Обновление запроса набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="70190-121">Update a review set query.</span></span> |
| [<span data-ttu-id="70190-122">Удаление запросов</span><span class="sxs-lookup"><span data-stu-id="70190-122">Delete queries</span></span>](../api/reviewsetquery-delete.md) | <span data-ttu-id="70190-123">Нет</span><span class="sxs-lookup"><span data-stu-id="70190-123">None</span></span> | <span data-ttu-id="70190-124">Удаление запроса набора для проверки.</span><span class="sxs-lookup"><span data-stu-id="70190-124">Delete review set query.</span></span> |

## <a name="properties"></a><span data-ttu-id="70190-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="70190-125">Properties</span></span>

| <span data-ttu-id="70190-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="70190-126">Property</span></span>     | <span data-ttu-id="70190-127">Тип</span><span class="sxs-lookup"><span data-stu-id="70190-127">Type</span></span>        | <span data-ttu-id="70190-128">Описание</span><span class="sxs-lookup"><span data-stu-id="70190-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="70190-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="70190-129">createdBy</span></span> | [<span data-ttu-id="70190-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="70190-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="70190-131">Пользователь, создавший запрос.</span><span class="sxs-lookup"><span data-stu-id="70190-131">The user who created the query.</span></span> |
| <span data-ttu-id="70190-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="70190-132">createdDateTime</span></span> |<span data-ttu-id="70190-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70190-133">DateTimeOffset</span></span>| <span data-ttu-id="70190-134">Время и дата создания запроса.</span><span class="sxs-lookup"><span data-stu-id="70190-134">The time and date when the query was created.</span></span> <span data-ttu-id="70190-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="70190-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="70190-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="70190-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="70190-137">displayName</span><span class="sxs-lookup"><span data-stu-id="70190-137">displayName</span></span> | <span data-ttu-id="70190-138">String</span><span class="sxs-lookup"><span data-stu-id="70190-138">String</span></span> | <span data-ttu-id="70190-139">Имя запроса</span><span class="sxs-lookup"><span data-stu-id="70190-139">The name of the query</span></span>|
| <span data-ttu-id="70190-140">id</span><span class="sxs-lookup"><span data-stu-id="70190-140">id</span></span> |<span data-ttu-id="70190-141">String</span><span class="sxs-lookup"><span data-stu-id="70190-141">String</span></span>| <span data-ttu-id="70190-142">Уникальный идентификатор запроса.</span><span class="sxs-lookup"><span data-stu-id="70190-142">The unique identifier of the query.</span></span> <span data-ttu-id="70190-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="70190-143">Read-only.</span></span>|
| <span data-ttu-id="70190-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="70190-144">lastModifiedBy</span></span> | [<span data-ttu-id="70190-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="70190-145">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="70190-146">Пользователь, который последним изменил запрос.</span><span class="sxs-lookup"><span data-stu-id="70190-146">The user who last modified the query.</span></span> |
| <span data-ttu-id="70190-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="70190-147">lastModifiedDateTime</span></span> |<span data-ttu-id="70190-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="70190-148">DateTimeOffset</span></span> | <span data-ttu-id="70190-149">Дата и время последнего изменения запроса.</span><span class="sxs-lookup"><span data-stu-id="70190-149">The date and time the query was last modified.</span></span> <span data-ttu-id="70190-150">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="70190-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="70190-151">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="70190-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
| <span data-ttu-id="70190-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="70190-152">query</span></span> | <span data-ttu-id="70190-153">String</span><span class="sxs-lookup"><span data-stu-id="70190-153">String</span></span> | <span data-ttu-id="70190-154">Строка запроса в KQL (язык запросов по ключевым словам).</span><span class="sxs-lookup"><span data-stu-id="70190-154">The query string in KQL (Keyword Query Language) query.</span></span> <span data-ttu-id="70190-155">Дополнительные сведения см. в [полях метаданных документа в Advanced eDiscovery.](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery)</span><span class="sxs-lookup"><span data-stu-id="70190-155">For details, see [Document metadata fields in Advanced eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/document-metadata-fields-in-advanced-ediscovery).</span></span>  <span data-ttu-id="70190-156">Это поле сопо карте непосредственно с условием ключевых слов.</span><span class="sxs-lookup"><span data-stu-id="70190-156">This field maps directly to the keywords condition.</span></span>  <span data-ttu-id="70190-157">Поиск можно уточнить с помощью полей, перечисленных в имени поля для поиска, в *паре* со значениями; например, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span><span class="sxs-lookup"><span data-stu-id="70190-157">You can refine searches by using fields listed in the *searchable field name* paired with values; for example, *subject:"Quarterly Financials" AND Date>=06/01/2016 AND Date<=07/01/2016*</span></span> |

## <a name="relationships"></a><span data-ttu-id="70190-158">Связи</span><span class="sxs-lookup"><span data-stu-id="70190-158">Relationships</span></span>

<span data-ttu-id="70190-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="70190-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70190-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="70190-160">JSON representation</span></span>

<span data-ttu-id="70190-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70190-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSetQuery",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSetQuery",
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
