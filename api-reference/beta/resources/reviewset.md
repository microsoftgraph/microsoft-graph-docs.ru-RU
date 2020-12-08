---
title: Тип ресурса Review
description: Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 411de013df02bcd71e851a694664ae010edaf4ab
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597272"
---
# <a name="reviewset-resource-type"></a><span data-ttu-id="2f144-103">Тип ресурса Review</span><span class="sxs-lookup"><span data-stu-id="2f144-103">reviewSet resource type</span></span>

<span data-ttu-id="2f144-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f144-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f144-105">Представляет статический набор хранящихся в электронном формате данных, собранных для использования в запросах судебного разбирательства, расследований или нормативных требований.</span><span class="sxs-lookup"><span data-stu-id="2f144-105">Represents static set of electronically stored information collected for use in a litigation, investigation, or regulatory request.</span></span>

## <a name="methods"></a><span data-ttu-id="2f144-106">Методы</span><span class="sxs-lookup"><span data-stu-id="2f144-106">Methods</span></span>

| <span data-ttu-id="2f144-107">Метод</span><span class="sxs-lookup"><span data-stu-id="2f144-107">Method</span></span>       | <span data-ttu-id="2f144-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2f144-108">Return Type</span></span> | <span data-ttu-id="2f144-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f144-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2f144-110">Список рецензентов</span><span class="sxs-lookup"><span data-stu-id="2f144-110">List reviewSet</span></span>](../api/reviewset-list.md) | <span data-ttu-id="2f144-111">Коллекция [reviewing](reviewset.md)</span><span class="sxs-lookup"><span data-stu-id="2f144-111">[reviewSet](reviewset.md) collection</span></span> | <span data-ttu-id="2f144-112">Получение коллекции наборов проверки.</span><span class="sxs-lookup"><span data-stu-id="2f144-112">Get a collection of review sets.</span></span> |
| [<span data-ttu-id="2f144-113">Получение представления</span><span class="sxs-lookup"><span data-stu-id="2f144-113">Get reviewSet</span></span>](../api/reviewset-get.md) | [<span data-ttu-id="2f144-114">reviewSet</span><span class="sxs-lookup"><span data-stu-id="2f144-114">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="2f144-115">Считывание свойств и связей объекта **reviewing** .</span><span class="sxs-lookup"><span data-stu-id="2f144-115">Read the properties and relationships of a **reviewSet** object.</span></span> |
| [<span data-ttu-id="2f144-116">Создание представления</span><span class="sxs-lookup"><span data-stu-id="2f144-116">Create reviewSet</span></span>](../api/reviewset-post.md) | [<span data-ttu-id="2f144-117">reviewSet</span><span class="sxs-lookup"><span data-stu-id="2f144-117">reviewSet</span></span>](reviewset.md) | <span data-ttu-id="2f144-118">Создайте новый набор рецензирования.</span><span class="sxs-lookup"><span data-stu-id="2f144-118">Create a new review set.</span></span> |
| [<span data-ttu-id="2f144-119">Перечисление запросов</span><span class="sxs-lookup"><span data-stu-id="2f144-119">List queries</span></span>](../api/reviewsetquery-list.md)|<span data-ttu-id="2f144-120">Коллекция [ревиевсеткуери](../resources/reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="2f144-120">[reviewSetQuery](../resources/reviewsetquery.md) collection</span></span>|<span data-ttu-id="2f144-121">Получение ресурсов Ревиевсеткуери из свойства навигации Queries.</span><span class="sxs-lookup"><span data-stu-id="2f144-121">Get the reviewSetQuery resources from the queries navigation property.</span></span>|
| [<span data-ttu-id="2f144-122">Создание запросов</span><span class="sxs-lookup"><span data-stu-id="2f144-122">Create queries</span></span>](../api/reviewsetquery-post.md)|[<span data-ttu-id="2f144-123">reviewSetQuery</span><span class="sxs-lookup"><span data-stu-id="2f144-123">reviewSetQuery</span></span>](../resources/reviewsetquery.md)|<span data-ttu-id="2f144-124">Создание нового объекта Ревиевсеткуери.</span><span class="sxs-lookup"><span data-stu-id="2f144-124">Create a new reviewSetQuery object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f144-125">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f144-125">Properties</span></span>

| <span data-ttu-id="2f144-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f144-126">Property</span></span>     | <span data-ttu-id="2f144-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2f144-127">Type</span></span>        | <span data-ttu-id="2f144-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2f144-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f144-129">createdBy</span><span class="sxs-lookup"><span data-stu-id="2f144-129">createdBy</span></span>        | [<span data-ttu-id="2f144-130">identitySet</span><span class="sxs-lookup"><span data-stu-id="2f144-130">identitySet</span></span>](/graph/api/resources/identityset) | <span data-ttu-id="2f144-131">Пользователь, создавший набор проверки.</span><span class="sxs-lookup"><span data-stu-id="2f144-131">The user who created the review set.</span></span> <span data-ttu-id="2f144-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f144-132">Read-only.</span></span> |
|<span data-ttu-id="2f144-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f144-133">createdDateTime</span></span>  |<span data-ttu-id="2f144-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f144-134">DateTimeOffset</span></span>| <span data-ttu-id="2f144-135">Дата и время создания набора проверки.</span><span class="sxs-lookup"><span data-stu-id="2f144-135">The datetime when the review set was created.</span></span> <span data-ttu-id="2f144-136">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2f144-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2f144-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2f144-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2f144-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f144-138">Read-only.</span></span> |
|<span data-ttu-id="2f144-139">displayName</span><span class="sxs-lookup"><span data-stu-id="2f144-139">displayName</span></span>      |<span data-ttu-id="2f144-140">String</span><span class="sxs-lookup"><span data-stu-id="2f144-140">String</span></span>| <span data-ttu-id="2f144-141">Имя набора проверки.</span><span class="sxs-lookup"><span data-stu-id="2f144-141">The review set name.</span></span> <span data-ttu-id="2f144-142">Имя уникально с максимальным ограничением в 64 символов.</span><span class="sxs-lookup"><span data-stu-id="2f144-142">Name is unique with a maximum limit of 64 characters.</span></span> |
|<span data-ttu-id="2f144-143">id</span><span class="sxs-lookup"><span data-stu-id="2f144-143">id</span></span>               |<span data-ttu-id="2f144-144">String</span><span class="sxs-lookup"><span data-stu-id="2f144-144">String</span></span>| <span data-ttu-id="2f144-145">Уникальный идентификатор набора проверки.</span><span class="sxs-lookup"><span data-stu-id="2f144-145">The review set unique identifier.</span></span> <span data-ttu-id="2f144-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f144-146">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2f144-147">Связи</span><span class="sxs-lookup"><span data-stu-id="2f144-147">Relationships</span></span>

| <span data-ttu-id="2f144-148">Связь</span><span class="sxs-lookup"><span data-stu-id="2f144-148">Relationship</span></span> | <span data-ttu-id="2f144-149">Тип</span><span class="sxs-lookup"><span data-stu-id="2f144-149">Type</span></span>        | <span data-ttu-id="2f144-150">Описание</span><span class="sxs-lookup"><span data-stu-id="2f144-150">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="2f144-151">Просмотр запроса Set</span><span class="sxs-lookup"><span data-stu-id="2f144-151">Review set query</span></span> |<span data-ttu-id="2f144-152">Коллекция [ревиевсеткуери](reviewsetquery.md)</span><span class="sxs-lookup"><span data-stu-id="2f144-152">[reviewSetQuery](reviewsetquery.md) collection</span></span>| <span data-ttu-id="2f144-p105">Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="2f144-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f144-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f144-155">JSON representation</span></span>

<span data-ttu-id="2f144-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f144-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reviewSet",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "@odata.type": "#microsoft.graph.reviewSet",
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
