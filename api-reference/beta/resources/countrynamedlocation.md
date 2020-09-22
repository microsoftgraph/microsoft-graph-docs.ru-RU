---
title: Тип ресурса Каунтринамедлокатион
description: Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c4807abc04cb980ec452590b9643f2b07d0ce67
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016711"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="3ce2e-104">Тип ресурса Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="3ce2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ce2e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ce2e-106">Представляет имя расположения Azure Active Directory, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="3ce2e-107">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="3ce2e-108">Наследуется от [намедлокатион](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3ce2e-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3ce2e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3ce2e-109">Methods</span></span>

| <span data-ttu-id="3ce2e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3ce2e-110">Method</span></span>       | <span data-ttu-id="3ce2e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ce2e-111">Return Type</span></span> | <span data-ttu-id="3ce2e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce2e-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3ce2e-113">Список Каунтринамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="3ce2e-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="3ce2e-114">Коллекция [каунтринамедлокатион](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3ce2e-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="3ce2e-115">Получение всех объектов **каунтринамедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="3ce2e-116">Создание Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="3ce2e-117">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="3ce2e-118">Создание нового объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3ce2e-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="3ce2e-119">Получение Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="3ce2e-120">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="3ce2e-121">Чтение свойств и связей объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3ce2e-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="3ce2e-122">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="3ce2e-123">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="3ce2e-124">Обновление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3ce2e-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="3ce2e-125">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3ce2e-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="3ce2e-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3ce2e-126">None</span></span> | <span data-ttu-id="3ce2e-127">Удаление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3ce2e-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3ce2e-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ce2e-128">Properties</span></span>

| <span data-ttu-id="3ce2e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ce2e-129">Property</span></span>     | <span data-ttu-id="3ce2e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3ce2e-130">Type</span></span>        | <span data-ttu-id="3ce2e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3ce2e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ce2e-132">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="3ce2e-132">countriesAndRegions</span></span>|<span data-ttu-id="3ce2e-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3ce2e-133">String collection</span></span>|<span data-ttu-id="3ce2e-134">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="3ce2e-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce2e-135">createdDateTime</span></span>|<span data-ttu-id="3ce2e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce2e-136">DateTimeOffset</span></span>|<span data-ttu-id="3ce2e-137">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ce2e-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3ce2e-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-139">Read-only.</span></span> <span data-ttu-id="3ce2e-140">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3ce2e-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3ce2e-141">displayName</span><span class="sxs-lookup"><span data-stu-id="3ce2e-141">displayName</span></span>|<span data-ttu-id="3ce2e-142">String</span><span class="sxs-lookup"><span data-stu-id="3ce2e-142">String</span></span>|<span data-ttu-id="3ce2e-143">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-143">Human-readable name of the location.</span></span> <span data-ttu-id="3ce2e-144">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3ce2e-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3ce2e-145">id</span><span class="sxs-lookup"><span data-stu-id="3ce2e-145">id</span></span>|<span data-ttu-id="3ce2e-146">String</span><span class="sxs-lookup"><span data-stu-id="3ce2e-146">String</span></span>|<span data-ttu-id="3ce2e-147">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="3ce2e-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-148">Read-only.</span></span> <span data-ttu-id="3ce2e-149">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3ce2e-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3ce2e-150">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="3ce2e-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="3ce2e-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ce2e-151">Boolean</span></span>|<span data-ttu-id="3ce2e-152">Значение true, если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="3ce2e-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3ce2e-153">modifiedDateTime</span></span>|<span data-ttu-id="3ce2e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ce2e-154">DateTimeOffset</span></span>|<span data-ttu-id="3ce2e-155">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ce2e-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3ce2e-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-157">Read-only.</span></span> <span data-ttu-id="3ce2e-158">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3ce2e-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ce2e-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ce2e-159">Relationships</span></span>

<span data-ttu-id="3ce2e-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ce2e-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3ce2e-161">JSON representation</span></span>

<span data-ttu-id="3ce2e-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ce2e-162">The following is a JSON representation of the resource.</span></span>

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


