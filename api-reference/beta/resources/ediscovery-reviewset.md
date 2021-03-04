---
title: тип ресурса reviewSet
description: Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 25c33dd911d9c14d91131508fad37c1fea149b9a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447367"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="4dc7c-103">тип ресурса reviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-103">reviewSet resource type</span></span>

<span data-ttu-id="4dc7c-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4dc7c-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc7c-105">Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="4dc7c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4dc7c-106">Methods</span></span>

| <span data-ttu-id="4dc7c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4dc7c-107">Method</span></span>       | <span data-ttu-id="4dc7c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4dc7c-108">Return Type</span></span> | <span data-ttu-id="4dc7c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc7c-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4dc7c-110">List reviewSets</span><span class="sxs-lookup"><span data-stu-id="4dc7c-110">List reviewSets</span></span>](../api/ediscovery-case-list-reviewsets.md) | <span data-ttu-id="4dc7c-111">[коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="4dc7c-111">[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) collection</span></span> | <span data-ttu-id="4dc7c-112">Получите коллекцию объектов **reviewset.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-112">Get a collection of **reviewset** objects.</span></span> |
| [<span data-ttu-id="4dc7c-113">Создание reviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-113">Create reviewSet</span></span>](../api/ediscovery-case-post-reviewsets.md) | [<span data-ttu-id="4dc7c-114">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-114">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="4dc7c-115">Создайте новый **обзор.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-115">Create a new **reviewset**.</span></span> |
| [<span data-ttu-id="4dc7c-116">Get reviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-116">Get reviewSet</span></span>](../api/ediscovery-reviewset-get.md) | [<span data-ttu-id="4dc7c-117">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-117">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="4dc7c-118">Ознакомьтесь с свойствами и отношениями объекта **reviewSet.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-118">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="4dc7c-119">Запросы списка</span><span class="sxs-lookup"><span data-stu-id="4dc7c-119">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md)|<span data-ttu-id="4dc7c-120">[коллекция microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="4dc7c-120">[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) collection</span></span>|<span data-ttu-id="4dc7c-121">Получите список ресурсов **reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-121">Get a list of **reviewSetQuery** resources.</span></span>|
| [<span data-ttu-id="4dc7c-122">экспорт</span><span class="sxs-lookup"><span data-stu-id="4dc7c-122">export</span></span>](../api/ediscovery-reviewset-export.md) | <span data-ttu-id="4dc7c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="4dc7c-123">None</span></span> | <span data-ttu-id="4dc7c-124">Инициировать экспорт данных из **наборов отзывов.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-124">Initiate an export of data from the **reviewset**.</span></span> |
| [<span data-ttu-id="4dc7c-125">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-125">addToReviewSet</span></span>](../api/ediscovery-reviewset-addtoreviewset.md)|<span data-ttu-id="4dc7c-126">Нет</span><span class="sxs-lookup"><span data-stu-id="4dc7c-126">None</span></span>|<span data-ttu-id="4dc7c-127">Добавление данных из **sourceCollection в** **набор отзывов.**</span><span class="sxs-lookup"><span data-stu-id="4dc7c-127">Add data from a **sourceCollection** to a **reviewset**.</span></span>|

## <a name="properties"></a><span data-ttu-id="4dc7c-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="4dc7c-128">Properties</span></span>

| <span data-ttu-id="4dc7c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4dc7c-129">Property</span></span>     | <span data-ttu-id="4dc7c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc7c-130">Type</span></span>        | <span data-ttu-id="4dc7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc7c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4dc7c-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="4dc7c-132">createdBy</span></span>        | [<span data-ttu-id="4dc7c-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="4dc7c-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="4dc7c-134">Пользователь, создавший набор отзывов.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-134">The user who created the review set.</span></span> <span data-ttu-id="4dc7c-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-135">Read-only.</span></span> |
|<span data-ttu-id="4dc7c-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4dc7c-136">createdDateTime</span></span>  |<span data-ttu-id="4dc7c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dc7c-137">DateTimeOffset</span></span>| <span data-ttu-id="4dc7c-138">Дата создания набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-138">The datetime when the review set was created.</span></span> <span data-ttu-id="4dc7c-139">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="4dc7c-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4dc7c-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4dc7c-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-141">Read-only.</span></span> |
|<span data-ttu-id="4dc7c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="4dc7c-142">displayName</span></span>      |<span data-ttu-id="4dc7c-143">String</span><span class="sxs-lookup"><span data-stu-id="4dc7c-143">String</span></span>| <span data-ttu-id="4dc7c-144">Имя набора обзоров.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-144">The review set name.</span></span> <span data-ttu-id="4dc7c-145">Имя уникально с максимальным ограничением в 64 символа.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-145">The name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="4dc7c-146">id</span><span class="sxs-lookup"><span data-stu-id="4dc7c-146">id</span></span>               |<span data-ttu-id="4dc7c-147">String</span><span class="sxs-lookup"><span data-stu-id="4dc7c-147">String</span></span>| <span data-ttu-id="4dc7c-148">В обзоре установлен уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-148">The review set unique identifier.</span></span> <span data-ttu-id="4dc7c-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-149">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4dc7c-150">Связи</span><span class="sxs-lookup"><span data-stu-id="4dc7c-150">Relationships</span></span>

| <span data-ttu-id="4dc7c-151">Связь</span><span class="sxs-lookup"><span data-stu-id="4dc7c-151">Relationship</span></span> | <span data-ttu-id="4dc7c-152">Тип</span><span class="sxs-lookup"><span data-stu-id="4dc7c-152">Type</span></span>        | <span data-ttu-id="4dc7c-153">Описание</span><span class="sxs-lookup"><span data-stu-id="4dc7c-153">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="4dc7c-154">запросы</span><span class="sxs-lookup"><span data-stu-id="4dc7c-154">queries</span></span> |<span data-ttu-id="4dc7c-155">[коллекция microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="4dc7c-155">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span>| <span data-ttu-id="4dc7c-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4dc7c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4dc7c-158">JSON representation</span></span>

<span data-ttu-id="4dc7c-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4dc7c-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ediscovery.reviewSet",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reviewSet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
