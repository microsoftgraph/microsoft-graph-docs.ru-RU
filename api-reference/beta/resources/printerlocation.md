---
title: Тип ресурса Принтерлокатион
description: Представляет физическое и иерархическое расположение принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ea54c7b3b572413be515aa728e18ae69f6f10fc3
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896020"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="74467-103">Тип ресурса Принтерлокатион</span><span class="sxs-lookup"><span data-stu-id="74467-103">printerLocation resource type</span></span>

<span data-ttu-id="74467-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74467-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74467-105">Представляет физическое и иерархическое расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="74467-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="74467-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="74467-106">Properties</span></span>
| <span data-ttu-id="74467-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="74467-107">Property</span></span>     | <span data-ttu-id="74467-108">Тип</span><span class="sxs-lookup"><span data-stu-id="74467-108">Type</span></span>        | <span data-ttu-id="74467-109">Описание</span><span class="sxs-lookup"><span data-stu-id="74467-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74467-110">latitude</span><span class="sxs-lookup"><span data-stu-id="74467-110">latitude</span></span>|<span data-ttu-id="74467-111">Double</span><span class="sxs-lookup"><span data-stu-id="74467-111">Double</span></span>|<span data-ttu-id="74467-112">Широта, в которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="74467-113">longitude</span><span class="sxs-lookup"><span data-stu-id="74467-113">longitude</span></span>|<span data-ttu-id="74467-114">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="74467-114">Double</span></span>|<span data-ttu-id="74467-115">Долгота, на которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="74467-116">алтитудеинметерс</span><span class="sxs-lookup"><span data-stu-id="74467-116">altitudeInMeters</span></span>|<span data-ttu-id="74467-117">Int32</span><span class="sxs-lookup"><span data-stu-id="74467-117">Int32</span></span>|<span data-ttu-id="74467-118">Высота в метрах, на которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="74467-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="74467-119">streetAddress</span></span>|<span data-ttu-id="74467-120">String</span><span class="sxs-lookup"><span data-stu-id="74467-120">String</span></span>|<span data-ttu-id="74467-121">Почтовый адрес, где расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="74467-122">подединица</span><span class="sxs-lookup"><span data-stu-id="74467-122">subUnit</span></span>|<span data-ttu-id="74467-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74467-123">String collection</span></span>|<span data-ttu-id="74467-124">Иерархия подразделений, в которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="74467-125">Элементы должны находиться в иерархическом порядке.</span><span class="sxs-lookup"><span data-stu-id="74467-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="74467-126">Например, если Кампус делится на несколько разделов, иерархия может выглядеть следующим образом:`["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="74467-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>
|<span data-ttu-id="74467-127">city</span><span class="sxs-lookup"><span data-stu-id="74467-127">city</span></span>|<span data-ttu-id="74467-128">String</span><span class="sxs-lookup"><span data-stu-id="74467-128">String</span></span>|<span data-ttu-id="74467-129">Город, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-129">The city that the printer is located in.</span></span>
|<span data-ttu-id="74467-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="74467-130">postalCode</span></span>|<span data-ttu-id="74467-131">String</span><span class="sxs-lookup"><span data-stu-id="74467-131">String</span></span>|<span data-ttu-id="74467-132">Почтовый индекс, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-132">The postal code that the printer is located in.</span></span>
|<span data-ttu-id="74467-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="74467-133">countryOrRegion</span></span>|<span data-ttu-id="74467-134">String</span><span class="sxs-lookup"><span data-stu-id="74467-134">String</span></span>|<span data-ttu-id="74467-135">Страна или регион, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="74467-136">site</span><span class="sxs-lookup"><span data-stu-id="74467-136">site</span></span>|<span data-ttu-id="74467-137">String</span><span class="sxs-lookup"><span data-stu-id="74467-137">String</span></span>|<span data-ttu-id="74467-138">Сайт, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-138">The site that the printer is located in.</span></span>
|<span data-ttu-id="74467-139">создания</span><span class="sxs-lookup"><span data-stu-id="74467-139">building</span></span>|<span data-ttu-id="74467-140">String</span><span class="sxs-lookup"><span data-stu-id="74467-140">String</span></span>|<span data-ttu-id="74467-141">Построение, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-141">The building that the printer is located in.</span></span>
|<span data-ttu-id="74467-142">флурнумбер</span><span class="sxs-lookup"><span data-stu-id="74467-142">floorNumber</span></span>|<span data-ttu-id="74467-143">Int32</span><span class="sxs-lookup"><span data-stu-id="74467-143">Int32</span></span>|<span data-ttu-id="74467-144">Номер этажа, на котором расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-144">The floor number that the printer is located on.</span></span>
|<span data-ttu-id="74467-145">флурдескриптион</span><span class="sxs-lookup"><span data-stu-id="74467-145">floorDescription</span></span>|<span data-ttu-id="74467-146">String</span><span class="sxs-lookup"><span data-stu-id="74467-146">String</span></span>|<span data-ttu-id="74467-147">Описание основания, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-147">The description of the floor that the printer is located on.</span></span>
|<span data-ttu-id="74467-148">румнумбер</span><span class="sxs-lookup"><span data-stu-id="74467-148">roomNumber</span></span>|<span data-ttu-id="74467-149">Int32</span><span class="sxs-lookup"><span data-stu-id="74467-149">Int32</span></span>|<span data-ttu-id="74467-150">Номер комнаты, в которой находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-150">The room number that the printer is located in.</span></span>
|<span data-ttu-id="74467-151">румдескриптион</span><span class="sxs-lookup"><span data-stu-id="74467-151">roomDescription</span></span>|<span data-ttu-id="74467-152">Int32</span><span class="sxs-lookup"><span data-stu-id="74467-152">Int32</span></span>|<span data-ttu-id="74467-153">Описание комнаты, в которой находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-153">The description of the room that the printer is located in.</span></span>
|<span data-ttu-id="74467-154">organization;</span><span class="sxs-lookup"><span data-stu-id="74467-154">organization</span></span>|<span data-ttu-id="74467-155">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74467-155">String collection</span></span>|<span data-ttu-id="74467-156">Организационная иерархия, к которой относится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-156">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="74467-157">Элементы должны находиться в иерархическом порядке.</span><span class="sxs-lookup"><span data-stu-id="74467-157">The elements should be in hierarchical order.</span></span>
|<span data-ttu-id="74467-158">подразделение</span><span class="sxs-lookup"><span data-stu-id="74467-158">subdivision</span></span>|<span data-ttu-id="74467-159">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74467-159">String collection</span></span>|<span data-ttu-id="74467-160">Подразделение, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-160">The subdivision that the printer is located in.</span></span> <span data-ttu-id="74467-161">Элементы должны находиться в иерархическом порядке.</span><span class="sxs-lookup"><span data-stu-id="74467-161">The elements should be in hierarchical order.</span></span>
|<span data-ttu-id="74467-162">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="74467-162">stateOrProvince</span></span>|<span data-ttu-id="74467-163">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="74467-163">String collection</span></span>|<span data-ttu-id="74467-164">Область или край, в котором находится принтер.</span><span class="sxs-lookup"><span data-stu-id="74467-164">The state or province that the printer is located in.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74467-165">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74467-165">JSON representation</span></span>

<span data-ttu-id="74467-166">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74467-166">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerLocation"
}-->

```json
{
    "latitude": 80.1,
    "longitude": -170.1,
    "altitudeInMeters": 123456,
    "streetAddress": "String",
    "subUnit": ["String"],
    "city": "String",
    "postalCode": "String",
    "countryOrRegion": "String",
    "site": "String",
    "building": "String",
    "floorNumber": 123456,
    "floorDescription": "String",
    "roomNumber": 123456,
    "roomDescription": "String",
    "organization": ["String"],
    "subdivision": ["String"],
    "stateOrProvince": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->