---
title: тип ресурса countryNamedLocation
description: Представляет расположение Azure Active Directory с именем, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: dcd31478a82e6e132264b31f070d5bad317edae7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444257"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="e69e3-104">тип ресурса countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="e69e3-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e69e3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e69e3-106">Представляет расположение Azure Active Directory с именем, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="e69e3-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="e69e3-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="e69e3-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="e69e3-108">Наследует от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="e69e3-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e69e3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e69e3-109">Methods</span></span>

| <span data-ttu-id="e69e3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e69e3-110">Method</span></span>       | <span data-ttu-id="e69e3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e69e3-111">Return Type</span></span> | <span data-ttu-id="e69e3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e69e3-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e69e3-113">Список countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="e69e3-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="e69e3-114">[коллекция countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="e69e3-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="e69e3-115">Получите все **объекты countryNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="e69e3-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="e69e3-116">Создание countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="e69e3-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="e69e3-118">Создание нового **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e69e3-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="e69e3-119">Get countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="e69e3-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="e69e3-121">Ознакомьтесь с свойствами и отношениями **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e69e3-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="e69e3-122">Обновление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="e69e3-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="e69e3-124">Обновление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e69e3-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="e69e3-125">Удаление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="e69e3-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="e69e3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="e69e3-126">None</span></span> | <span data-ttu-id="e69e3-127">Удаление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="e69e3-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e69e3-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="e69e3-128">Properties</span></span>

| <span data-ttu-id="e69e3-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e69e3-129">Property</span></span>     | <span data-ttu-id="e69e3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e69e3-130">Type</span></span>        | <span data-ttu-id="e69e3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e69e3-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e69e3-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="e69e3-132">countriesAndRegions</span></span>|<span data-ttu-id="e69e3-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="e69e3-133">String collection</span></span>|<span data-ttu-id="e69e3-134">Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="e69e3-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="e69e3-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e69e3-135">createdDateTime</span></span>|<span data-ttu-id="e69e3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e69e3-136">DateTimeOffset</span></span>|<span data-ttu-id="e69e3-137">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="e69e3-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e69e3-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e69e3-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e69e3-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e69e3-139">Read-only.</span></span> <span data-ttu-id="e69e3-140">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="e69e3-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="e69e3-141">displayName</span><span class="sxs-lookup"><span data-stu-id="e69e3-141">displayName</span></span>|<span data-ttu-id="e69e3-142">String</span><span class="sxs-lookup"><span data-stu-id="e69e3-142">String</span></span>|<span data-ttu-id="e69e3-143">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="e69e3-143">Human-readable name of the location.</span></span> <span data-ttu-id="e69e3-144">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="e69e3-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="e69e3-145">id</span><span class="sxs-lookup"><span data-stu-id="e69e3-145">id</span></span>|<span data-ttu-id="e69e3-146">String</span><span class="sxs-lookup"><span data-stu-id="e69e3-146">String</span></span>|<span data-ttu-id="e69e3-147">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="e69e3-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="e69e3-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e69e3-148">Read-only.</span></span> <span data-ttu-id="e69e3-149">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="e69e3-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="e69e3-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="e69e3-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="e69e3-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="e69e3-151">Boolean</span></span>|<span data-ttu-id="e69e3-152">Верно, если IP-адреса, которые не относятся к стране или региону, должны быть включены в именоваемом расположении.</span><span class="sxs-lookup"><span data-stu-id="e69e3-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="e69e3-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e69e3-153">modifiedDateTime</span></span>|<span data-ttu-id="e69e3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e69e3-154">DateTimeOffset</span></span>|<span data-ttu-id="e69e3-155">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="e69e3-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e69e3-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e69e3-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="e69e3-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e69e3-157">Read-only.</span></span> <span data-ttu-id="e69e3-158">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="e69e3-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e69e3-159">Связи</span><span class="sxs-lookup"><span data-stu-id="e69e3-159">Relationships</span></span>

<span data-ttu-id="e69e3-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e69e3-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e69e3-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e69e3-161">JSON representation</span></span>

<span data-ttu-id="e69e3-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e69e3-162">The following is a JSON representation of the resource.</span></span>

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


