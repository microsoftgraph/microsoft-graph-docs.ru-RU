---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2560309e937bb1b2e6ffd436cec5988fd38dbf2c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773149"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="b8ecf-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="b8ecf-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="b8ecf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8ecf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ecf-106">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="b8ecf-107">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b8ecf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="b8ecf-108">Methods</span></span>
|<span data-ttu-id="b8ecf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="b8ecf-109">Method</span></span>|<span data-ttu-id="b8ecf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b8ecf-110">Return Type</span></span>|<span data-ttu-id="b8ecf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ecf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8ecf-112">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="b8ecf-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="b8ecf-113">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="b8ecf-114">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b8ecf-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="b8ecf-115">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="b8ecf-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="b8ecf-116">Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="b8ecf-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="b8ecf-117">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="b8ecf-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8ecf-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8ecf-118">Properties</span></span>
|<span data-ttu-id="b8ecf-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8ecf-119">Property</span></span>|<span data-ttu-id="b8ecf-120">Тип</span><span class="sxs-lookup"><span data-stu-id="b8ecf-120">Type</span></span>|<span data-ttu-id="b8ecf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ecf-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ecf-122">id</span><span class="sxs-lookup"><span data-stu-id="b8ecf-122">id</span></span>|<span data-ttu-id="b8ecf-123">Строка</span><span class="sxs-lookup"><span data-stu-id="b8ecf-123">String</span></span>|<span data-ttu-id="b8ecf-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="b8ecf-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-125">System generated value assigned when created.</span></span> <span data-ttu-id="b8ecf-126">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="b8ecf-127">uniqueName</span></span>|<span data-ttu-id="b8ecf-128">String</span><span class="sxs-lookup"><span data-stu-id="b8ecf-128">String</span></span>|<span data-ttu-id="b8ecf-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-129">Unique name for the management condition.</span></span> <span data-ttu-id="b8ecf-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-130">Used in management condition expressions.</span></span> <span data-ttu-id="b8ecf-131">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b8ecf-132">displayName</span></span>|<span data-ttu-id="b8ecf-133">String</span><span class="sxs-lookup"><span data-stu-id="b8ecf-133">String</span></span>|<span data-ttu-id="b8ecf-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="b8ecf-135">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-136">description</span><span class="sxs-lookup"><span data-stu-id="b8ecf-136">description</span></span>|<span data-ttu-id="b8ecf-137">String</span><span class="sxs-lookup"><span data-stu-id="b8ecf-137">String</span></span>|<span data-ttu-id="b8ecf-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="b8ecf-139">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ecf-140">createdDateTime</span></span>|<span data-ttu-id="b8ecf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ecf-141">DateTimeOffset</span></span>|<span data-ttu-id="b8ecf-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-142">The time the management condition was created.</span></span> <span data-ttu-id="b8ecf-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-143">Generated service side.</span></span> <span data-ttu-id="b8ecf-144">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ecf-145">modifiedDateTime</span></span>|<span data-ttu-id="b8ecf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ecf-146">DateTimeOffset</span></span>|<span data-ttu-id="b8ecf-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-147">The time the management condition was last modified.</span></span> <span data-ttu-id="b8ecf-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-148">Updated service side.</span></span> <span data-ttu-id="b8ecf-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-150">eTag</span><span class="sxs-lookup"><span data-stu-id="b8ecf-150">eTag</span></span>|<span data-ttu-id="b8ecf-151">String</span><span class="sxs-lookup"><span data-stu-id="b8ecf-151">String</span></span>|<span data-ttu-id="b8ecf-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-152">ETag of the management condition.</span></span> <span data-ttu-id="b8ecf-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-153">Updated service side.</span></span> <span data-ttu-id="b8ecf-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b8ecf-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="b8ecf-155">applicablePlatforms</span></span>|<span data-ttu-id="b8ecf-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b8ecf-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b8ecf-158">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ecf-159">Связи</span><span class="sxs-lookup"><span data-stu-id="b8ecf-159">Relationships</span></span>
|<span data-ttu-id="b8ecf-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="b8ecf-160">Relationship</span></span>|<span data-ttu-id="b8ecf-161">Тип</span><span class="sxs-lookup"><span data-stu-id="b8ecf-161">Type</span></span>|<span data-ttu-id="b8ecf-162">Описание</span><span class="sxs-lookup"><span data-stu-id="b8ecf-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ecf-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="b8ecf-163">managementConditionStatements</span></span>|<span data-ttu-id="b8ecf-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="b8ecf-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="b8ecf-166">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b8ecf-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8ecf-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8ecf-167">JSON Representation</span></span>
<span data-ttu-id="b8ecf-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8ecf-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.locationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





