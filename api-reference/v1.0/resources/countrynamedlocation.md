---
title: тип ресурса countryNamedLocation
description: Представляет расположение Azure Active Directory, определенное странами и регионами. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 531942e5026e2fc3d4d9ed3311d9130275d5a853
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443167"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="525ff-104">тип ресурса countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="525ff-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="525ff-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="525ff-106">Представляет расположение Azure Active Directory, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="525ff-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="525ff-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="525ff-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="525ff-108">Наследует от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="525ff-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="525ff-109">Методы</span><span class="sxs-lookup"><span data-stu-id="525ff-109">Methods</span></span>

| <span data-ttu-id="525ff-110">Метод</span><span class="sxs-lookup"><span data-stu-id="525ff-110">Method</span></span>       | <span data-ttu-id="525ff-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="525ff-111">Return Type</span></span> | <span data-ttu-id="525ff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="525ff-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="525ff-113">Список countryNamedLocations</span><span class="sxs-lookup"><span data-stu-id="525ff-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="525ff-114">[коллекция countryNamedLocation](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="525ff-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="525ff-115">Получите все **объекты countryNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="525ff-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="525ff-116">Создание countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="525ff-117">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="525ff-118">Создание нового **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="525ff-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="525ff-119">Get countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="525ff-120">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="525ff-121">Ознакомьтесь с свойствами и отношениями **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="525ff-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="525ff-122">Обновление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="525ff-123">countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="525ff-124">Обновление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="525ff-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="525ff-125">Удаление countryNamedLocation</span><span class="sxs-lookup"><span data-stu-id="525ff-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="525ff-126">Нет</span><span class="sxs-lookup"><span data-stu-id="525ff-126">None</span></span> | <span data-ttu-id="525ff-127">Удаление **объекта countryNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="525ff-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="525ff-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="525ff-128">Properties</span></span>

| <span data-ttu-id="525ff-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="525ff-129">Property</span></span>     | <span data-ttu-id="525ff-130">Тип</span><span class="sxs-lookup"><span data-stu-id="525ff-130">Type</span></span>        | <span data-ttu-id="525ff-131">Описание</span><span class="sxs-lookup"><span data-stu-id="525ff-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="525ff-132">countriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="525ff-132">countriesAndRegions</span></span>|<span data-ttu-id="525ff-133">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="525ff-133">String collection</span></span>|<span data-ttu-id="525ff-134">Список стран и/или регионов в формате двух букв, заданный ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="525ff-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="525ff-135">countryLookupMethod</span><span class="sxs-lookup"><span data-stu-id="525ff-135">countryLookupMethod</span></span>|<span data-ttu-id="525ff-136">countryLookupMethodType</span><span class="sxs-lookup"><span data-stu-id="525ff-136">countryLookupMethodType</span></span>|<span data-ttu-id="525ff-137">Определяет, какой метод используется для определения страны, в которой находится пользователь.</span><span class="sxs-lookup"><span data-stu-id="525ff-137">Determines what method is used to decide which country the user is located in.</span></span> <span data-ttu-id="525ff-138">Возможные значения: `clientIpAddress` и `authenticatorAppGps`.</span><span class="sxs-lookup"><span data-stu-id="525ff-138">Possible values are `clientIpAddress` and `authenticatorAppGps`.</span></span>|
|<span data-ttu-id="525ff-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="525ff-139">createdDateTime</span></span>|<span data-ttu-id="525ff-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525ff-140">DateTimeOffset</span></span>|<span data-ttu-id="525ff-141">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="525ff-141">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="525ff-142">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="525ff-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="525ff-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="525ff-143">Read-only.</span></span> <span data-ttu-id="525ff-144">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="525ff-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="525ff-145">displayName</span><span class="sxs-lookup"><span data-stu-id="525ff-145">displayName</span></span>|<span data-ttu-id="525ff-146">String</span><span class="sxs-lookup"><span data-stu-id="525ff-146">String</span></span>|<span data-ttu-id="525ff-147">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="525ff-147">Human-readable name of the location.</span></span> <span data-ttu-id="525ff-148">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="525ff-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="525ff-149">id</span><span class="sxs-lookup"><span data-stu-id="525ff-149">id</span></span>|<span data-ttu-id="525ff-150">String</span><span class="sxs-lookup"><span data-stu-id="525ff-150">String</span></span>|<span data-ttu-id="525ff-151">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="525ff-151">Identifier of a namedLocation object.</span></span> <span data-ttu-id="525ff-152">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="525ff-152">Read-only.</span></span> <span data-ttu-id="525ff-153">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="525ff-153">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="525ff-154">includeUnknownCountriesAndRegions</span><span class="sxs-lookup"><span data-stu-id="525ff-154">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="525ff-155">Логический</span><span class="sxs-lookup"><span data-stu-id="525ff-155">Boolean</span></span>|<span data-ttu-id="525ff-156">Верно, если IP-адреса, которые не относятся к стране или региону, должны быть включены в именоваемом расположении.</span><span class="sxs-lookup"><span data-stu-id="525ff-156">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="525ff-157">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="525ff-157">modifiedDateTime</span></span>|<span data-ttu-id="525ff-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="525ff-158">DateTimeOffset</span></span>|<span data-ttu-id="525ff-159">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="525ff-159">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="525ff-160">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="525ff-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="525ff-161">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="525ff-161">Read-only.</span></span> <span data-ttu-id="525ff-162">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="525ff-162">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="525ff-163">Связи</span><span class="sxs-lookup"><span data-stu-id="525ff-163">Relationships</span></span>

<span data-ttu-id="525ff-164">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="525ff-164">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="525ff-165">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="525ff-165">JSON representation</span></span>

<span data-ttu-id="525ff-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="525ff-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation"
}-->

```json
{
  "countriesAndRegions": ["String"],
  "countryLookupMethod": "String",
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
