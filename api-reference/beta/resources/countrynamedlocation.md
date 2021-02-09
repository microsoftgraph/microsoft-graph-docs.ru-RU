---
title: Тип ресурса countryNamedLocation
description: Представляет именуемую позицию Azure Active Directory, определяемую в странах и регионах. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d61621a0cade0bcb479f19ffb0c29050f367401
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157724"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="be27a-104">Тип ресурса countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="be27a-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be27a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be27a-106">Представляет именуемую позицию Azure Active Directory, определяемую в странах и регионах.</span><span class="sxs-lookup"><span data-stu-id="be27a-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="be27a-107">Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="be27a-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="be27a-108">Наследуется от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="be27a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="be27a-109">Methods</span></span>

| <span data-ttu-id="be27a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="be27a-110">Method</span></span>       | <span data-ttu-id="be27a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="be27a-111">Return Type</span></span> | <span data-ttu-id="be27a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="be27a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="be27a-113">Список countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="be27a-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="be27a-114">[коллекция countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="be27a-115">Получить все **объекты countryNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="be27a-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="be27a-116">Создание countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="be27a-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="be27a-118">Создание объекта **countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="be27a-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="be27a-119">Get countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="be27a-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="be27a-121">Чтение свойств и связей объекта **countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="be27a-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="be27a-122">Обновление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="be27a-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="be27a-124">Обновление объекта **countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="be27a-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="be27a-125">Удаление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="be27a-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="be27a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="be27a-126">None</span></span> | <span data-ttu-id="be27a-127">Удаление объекта **countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="be27a-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="be27a-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="be27a-128">Properties</span></span>

| <span data-ttu-id="be27a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be27a-129">Property</span></span>     | <span data-ttu-id="be27a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be27a-130">Type</span></span>        | <span data-ttu-id="be27a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be27a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be27a-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="be27a-132">countriesAndRegions</span></span>|<span data-ttu-id="be27a-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="be27a-133">String collection</span></span>|<span data-ttu-id="be27a-134">Список стран и/или регионов в двухформатном формате, заданном в ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="be27a-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="be27a-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be27a-135">createdDateTime</span></span>|<span data-ttu-id="be27a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be27a-136">DateTimeOffset</span></span>|<span data-ttu-id="be27a-137">Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="be27a-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="be27a-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="be27a-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="be27a-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be27a-139">Read-only.</span></span> <span data-ttu-id="be27a-140">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="be27a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="be27a-141">displayName</span></span>|<span data-ttu-id="be27a-142">String</span><span class="sxs-lookup"><span data-stu-id="be27a-142">String</span></span>|<span data-ttu-id="be27a-143">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="be27a-143">Human-readable name of the location.</span></span> <span data-ttu-id="be27a-144">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="be27a-145">id</span><span class="sxs-lookup"><span data-stu-id="be27a-145">id</span></span>|<span data-ttu-id="be27a-146">String</span><span class="sxs-lookup"><span data-stu-id="be27a-146">String</span></span>|<span data-ttu-id="be27a-147">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="be27a-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="be27a-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be27a-148">Read-only.</span></span> <span data-ttu-id="be27a-149">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="be27a-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="be27a-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="be27a-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="be27a-151">Boolean</span></span>|<span data-ttu-id="be27a-152">Имеет true, если IP-адреса, которые не сопойдутся со странаю или регионом, должны быть включены в именоваемом расположении.</span><span class="sxs-lookup"><span data-stu-id="be27a-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="be27a-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be27a-153">modifiedDateTime</span></span>|<span data-ttu-id="be27a-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be27a-154">DateTimeOffset</span></span>|<span data-ttu-id="be27a-155">Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="be27a-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="be27a-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="be27a-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="be27a-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be27a-157">Read-only.</span></span> <span data-ttu-id="be27a-158">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="be27a-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="be27a-159">Связи</span><span class="sxs-lookup"><span data-stu-id="be27a-159">Relationships</span></span>

<span data-ttu-id="be27a-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="be27a-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be27a-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="be27a-161">JSON representation</span></span>

<span data-ttu-id="be27a-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be27a-162">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "includeUnknownCountriesAndRegions": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "countryNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


