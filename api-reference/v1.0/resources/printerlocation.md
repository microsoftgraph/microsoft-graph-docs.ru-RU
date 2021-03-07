---
title: тип ресурса printerLocation
description: Представляет физическое и иерархическое расположение принтера.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: f357ab3b33182ac6ffb2f8ae705a359a0e955eed
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517367"
---
# <a name="printerlocation-resource-type"></a><span data-ttu-id="db9c7-103">тип ресурса printerLocation</span><span class="sxs-lookup"><span data-stu-id="db9c7-103">printerLocation resource type</span></span>

<span data-ttu-id="db9c7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db9c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="db9c7-105">Представляет физическое и иерархическое расположение принтера.</span><span class="sxs-lookup"><span data-stu-id="db9c7-105">Represents the physical and hierarchical location of a printer.</span></span>

## <a name="properties"></a><span data-ttu-id="db9c7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="db9c7-106">Properties</span></span>
|<span data-ttu-id="db9c7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="db9c7-107">Property</span></span>|<span data-ttu-id="db9c7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="db9c7-108">Type</span></span>|<span data-ttu-id="db9c7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="db9c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db9c7-110">latitude</span><span class="sxs-lookup"><span data-stu-id="db9c7-110">latitude</span></span>|<span data-ttu-id="db9c7-111">Double</span><span class="sxs-lookup"><span data-stu-id="db9c7-111">Double</span></span>|<span data-ttu-id="db9c7-112">Широта, на которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-112">The latitude that the printer is located at.</span></span>|
|<span data-ttu-id="db9c7-113">longitude</span><span class="sxs-lookup"><span data-stu-id="db9c7-113">longitude</span></span>|<span data-ttu-id="db9c7-114">Double</span><span class="sxs-lookup"><span data-stu-id="db9c7-114">Double</span></span>|<span data-ttu-id="db9c7-115">Долгота, на которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-115">The longitude that the printer is located at.</span></span>|
|<span data-ttu-id="db9c7-116">altitudeInMeters</span><span class="sxs-lookup"><span data-stu-id="db9c7-116">altitudeInMeters</span></span>|<span data-ttu-id="db9c7-117">Int32</span><span class="sxs-lookup"><span data-stu-id="db9c7-117">Int32</span></span>|<span data-ttu-id="db9c7-118">Высота в метрах, на которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-118">The altitude, in meters, that the printer is located at.</span></span>|
|<span data-ttu-id="db9c7-119">streetAddress</span><span class="sxs-lookup"><span data-stu-id="db9c7-119">streetAddress</span></span>|<span data-ttu-id="db9c7-120">String</span><span class="sxs-lookup"><span data-stu-id="db9c7-120">String</span></span>|<span data-ttu-id="db9c7-121">Адрес улицы, где расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-121">The street address where the printer is located.</span></span>|
|<span data-ttu-id="db9c7-122">subUnit</span><span class="sxs-lookup"><span data-stu-id="db9c7-122">subUnit</span></span>|<span data-ttu-id="db9c7-123">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db9c7-123">String collection</span></span>|<span data-ttu-id="db9c7-124">Иерархия подразделения, в которой расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-124">The subunit hierarchy where the printer is located.</span></span> <span data-ttu-id="db9c7-125">Элементы должны быть в иерархичном порядке.</span><span class="sxs-lookup"><span data-stu-id="db9c7-125">The elements should be in hierarchical order.</span></span> <span data-ttu-id="db9c7-126">Например, если кампус разделен на разные разделы, иерархия может выглядеть так: `["East Wing", "Block A"]`</span><span class="sxs-lookup"><span data-stu-id="db9c7-126">For example, if a campus is divided into different sections, the hierarchy might look like this: `["East Wing", "Block A"]`</span></span>|
|<span data-ttu-id="db9c7-127">city</span><span class="sxs-lookup"><span data-stu-id="db9c7-127">city</span></span>|<span data-ttu-id="db9c7-128">String</span><span class="sxs-lookup"><span data-stu-id="db9c7-128">String</span></span>|<span data-ttu-id="db9c7-129">Город, в который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-129">The city that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-130">postalCode</span><span class="sxs-lookup"><span data-stu-id="db9c7-130">postalCode</span></span>|<span data-ttu-id="db9c7-131">String</span><span class="sxs-lookup"><span data-stu-id="db9c7-131">String</span></span>|<span data-ttu-id="db9c7-132">Почтовый код, в который находится принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-132">The postal code that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-133">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="db9c7-133">countryOrRegion</span></span>|<span data-ttu-id="db9c7-134">String</span><span class="sxs-lookup"><span data-stu-id="db9c7-134">String</span></span>|<span data-ttu-id="db9c7-135">Страна или область, в которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-135">The country or region that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-136">site</span><span class="sxs-lookup"><span data-stu-id="db9c7-136">site</span></span>|<span data-ttu-id="db9c7-137">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-137">String</span></span>|<span data-ttu-id="db9c7-138">Сайт, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-138">The site that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-139">здание</span><span class="sxs-lookup"><span data-stu-id="db9c7-139">building</span></span>|<span data-ttu-id="db9c7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-140">String</span></span>|<span data-ttu-id="db9c7-141">Здание, в которое расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-141">The building that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-142">floor</span><span class="sxs-lookup"><span data-stu-id="db9c7-142">floor</span></span>|<span data-ttu-id="db9c7-143">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-143">String</span></span>|<span data-ttu-id="db9c7-144">Пол, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-144">The floor that the printer is located on.</span></span> <span data-ttu-id="db9c7-145">Сейчас поддерживаются только численное значение.</span><span class="sxs-lookup"><span data-stu-id="db9c7-145">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="db9c7-146">floorDescription</span><span class="sxs-lookup"><span data-stu-id="db9c7-146">floorDescription</span></span>|<span data-ttu-id="db9c7-147">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-147">String</span></span>|<span data-ttu-id="db9c7-148">Описание пола, на который расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-148">The description of the floor that the printer is located on.</span></span>|
|<span data-ttu-id="db9c7-149">имя roomName</span><span class="sxs-lookup"><span data-stu-id="db9c7-149">roomName</span></span>|<span data-ttu-id="db9c7-150">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-150">String</span></span>|<span data-ttu-id="db9c7-151">Комната, в которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-151">The room that the printer is located in.</span></span> <span data-ttu-id="db9c7-152">Сейчас поддерживаются только численное значение.</span><span class="sxs-lookup"><span data-stu-id="db9c7-152">Only numerical values are supported right now.</span></span>|
|<span data-ttu-id="db9c7-153">roomDescription</span><span class="sxs-lookup"><span data-stu-id="db9c7-153">roomDescription</span></span>|<span data-ttu-id="db9c7-154">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-154">String</span></span>|<span data-ttu-id="db9c7-155">Описание комнаты, в которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-155">The description of the room that the printer is located in.</span></span>|
|<span data-ttu-id="db9c7-156">organization;</span><span class="sxs-lookup"><span data-stu-id="db9c7-156">organization</span></span>|<span data-ttu-id="db9c7-157">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db9c7-157">String collection</span></span>|<span data-ttu-id="db9c7-158">Иерархия организации, к которой принадлежит принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-158">The organizational hierarchy that the printer belongs to.</span></span> <span data-ttu-id="db9c7-159">Элементы должны быть в иерархичном порядке.</span><span class="sxs-lookup"><span data-stu-id="db9c7-159">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="db9c7-160">подразделение</span><span class="sxs-lookup"><span data-stu-id="db9c7-160">subdivision</span></span>|<span data-ttu-id="db9c7-161">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="db9c7-161">String collection</span></span>|<span data-ttu-id="db9c7-162">Подразделение, в которое расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-162">The subdivision that the printer is located in.</span></span> <span data-ttu-id="db9c7-163">Элементы должны быть в иерархичном порядке.</span><span class="sxs-lookup"><span data-stu-id="db9c7-163">The elements should be in hierarchical order.</span></span>|
|<span data-ttu-id="db9c7-164">stateOrProvince</span><span class="sxs-lookup"><span data-stu-id="db9c7-164">stateOrProvince</span></span>|<span data-ttu-id="db9c7-165">Строка</span><span class="sxs-lookup"><span data-stu-id="db9c7-165">String</span></span>|<span data-ttu-id="db9c7-166">Состояние или область, в которую расположен принтер.</span><span class="sxs-lookup"><span data-stu-id="db9c7-166">The state or province that the printer is located in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db9c7-167">Отношения</span><span class="sxs-lookup"><span data-stu-id="db9c7-167">Relationships</span></span>
<span data-ttu-id="db9c7-168">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="db9c7-168">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db9c7-169">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db9c7-169">JSON representation</span></span>
<span data-ttu-id="db9c7-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db9c7-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerLocation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerLocation",
  "latitude": "Double",
  "longitude": "Double",
  "altitudeInMeters": "Integer",
  "streetAddress": "String",
  "subunit": [
    "String"
  ],
  "city": "String",
  "postalCode": "String",
  "countryOrRegion": "String",
  "site": "String",
  "building": "String",
  "floor": "String",
  "floorDescription": "String",
  "roomName": "String",
  "roomDescription": "String",
  "organization": [
    "String"
  ],
  "subdivision": [
    "String"
  ],
  "stateOrProvince": "String"
}
```

