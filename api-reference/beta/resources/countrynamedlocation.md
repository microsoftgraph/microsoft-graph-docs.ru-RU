---
title: Тип ресурса Каунтринамедлокатион
description: Представляет имя расположения Azure Active Directory, определенное странами и регионами. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f0683c967d56303cb092b7300e50312ab329ea4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458035"
---
# <a name="countrynamedlocation-resource-type"></a><span data-ttu-id="36acd-104">Тип ресурса Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-104">countryNamedLocation resource type</span></span>

<span data-ttu-id="36acd-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36acd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36acd-106">Представляет имя расположения Azure Active Directory, определенное странами и регионами.</span><span class="sxs-lookup"><span data-stu-id="36acd-106">Represents an Azure Active Directory named location defined by countries and regions.</span></span> <span data-ttu-id="36acd-107">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="36acd-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="36acd-108">Наследуется от [намедлокатион](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="36acd-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="36acd-109">Методы</span><span class="sxs-lookup"><span data-stu-id="36acd-109">Methods</span></span>

| <span data-ttu-id="36acd-110">Метод</span><span class="sxs-lookup"><span data-stu-id="36acd-110">Method</span></span>       | <span data-ttu-id="36acd-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="36acd-111">Return Type</span></span> | <span data-ttu-id="36acd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="36acd-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="36acd-113">Список Каунтринамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="36acd-113">List countryNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="36acd-114">Коллекция [каунтринамедлокатион](countryNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="36acd-114">[countryNamedLocation](countryNamedLocation.md) collection</span></span> | <span data-ttu-id="36acd-115">Получение всех объектов **каунтринамедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="36acd-115">Get all the **countryNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="36acd-116">Создание Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-116">Create countryNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="36acd-117">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-117">countryNamedLocation</span></span>](countryNamedLocation.md) | <span data-ttu-id="36acd-118">Создание нового объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="36acd-118">Create a new **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="36acd-119">Получение Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-119">Get countryNamedLocation</span></span>](../api/countrynamedlocation-get.md) | [<span data-ttu-id="36acd-120">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-120">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="36acd-121">Чтение свойств и связей объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="36acd-121">Read the properties and relationships of a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="36acd-122">Обновление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-122">Update countryNamedLocation</span></span>](../api/countrynamedlocation-update.md) | [<span data-ttu-id="36acd-123">каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-123">countryNamedLocation</span></span>](countrynamedlocation.md) | <span data-ttu-id="36acd-124">Обновление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="36acd-124">Update a **countryNamedLocation** object.</span></span> |
| [<span data-ttu-id="36acd-125">Удаление Каунтринамедлокатион</span><span class="sxs-lookup"><span data-stu-id="36acd-125">Delete countryNamedLocation</span></span>](../api/countrynamedlocation-delete.md) | <span data-ttu-id="36acd-126">Нет</span><span class="sxs-lookup"><span data-stu-id="36acd-126">None</span></span> | <span data-ttu-id="36acd-127">Удаление объекта **каунтринамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="36acd-127">Delete a **countryNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="36acd-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="36acd-128">Properties</span></span>

| <span data-ttu-id="36acd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="36acd-129">Property</span></span>     | <span data-ttu-id="36acd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="36acd-130">Type</span></span>        | <span data-ttu-id="36acd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="36acd-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36acd-132">каунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="36acd-132">countriesAndRegions</span></span>|<span data-ttu-id="36acd-133">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="36acd-133">String collection</span></span>|<span data-ttu-id="36acd-134">Список стран и/или регионов в формате из двух букв, заданных в стандарте ISO 3166-2.</span><span class="sxs-lookup"><span data-stu-id="36acd-134">List of countries and/or regions in two-letter format specified by ISO 3166-2.</span></span>|
|<span data-ttu-id="36acd-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36acd-135">createdDateTime</span></span>|<span data-ttu-id="36acd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36acd-136">DateTimeOffset</span></span>|<span data-ttu-id="36acd-137">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="36acd-137">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="36acd-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="36acd-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="36acd-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36acd-139">Read-only.</span></span> <span data-ttu-id="36acd-140">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="36acd-140">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="36acd-141">displayName</span><span class="sxs-lookup"><span data-stu-id="36acd-141">displayName</span></span>|<span data-ttu-id="36acd-142">Строка</span><span class="sxs-lookup"><span data-stu-id="36acd-142">String</span></span>|<span data-ttu-id="36acd-143">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="36acd-143">Human-readable name of the location.</span></span> <span data-ttu-id="36acd-144">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="36acd-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="36acd-145">id</span><span class="sxs-lookup"><span data-stu-id="36acd-145">id</span></span>|<span data-ttu-id="36acd-146">String</span><span class="sxs-lookup"><span data-stu-id="36acd-146">String</span></span>|<span data-ttu-id="36acd-147">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="36acd-147">Identifier of a namedLocation object.</span></span> <span data-ttu-id="36acd-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36acd-148">Read-only.</span></span> <span data-ttu-id="36acd-149">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="36acd-149">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="36acd-150">инклудеункновнкаунтриесандрегионс</span><span class="sxs-lookup"><span data-stu-id="36acd-150">includeUnknownCountriesAndRegions</span></span>|<span data-ttu-id="36acd-151">Логическое</span><span class="sxs-lookup"><span data-stu-id="36acd-151">Boolean</span></span>|<span data-ttu-id="36acd-152">Значение true, если IP-адреса, которые не сопоставляются со страной или регионом, должны быть включены в именованное расположение.</span><span class="sxs-lookup"><span data-stu-id="36acd-152">True if IP addresses that don't map to a country or region should be included in the named location.</span></span>|
|<span data-ttu-id="36acd-153">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36acd-153">modifiedDateTime</span></span>|<span data-ttu-id="36acd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36acd-154">DateTimeOffset</span></span>|<span data-ttu-id="36acd-155">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="36acd-155">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="36acd-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="36acd-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="36acd-157">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="36acd-157">Read-only.</span></span> <span data-ttu-id="36acd-158">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="36acd-158">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="36acd-159">Связи</span><span class="sxs-lookup"><span data-stu-id="36acd-159">Relationships</span></span>

<span data-ttu-id="36acd-160">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36acd-160">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36acd-161">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36acd-161">JSON representation</span></span>

<span data-ttu-id="36acd-162">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36acd-162">The following is a JSON representation of the resource.</span></span>

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
