---
title: Тип ресурса namedLocation
description: Это базовый класс, который представляет именуемую позицию Azure Active Directory. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1e714bb949c79d65a1563fe51bb5e1f16d6d67c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156730"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="2237c-104">Тип ресурса namedLocation</span><span class="sxs-lookup"><span data-stu-id="2237c-104">namedLocation resource type</span></span>

<span data-ttu-id="2237c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2237c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2237c-106">Это базовый класс, который представляет именуемую позицию Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2237c-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="2237c-107">Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="2237c-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="2237c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2237c-108">Methods</span></span>

| <span data-ttu-id="2237c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2237c-109">Method</span></span>       | <span data-ttu-id="2237c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2237c-110">Return Type</span></span> | <span data-ttu-id="2237c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2237c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2237c-112">Список namedLocations</span><span class="sxs-lookup"><span data-stu-id="2237c-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="2237c-113">[Коллекция namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="2237c-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="2237c-114">Получите все **объекты namedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="2237c-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="2237c-115">Получить namedLocation</span><span class="sxs-lookup"><span data-stu-id="2237c-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="2237c-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="2237c-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="2237c-117">Чтение свойств и связей объекта **namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="2237c-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="2237c-118">Удаление namedLocation</span><span class="sxs-lookup"><span data-stu-id="2237c-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="2237c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2237c-119">None</span></span> | <span data-ttu-id="2237c-120">Удаление объекта **namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="2237c-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="2237c-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="2237c-121">Properties</span></span>

| <span data-ttu-id="2237c-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="2237c-122">Property</span></span>     | <span data-ttu-id="2237c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="2237c-123">Type</span></span>        | <span data-ttu-id="2237c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="2237c-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2237c-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2237c-125">createdDateTime</span></span>|<span data-ttu-id="2237c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2237c-126">DateTimeOffset</span></span>|<span data-ttu-id="2237c-127">Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="2237c-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2237c-128">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2237c-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2237c-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2237c-129">Read-only.</span></span>|
|<span data-ttu-id="2237c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="2237c-130">displayName</span></span>|<span data-ttu-id="2237c-131">String</span><span class="sxs-lookup"><span data-stu-id="2237c-131">String</span></span>|<span data-ttu-id="2237c-132">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="2237c-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="2237c-133">id</span><span class="sxs-lookup"><span data-stu-id="2237c-133">id</span></span>|<span data-ttu-id="2237c-134">String</span><span class="sxs-lookup"><span data-stu-id="2237c-134">String</span></span>|<span data-ttu-id="2237c-135">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="2237c-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="2237c-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2237c-136">Read-only.</span></span>|
|<span data-ttu-id="2237c-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2237c-137">modifiedDateTime</span></span>|<span data-ttu-id="2237c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2237c-138">DateTimeOffset</span></span>|<span data-ttu-id="2237c-139">Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="2237c-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2237c-140">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2237c-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="2237c-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2237c-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2237c-142">Связи</span><span class="sxs-lookup"><span data-stu-id="2237c-142">Relationships</span></span>

<span data-ttu-id="2237c-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2237c-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2237c-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2237c-144">JSON representation</span></span>

<span data-ttu-id="2237c-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2237c-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
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


