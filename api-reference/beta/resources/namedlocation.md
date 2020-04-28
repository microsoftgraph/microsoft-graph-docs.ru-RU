---
title: Тип ресурса Намедлокатион
description: Это базовый класс, представляющий имя расположения Azure Active Directory. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4537824971d2417c7f202ad12c1e8c371acf5650
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917140"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="0ee57-104">Тип ресурса Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0ee57-104">namedLocation resource type</span></span>

<span data-ttu-id="0ee57-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ee57-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ee57-106">Это базовый класс, представляющий имя расположения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0ee57-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="0ee57-107">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0ee57-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="0ee57-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0ee57-108">Methods</span></span>

| <span data-ttu-id="0ee57-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0ee57-109">Method</span></span>       | <span data-ttu-id="0ee57-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0ee57-110">Return Type</span></span> | <span data-ttu-id="0ee57-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee57-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0ee57-112">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="0ee57-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0ee57-113">Коллекция [намедлокатион](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0ee57-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="0ee57-114">Получение всех объектов **намедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="0ee57-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0ee57-115">Получение Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0ee57-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="0ee57-116">намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0ee57-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="0ee57-117">Чтение свойств и связей объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="0ee57-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="0ee57-118">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0ee57-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="0ee57-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0ee57-119">None</span></span> | <span data-ttu-id="0ee57-120">Удаление объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="0ee57-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0ee57-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ee57-121">Properties</span></span>

| <span data-ttu-id="0ee57-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ee57-122">Property</span></span>     | <span data-ttu-id="0ee57-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0ee57-123">Type</span></span>        | <span data-ttu-id="0ee57-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0ee57-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ee57-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee57-125">createdDateTime</span></span>|<span data-ttu-id="0ee57-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee57-126">DateTimeOffset</span></span>|<span data-ttu-id="0ee57-127">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0ee57-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ee57-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ee57-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0ee57-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ee57-129">Read-only.</span></span>|
|<span data-ttu-id="0ee57-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0ee57-130">displayName</span></span>|<span data-ttu-id="0ee57-131">Строка</span><span class="sxs-lookup"><span data-stu-id="0ee57-131">String</span></span>|<span data-ttu-id="0ee57-132">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="0ee57-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0ee57-133">id</span><span class="sxs-lookup"><span data-stu-id="0ee57-133">id</span></span>|<span data-ttu-id="0ee57-134">String</span><span class="sxs-lookup"><span data-stu-id="0ee57-134">String</span></span>|<span data-ttu-id="0ee57-135">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="0ee57-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0ee57-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ee57-136">Read-only.</span></span>|
|<span data-ttu-id="0ee57-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ee57-137">modifiedDateTime</span></span>|<span data-ttu-id="0ee57-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ee57-138">DateTimeOffset</span></span>|<span data-ttu-id="0ee57-139">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0ee57-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0ee57-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0ee57-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0ee57-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ee57-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ee57-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ee57-142">Relationships</span></span>

<span data-ttu-id="0ee57-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ee57-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ee57-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0ee57-144">JSON representation</span></span>

<span data-ttu-id="0ee57-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ee57-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
