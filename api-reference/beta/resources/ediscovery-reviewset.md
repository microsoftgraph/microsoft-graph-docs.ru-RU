---
title: тип ресурса reviewSet
description: Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bcb21fece207e9e4d98fa7a0fc612f886e5ab0e6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720338"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="b85f2-103">тип ресурса reviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-103">reviewSet resource type</span></span>

<span data-ttu-id="b85f2-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="b85f2-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b85f2-105">Представляет статический набор сведений, хранимых в электронной форме, собранных для использования в судебном, следственном или нормативном запросе.</span><span class="sxs-lookup"><span data-stu-id="b85f2-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="b85f2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b85f2-106">Methods</span></span>

| <span data-ttu-id="b85f2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b85f2-107">Method</span></span>       | <span data-ttu-id="b85f2-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b85f2-108">Return Type</span></span> | <span data-ttu-id="b85f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b85f2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b85f2-110">List reviewSets</span><span class="sxs-lookup"><span data-stu-id="b85f2-110">List reviewSets</span></span>](../api/ediscovery-case-list-reviewsets.md) | <span data-ttu-id="b85f2-111">[коллекция microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="b85f2-111">[microsoft.graph.ediscovery.reviewSet](../resources/ediscovery-reviewset.md) collection</span></span> | <span data-ttu-id="b85f2-112">Получите коллекцию объектов **reviewset.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-112">Get a collection of **reviewset** objects.</span></span> |
| [<span data-ttu-id="b85f2-113">Создание reviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-113">Create reviewSet</span></span>](../api/ediscovery-case-post-reviewsets.md) | [<span data-ttu-id="b85f2-114">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-114">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="b85f2-115">Создайте новый **обзор.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-115">Create a new **reviewset**.</span></span> |
| [<span data-ttu-id="b85f2-116">Get reviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-116">Get reviewSet</span></span>](../api/ediscovery-reviewset-get.md) | [<span data-ttu-id="b85f2-117">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-117">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md) | <span data-ttu-id="b85f2-118">Ознакомьтесь с свойствами и отношениями объекта **reviewSet.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-118">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="b85f2-119">Запросы списка</span><span class="sxs-lookup"><span data-stu-id="b85f2-119">List queries</span></span>](../api/ediscovery-reviewsetquery-list.md)|<span data-ttu-id="b85f2-120">[коллекция microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="b85f2-120">[microsoft.graph.ediscovery.reviewSetQuery](../resources/ediscovery-reviewsetquery.md) collection</span></span>|<span data-ttu-id="b85f2-121">Получите список ресурсов **reviewSetQuery.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-121">Get a list of **reviewSetQuery** resources.</span></span>|
| [<span data-ttu-id="b85f2-122">экспорт</span><span class="sxs-lookup"><span data-stu-id="b85f2-122">export</span></span>](../api/ediscovery-reviewset-export.md) | <span data-ttu-id="b85f2-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b85f2-123">None</span></span> | <span data-ttu-id="b85f2-124">Инициировать экспорт данных из **наборов отзывов.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-124">Initiate an export of data from the **reviewset**.</span></span> |
| [<span data-ttu-id="b85f2-125">addToReviewSet</span><span class="sxs-lookup"><span data-stu-id="b85f2-125">addToReviewSet</span></span>](../api/ediscovery-reviewset-addtoreviewset.md)|<span data-ttu-id="b85f2-126">Нет</span><span class="sxs-lookup"><span data-stu-id="b85f2-126">None</span></span>|<span data-ttu-id="b85f2-127">Добавление данных из **sourceCollection в** **набор отзывов.**</span><span class="sxs-lookup"><span data-stu-id="b85f2-127">Add data from a **sourceCollection** to a **reviewset**.</span></span>|

## <a name="properties"></a><span data-ttu-id="b85f2-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="b85f2-128">Properties</span></span>

| <span data-ttu-id="b85f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b85f2-129">Property</span></span>     | <span data-ttu-id="b85f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b85f2-130">Type</span></span>        | <span data-ttu-id="b85f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b85f2-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b85f2-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="b85f2-132">createdBy</span></span>        | [<span data-ttu-id="b85f2-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="b85f2-133">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="b85f2-134">Пользователь, создавший набор отзывов.</span><span class="sxs-lookup"><span data-stu-id="b85f2-134">The user who created the review set.</span></span> <span data-ttu-id="b85f2-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b85f2-135">Read-only.</span></span> |
|<span data-ttu-id="b85f2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b85f2-136">createdDateTime</span></span>  |<span data-ttu-id="b85f2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b85f2-137">DateTimeOffset</span></span>| <span data-ttu-id="b85f2-138">Дата создания набора отзывов.</span><span class="sxs-lookup"><span data-stu-id="b85f2-138">The datetime when the review set was created.</span></span> <span data-ttu-id="b85f2-139">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="b85f2-139">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b85f2-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b85f2-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b85f2-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b85f2-141">Read-only.</span></span> |
|<span data-ttu-id="b85f2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b85f2-142">displayName</span></span>      |<span data-ttu-id="b85f2-143">String</span><span class="sxs-lookup"><span data-stu-id="b85f2-143">String</span></span>| <span data-ttu-id="b85f2-144">Имя набора обзоров.</span><span class="sxs-lookup"><span data-stu-id="b85f2-144">The review set name.</span></span> <span data-ttu-id="b85f2-145">Имя уникально с максимальным ограничением в 64 символа.</span><span class="sxs-lookup"><span data-stu-id="b85f2-145">The name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="b85f2-146">id</span><span class="sxs-lookup"><span data-stu-id="b85f2-146">id</span></span>               |<span data-ttu-id="b85f2-147">String</span><span class="sxs-lookup"><span data-stu-id="b85f2-147">String</span></span>| <span data-ttu-id="b85f2-148">В обзоре установлен уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b85f2-148">The review set unique identifier.</span></span> <span data-ttu-id="b85f2-149">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b85f2-149">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b85f2-150">Связи</span><span class="sxs-lookup"><span data-stu-id="b85f2-150">Relationships</span></span>

| <span data-ttu-id="b85f2-151">Связь</span><span class="sxs-lookup"><span data-stu-id="b85f2-151">Relationship</span></span> | <span data-ttu-id="b85f2-152">Тип</span><span class="sxs-lookup"><span data-stu-id="b85f2-152">Type</span></span>        | <span data-ttu-id="b85f2-153">Описание</span><span class="sxs-lookup"><span data-stu-id="b85f2-153">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b85f2-154">запросы</span><span class="sxs-lookup"><span data-stu-id="b85f2-154">queries</span></span> |<span data-ttu-id="b85f2-155">[коллекция microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="b85f2-155">[microsoft.graph.ediscovery.reviewSetQuery](ediscovery-reviewsetquery.md) collection</span></span>| <span data-ttu-id="b85f2-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="b85f2-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b85f2-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b85f2-158">JSON representation</span></span>

<span data-ttu-id="b85f2-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b85f2-159">The following is a JSON representation of the resource.</span></span>

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
