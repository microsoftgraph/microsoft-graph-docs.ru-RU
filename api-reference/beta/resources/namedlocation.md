---
title: Тип ресурса Намедлокатион
description: Это базовый класс, представляющий имя расположения Azure Active Directory. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fda5c1854dee5e6ce108f2cc46b95c6a69c64230
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089315"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="0a5cc-104">Тип ресурса Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0a5cc-104">namedLocation resource type</span></span>

<span data-ttu-id="0a5cc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a5cc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a5cc-106">Это базовый класс, представляющий имя расположения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="0a5cc-107">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="0a5cc-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0a5cc-108">Methods</span></span>

| <span data-ttu-id="0a5cc-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0a5cc-109">Method</span></span>       | <span data-ttu-id="0a5cc-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0a5cc-110">Return Type</span></span> | <span data-ttu-id="0a5cc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a5cc-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0a5cc-112">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="0a5cc-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0a5cc-113">Коллекция [намедлокатион](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0a5cc-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="0a5cc-114">Получение всех объектов **намедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0a5cc-115">Получение Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0a5cc-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="0a5cc-116">намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0a5cc-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="0a5cc-117">Чтение свойств и связей объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="0a5cc-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="0a5cc-118">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="0a5cc-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="0a5cc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0a5cc-119">None</span></span> | <span data-ttu-id="0a5cc-120">Удаление объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="0a5cc-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a5cc-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a5cc-121">Properties</span></span>

| <span data-ttu-id="0a5cc-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a5cc-122">Property</span></span>     | <span data-ttu-id="0a5cc-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0a5cc-123">Type</span></span>        | <span data-ttu-id="0a5cc-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0a5cc-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a5cc-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a5cc-125">createdDateTime</span></span>|<span data-ttu-id="0a5cc-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a5cc-126">DateTimeOffset</span></span>|<span data-ttu-id="0a5cc-127">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0a5cc-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0a5cc-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-129">Read-only.</span></span>|
|<span data-ttu-id="0a5cc-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0a5cc-130">displayName</span></span>|<span data-ttu-id="0a5cc-131">Строка</span><span class="sxs-lookup"><span data-stu-id="0a5cc-131">String</span></span>|<span data-ttu-id="0a5cc-132">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0a5cc-133">id</span><span class="sxs-lookup"><span data-stu-id="0a5cc-133">id</span></span>|<span data-ttu-id="0a5cc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0a5cc-134">String</span></span>|<span data-ttu-id="0a5cc-135">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0a5cc-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-136">Read-only.</span></span>|
|<span data-ttu-id="0a5cc-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a5cc-137">modifiedDateTime</span></span>|<span data-ttu-id="0a5cc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a5cc-138">DateTimeOffset</span></span>|<span data-ttu-id="0a5cc-139">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0a5cc-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="0a5cc-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a5cc-142">Связи</span><span class="sxs-lookup"><span data-stu-id="0a5cc-142">Relationships</span></span>

<span data-ttu-id="0a5cc-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a5cc-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0a5cc-144">JSON representation</span></span>

<span data-ttu-id="0a5cc-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a5cc-145">The following is a JSON representation of the resource.</span></span>

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


