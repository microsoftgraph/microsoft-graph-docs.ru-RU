---
title: Тип ресурса Каунтринамедлокатион
description: Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cb413aab72abe401152b67b985f023350f80f30
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653673"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="4d51c-104">Тип ресурса Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-104">countryNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d51c-105">Представляет имя расположения Azure Active Directory, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="4d51c-105">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="4d51c-106">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="4d51c-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="4d51c-107">Наследуется от [намедлокатион](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="4d51c-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="4d51c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="4d51c-108">Methods</span></span>

| <span data-ttu-id="4d51c-109">Метод</span><span class="sxs-lookup"><span data-stu-id="4d51c-109">Method</span></span>       | <span data-ttu-id="4d51c-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4d51c-110">Return Type</span></span> | <span data-ttu-id="4d51c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4d51c-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4d51c-112">Список Каунтринамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="4d51c-112">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="4d51c-113">Коллекция [каунтринамедлокатион](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="4d51c-113">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="4d51c-114">Получение всех объектов **каунтринамедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="4d51c-114">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="4d51c-115">Создание Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-115">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="4d51c-116">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-116">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="4d51c-117">Создание нового объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="4d51c-117">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="4d51c-118">Получение Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-118">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="4d51c-119">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-119">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="4d51c-120">Чтение свойств и связей объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="4d51c-120">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="4d51c-121">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-121">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="4d51c-122">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-122">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="4d51c-123">Обновление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="4d51c-123">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="4d51c-124">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="4d51c-124">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="4d51c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="4d51c-125">None</span></span> | <span data-ttu-id="4d51c-126">Удаление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="4d51c-126">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4d51c-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="4d51c-127">Properties</span></span>

| <span data-ttu-id="4d51c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4d51c-128">Property</span></span>     | <span data-ttu-id="4d51c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4d51c-129">Type</span></span>        | <span data-ttu-id="4d51c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4d51c-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d51c-131">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="4d51c-131">countriesAndRegions</span></span>|<span data-ttu-id="4d51c-132">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4d51c-132">String collection</span></span>|<span data-ttu-id="4d51c-133">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="4d51c-133">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="4d51c-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4d51c-134">createdDateTime</span></span>|<span data-ttu-id="4d51c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d51c-135">DateTimeOffset</span></span>|<span data-ttu-id="4d51c-136">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4d51c-136">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d51c-137">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4d51c-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4d51c-138">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d51c-138">Read-only.</span></span> <span data-ttu-id="4d51c-139">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="4d51c-139">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="4d51c-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4d51c-140">displayName</span></span>|<span data-ttu-id="4d51c-141">Строка</span><span class="sxs-lookup"><span data-stu-id="4d51c-141">String</span></span>|<span data-ttu-id="4d51c-142">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="4d51c-142">Human-readable name of the location.</span></span> <span data-ttu-id="4d51c-143">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="4d51c-143">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="4d51c-144">id</span><span class="sxs-lookup"><span data-stu-id="4d51c-144">id</span></span>|<span data-ttu-id="4d51c-145">String</span><span class="sxs-lookup"><span data-stu-id="4d51c-145">String</span></span>|<span data-ttu-id="4d51c-146">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="4d51c-146">Identifier of a namedLocation object.</span></span> <span data-ttu-id="4d51c-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d51c-147">Read-only.</span></span> <span data-ttu-id="4d51c-148">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="4d51c-148">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="4d51c-149">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="4d51c-149">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="4d51c-150">Логический</span><span class="sxs-lookup"><span data-stu-id="4d51c-150">Boolean</span></span>|<span data-ttu-id="4d51c-151">Значение true, если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="4d51c-151">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="4d51c-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d51c-152">modifiedDateTime</span></span>|<span data-ttu-id="4d51c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d51c-153">DateTimeOffset</span></span>|<span data-ttu-id="4d51c-154">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4d51c-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d51c-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="4d51c-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="4d51c-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4d51c-156">Read-only.</span></span> <span data-ttu-id="4d51c-157">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="4d51c-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d51c-158">Связи</span><span class="sxs-lookup"><span data-stu-id="4d51c-158">Relationships</span></span>

<span data-ttu-id="4d51c-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d51c-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d51c-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4d51c-160">JSON representation</span></span>

<span data-ttu-id="4d51c-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4d51c-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": ""
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
