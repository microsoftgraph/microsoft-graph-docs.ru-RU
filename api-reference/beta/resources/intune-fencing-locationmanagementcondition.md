---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70258c73aa146451dbe0aaab919fc8192017bc27
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979237"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="ddabf-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="ddabf-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="ddabf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ddabf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ddabf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ddabf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ddabf-106">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="ddabf-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="ddabf-107">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ddabf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="ddabf-108">Methods</span></span>
|<span data-ttu-id="ddabf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="ddabf-109">Method</span></span>|<span data-ttu-id="ddabf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ddabf-110">Return Type</span></span>|<span data-ttu-id="ddabf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ddabf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ddabf-112">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="ddabf-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="ddabf-113">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="ddabf-114">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ddabf-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="ddabf-115">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="ddabf-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="ddabf-116">Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="ddabf-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="ddabf-117">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ddabf-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ddabf-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="ddabf-118">Properties</span></span>
|<span data-ttu-id="ddabf-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="ddabf-119">Property</span></span>|<span data-ttu-id="ddabf-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ddabf-120">Type</span></span>|<span data-ttu-id="ddabf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ddabf-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddabf-122">id</span><span class="sxs-lookup"><span data-stu-id="ddabf-122">id</span></span>|<span data-ttu-id="ddabf-123">String</span><span class="sxs-lookup"><span data-stu-id="ddabf-123">String</span></span>|<span data-ttu-id="ddabf-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="ddabf-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="ddabf-125">System generated value assigned when created.</span></span> <span data-ttu-id="ddabf-126">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="ddabf-127">uniqueName</span></span>|<span data-ttu-id="ddabf-128">String</span><span class="sxs-lookup"><span data-stu-id="ddabf-128">String</span></span>|<span data-ttu-id="ddabf-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-129">Unique name for the management condition.</span></span> <span data-ttu-id="ddabf-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-130">Used in management condition expressions.</span></span> <span data-ttu-id="ddabf-131">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ddabf-132">displayName</span></span>|<span data-ttu-id="ddabf-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ddabf-133">String</span></span>|<span data-ttu-id="ddabf-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="ddabf-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="ddabf-135">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-136">description</span><span class="sxs-lookup"><span data-stu-id="ddabf-136">description</span></span>|<span data-ttu-id="ddabf-137">String</span><span class="sxs-lookup"><span data-stu-id="ddabf-137">String</span></span>|<span data-ttu-id="ddabf-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="ddabf-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="ddabf-139">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddabf-140">createdDateTime</span></span>|<span data-ttu-id="ddabf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddabf-141">DateTimeOffset</span></span>|<span data-ttu-id="ddabf-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-142">The time the management condition was created.</span></span> <span data-ttu-id="ddabf-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="ddabf-143">Generated service side.</span></span> <span data-ttu-id="ddabf-144">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddabf-145">modifiedDateTime</span></span>|<span data-ttu-id="ddabf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddabf-146">DateTimeOffset</span></span>|<span data-ttu-id="ddabf-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-147">The time the management condition was last modified.</span></span> <span data-ttu-id="ddabf-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="ddabf-148">Updated service side.</span></span> <span data-ttu-id="ddabf-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-150">eTag</span><span class="sxs-lookup"><span data-stu-id="ddabf-150">eTag</span></span>|<span data-ttu-id="ddabf-151">String</span><span class="sxs-lookup"><span data-stu-id="ddabf-151">String</span></span>|<span data-ttu-id="ddabf-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-152">ETag of the management condition.</span></span> <span data-ttu-id="ddabf-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="ddabf-153">Updated service side.</span></span> <span data-ttu-id="ddabf-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ddabf-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="ddabf-155">applicablePlatforms</span></span>|<span data-ttu-id="ddabf-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ddabf-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ddabf-158">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ddabf-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="ddabf-159">Relationships</span></span>
|<span data-ttu-id="ddabf-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="ddabf-160">Relationship</span></span>|<span data-ttu-id="ddabf-161">Тип</span><span class="sxs-lookup"><span data-stu-id="ddabf-161">Type</span></span>|<span data-ttu-id="ddabf-162">Описание</span><span class="sxs-lookup"><span data-stu-id="ddabf-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddabf-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="ddabf-163">managementConditionStatements</span></span>|<span data-ttu-id="ddabf-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="ddabf-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="ddabf-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="ddabf-166">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ddabf-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ddabf-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ddabf-167">JSON Representation</span></span>
<span data-ttu-id="ddabf-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ddabf-168">Here is a JSON representation of the resource.</span></span>
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





