---
title: Тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bfb082571ab1c5ddf2b46a06c6e66b9e31e47309
ms.sourcegitcommit: 7902607a1e5a030d46e907d08e16644a47a47006
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/12/2020
ms.locfileid: "49664060"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="ce269-103">Тип ресурса printerLocation</span><span class="sxs-lookup"><span data-stu-id="ce269-103">printerLocation resource type</span></span>

<span data-ttu-id="ce269-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce269-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce269-105">Представляет физическое и иерархическое расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="ce269-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="ce269-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce269-106">Properties</span></span>
| <span data-ttu-id="ce269-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce269-107">Property</span></span>     | <span data-ttu-id="ce269-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce269-108">Type</span></span>        | <span data-ttu-id="ce269-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce269-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ce269-110">latitude</span><span class="sxs-lookup"><span data-stu-id="ce269-110">latitude</span></span>|<span data-ttu-id="ce269-111">Double</span><span class="sxs-lookup"><span data-stu-id="ce269-111">Double</span></span>|<span data-ttu-id="ce269-112">Широта, в которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="ce269-113">longitude</span><span class="sxs-lookup"><span data-stu-id="ce269-113">longitude</span></span>|<span data-ttu-id="ce269-114">Double</span><span class="sxs-lookup"><span data-stu-id="ce269-114">Double</span></span>|<span data-ttu-id="ce269-115">Долгота, в которую находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="ce269-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="ce269-116">altitudeInMeters</span></span>|<span data-ttu-id="ce269-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ce269-117">Int32</span></span>|<span data-ttu-id="ce269-118">Высота в метрах, в которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="ce269-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="ce269-119">streetAddress</span></span>|<span data-ttu-id="ce269-120">String</span><span class="sxs-lookup"><span data-stu-id="ce269-120">String</span></span>|<span data-ttu-id="ce269-121">Адрес улицы, где расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="ce269-122">subUnit</span><span class="sxs-lookup"><span data-stu-id="ce269-122">subUnit</span></span>|<span data-ttu-id="ce269-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce269-123">String collection</span></span>|<span data-ttu-id="ce269-124">Иерархия, в которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="ce269-125">Элементы должны быть в иерархическому порядке.</span><span class="sxs-lookup"><span data-stu-id="ce269-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="ce269-126">Например, если территории разделены на разные разделы, иерархия может выглядеть так: `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="ce269-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="ce269-127">city</span><span class="sxs-lookup"><span data-stu-id="ce269-127">city</span></span>|<span data-ttu-id="ce269-128">String</span><span class="sxs-lookup"><span data-stu-id="ce269-128">String</span></span>|<span data-ttu-id="ce269-129">Город, в который находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="ce269-130">postalCode</span></span>|<span data-ttu-id="ce269-131">String</span><span class="sxs-lookup"><span data-stu-id="ce269-131">String</span></span>|<span data-ttu-id="ce269-132">Почтовый индекс, в который находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ce269-133">countryOrRegion</span></span>|<span data-ttu-id="ce269-134">String</span><span class="sxs-lookup"><span data-stu-id="ce269-134">String</span></span>|<span data-ttu-id="ce269-135">Страна или регион, где находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-136">site</span><span class="sxs-lookup"><span data-stu-id="ce269-136">site</span></span>|<span data-ttu-id="ce269-137">String</span><span class="sxs-lookup"><span data-stu-id="ce269-137">String</span></span>|<span data-ttu-id="ce269-138">Сайт, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-139">building</span><span class="sxs-lookup"><span data-stu-id="ce269-139">building</span></span>|<span data-ttu-id="ce269-140">String</span><span class="sxs-lookup"><span data-stu-id="ce269-140">String</span></span>|<span data-ttu-id="ce269-141">Здание, в которое находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-142">floor</span><span class="sxs-lookup"><span data-stu-id="ce269-142">floor</span></span>|<span data-ttu-id="ce269-143">String</span><span class="sxs-lookup"><span data-stu-id="ce269-143">String</span></span>|<span data-ttu-id="ce269-144">Пол, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-144">The floor that the printer is located on.</span></span> <span data-ttu-id="ce269-145">В настоящее время поддерживаются только числимые значения.</span><span class="sxs-lookup"><span data-stu-id="ce269-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="ce269-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="ce269-146">floorDescription</span></span>|<span data-ttu-id="ce269-147">String</span><span class="sxs-lookup"><span data-stu-id="ce269-147">String</span></span>|<span data-ttu-id="ce269-148">Описание этажа, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="ce269-149">roomName</span><span class="sxs-lookup"><span data-stu-id="ce269-149">roomName</span></span>|<span data-ttu-id="ce269-150">String</span><span class="sxs-lookup"><span data-stu-id="ce269-150">String</span></span>|<span data-ttu-id="ce269-151">Комната, в которую находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-151">The room that the printer is located in.</span></span> <span data-ttu-id="ce269-152">В настоящее время поддерживаются только числимые значения.</span><span class="sxs-lookup"><span data-stu-id="ce269-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="ce269-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="ce269-153">roomDescription</span></span>|<span data-ttu-id="ce269-154">String</span><span class="sxs-lookup"><span data-stu-id="ce269-154">String</span></span>|<span data-ttu-id="ce269-155">Описание комнаты, в которую находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="ce269-156">organization;</span><span class="sxs-lookup"><span data-stu-id="ce269-156">organization</span></span>|<span data-ttu-id="ce269-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce269-157">String collection</span></span>|<span data-ttu-id="ce269-158">Организационная иерархия, к которой принадлежит принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="ce269-159">Элементы должны быть в иерархическому порядке.</span><span class="sxs-lookup"><span data-stu-id="ce269-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="ce269-160">subdivision</span><span class="sxs-lookup"><span data-stu-id="ce269-160">subdivision</span></span>|<span data-ttu-id="ce269-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="ce269-161">String collection</span></span>|<span data-ttu-id="ce269-162">Подраздел, в который находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="ce269-163">Элементы должны быть в иерархическому порядке.</span><span class="sxs-lookup"><span data-stu-id="ce269-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="ce269-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="ce269-164">stateOrProvince</span></span>|<span data-ttu-id="ce269-165">String</span><span class="sxs-lookup"><span data-stu-id="ce269-165">String</span></span>|<span data-ttu-id="ce269-166">Область или край, где находится принтер.</span><span class="sxs-lookup"><span data-stu-id="ce269-166">The state or province that the printer is located in.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ce269-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce269-167">JSON representation</span></span>

<span data-ttu-id="ce269-168">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce269-168">The following is a JSON representation of the resource.</span></span>

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
    "floor": "123456",
    "floorDescription": "String",
    "roomName": "123456",
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

