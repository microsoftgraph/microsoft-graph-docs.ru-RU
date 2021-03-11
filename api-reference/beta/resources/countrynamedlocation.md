---
title: тип ресурса countryNamedLocation
description: Представляет расположение Azure Active Directory с именем, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f6a986907ee82ea3f40c7b294cf21bf4dcc191a4
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721658"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="180e0-104">тип ресурса countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="180e0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="180e0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="180e0-106">Представляет расположение Azure Active Directory с именем, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="180e0-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="180e0-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="180e0-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="180e0-108">Наследует от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="180e0-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="180e0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="180e0-109">Methods</span></span>

| <span data-ttu-id="180e0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="180e0-110">Method</span></span>       | <span data-ttu-id="180e0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="180e0-111">Return Type</span></span> | <span data-ttu-id="180e0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="180e0-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="180e0-113">Список countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="180e0-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="180e0-114">[коллекция countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="180e0-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="180e0-115">Получите все **объекты countryNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="180e0-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="180e0-116">Создание countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="180e0-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="180e0-118">Создание нового **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="180e0-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="180e0-119">Get countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="180e0-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="180e0-121">Ознакомьтесь с свойствами и отношениями **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="180e0-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="180e0-122">Обновление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="180e0-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="180e0-124">Обновление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="180e0-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="180e0-125">Удаление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="180e0-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="180e0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="180e0-126">None</span></span> | <span data-ttu-id="180e0-127">Удаление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="180e0-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="180e0-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="180e0-128">Properties</span></span>

| <span data-ttu-id="180e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="180e0-129">Property</span></span>     | <span data-ttu-id="180e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="180e0-130">Type</span></span>        | <span data-ttu-id="180e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="180e0-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="180e0-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="180e0-132">countriesAndRegions</span></span>|<span data-ttu-id="180e0-133">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="180e0-133">String collection</span></span>|<span data-ttu-id="180e0-134">Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="180e0-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="180e0-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="180e0-135">createdDateTime</span></span>|<span data-ttu-id="180e0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180e0-136">DateTimeOffset</span></span>|<span data-ttu-id="180e0-137">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="180e0-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="180e0-138">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="180e0-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="180e0-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180e0-139">Read-only.</span></span> <span data-ttu-id="180e0-140">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="180e0-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="180e0-141">displayName</span><span class="sxs-lookup"><span data-stu-id="180e0-141">displayName</span></span>|<span data-ttu-id="180e0-142">String</span><span class="sxs-lookup"><span data-stu-id="180e0-142">String</span></span>|<span data-ttu-id="180e0-143">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="180e0-143">Human-readable name of the location.</span></span> <span data-ttu-id="180e0-144">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="180e0-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="180e0-145">id</span><span class="sxs-lookup"><span data-stu-id="180e0-145">id</span></span>|<span data-ttu-id="180e0-146">String</span><span class="sxs-lookup"><span data-stu-id="180e0-146">String</span></span>|<span data-ttu-id="180e0-147">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="180e0-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="180e0-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180e0-148">Read-only.</span></span> <span data-ttu-id="180e0-149">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="180e0-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="180e0-150">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="180e0-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="180e0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="180e0-151">Boolean</span></span>|<span data-ttu-id="180e0-152">Верно, если IP-адреса, которые не относятся к стране или региону, должны быть включены в именоваемом расположении.</span><span class="sxs-lookup"><span data-stu-id="180e0-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="180e0-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="180e0-153">modifiedDateTime</span></span>|<span data-ttu-id="180e0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="180e0-154">DateTimeOffset</span></span>|<span data-ttu-id="180e0-155">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="180e0-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="180e0-156">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="180e0-156">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="180e0-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="180e0-157">Read-only.</span></span> <span data-ttu-id="180e0-158">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="180e0-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="180e0-159">Связи</span><span class="sxs-lookup"><span data-stu-id="180e0-159">Relationships</span></span>

<span data-ttu-id="180e0-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="180e0-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="180e0-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="180e0-161">JSON representation</span></span>

<span data-ttu-id="180e0-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="180e0-162">The following is a JSON representation of the resource.</span></span>

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


