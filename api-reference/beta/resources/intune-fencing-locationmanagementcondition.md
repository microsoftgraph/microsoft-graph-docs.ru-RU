---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56e9c10d8d9d53a9e0009b6a70210da6d7873065
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783258"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="53b30-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="53b30-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="53b30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53b30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53b30-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53b30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53b30-106">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="53b30-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="53b30-107">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="53b30-108">Методы</span><span class="sxs-lookup"><span data-stu-id="53b30-108">Methods</span></span>
|<span data-ttu-id="53b30-109">Метод</span><span class="sxs-lookup"><span data-stu-id="53b30-109">Method</span></span>|<span data-ttu-id="53b30-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53b30-110">Return Type</span></span>|<span data-ttu-id="53b30-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53b30-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53b30-112">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="53b30-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="53b30-113">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="53b30-114">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="53b30-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="53b30-115">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="53b30-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="53b30-116">локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="53b30-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="53b30-117">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="53b30-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53b30-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="53b30-118">Properties</span></span>
|<span data-ttu-id="53b30-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="53b30-119">Property</span></span>|<span data-ttu-id="53b30-120">Тип</span><span class="sxs-lookup"><span data-stu-id="53b30-120">Type</span></span>|<span data-ttu-id="53b30-121">Описание</span><span class="sxs-lookup"><span data-stu-id="53b30-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b30-122">id</span><span class="sxs-lookup"><span data-stu-id="53b30-122">id</span></span>|<span data-ttu-id="53b30-123">String</span><span class="sxs-lookup"><span data-stu-id="53b30-123">String</span></span>|<span data-ttu-id="53b30-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="53b30-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="53b30-125">System generated value assigned when created.</span></span> <span data-ttu-id="53b30-126">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="53b30-127">uniqueName</span></span>|<span data-ttu-id="53b30-128">String</span><span class="sxs-lookup"><span data-stu-id="53b30-128">String</span></span>|<span data-ttu-id="53b30-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-129">Unique name for the management condition.</span></span> <span data-ttu-id="53b30-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-130">Used in management condition expressions.</span></span> <span data-ttu-id="53b30-131">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-132">displayName</span><span class="sxs-lookup"><span data-stu-id="53b30-132">displayName</span></span>|<span data-ttu-id="53b30-133">Строка</span><span class="sxs-lookup"><span data-stu-id="53b30-133">String</span></span>|<span data-ttu-id="53b30-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="53b30-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="53b30-135">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-136">description</span><span class="sxs-lookup"><span data-stu-id="53b30-136">description</span></span>|<span data-ttu-id="53b30-137">String</span><span class="sxs-lookup"><span data-stu-id="53b30-137">String</span></span>|<span data-ttu-id="53b30-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="53b30-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="53b30-139">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53b30-140">createdDateTime</span></span>|<span data-ttu-id="53b30-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b30-141">DateTimeOffset</span></span>|<span data-ttu-id="53b30-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-142">The time the management condition was created.</span></span> <span data-ttu-id="53b30-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="53b30-143">Generated service side.</span></span> <span data-ttu-id="53b30-144">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53b30-145">modifiedDateTime</span></span>|<span data-ttu-id="53b30-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b30-146">DateTimeOffset</span></span>|<span data-ttu-id="53b30-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-147">The time the management condition was last modified.</span></span> <span data-ttu-id="53b30-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="53b30-148">Updated service side.</span></span> <span data-ttu-id="53b30-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-150">eTag</span><span class="sxs-lookup"><span data-stu-id="53b30-150">eTag</span></span>|<span data-ttu-id="53b30-151">String</span><span class="sxs-lookup"><span data-stu-id="53b30-151">String</span></span>|<span data-ttu-id="53b30-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-152">ETag of the management condition.</span></span> <span data-ttu-id="53b30-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="53b30-153">Updated service side.</span></span> <span data-ttu-id="53b30-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="53b30-155">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="53b30-155">applicablePlatforms</span></span>|<span data-ttu-id="53b30-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="53b30-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="53b30-158">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="53b30-159">Связи</span><span class="sxs-lookup"><span data-stu-id="53b30-159">Relationships</span></span>
|<span data-ttu-id="53b30-160">Связь</span><span class="sxs-lookup"><span data-stu-id="53b30-160">Relationship</span></span>|<span data-ttu-id="53b30-161">Тип</span><span class="sxs-lookup"><span data-stu-id="53b30-161">Type</span></span>|<span data-ttu-id="53b30-162">Описание</span><span class="sxs-lookup"><span data-stu-id="53b30-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b30-163">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="53b30-163">managementConditionStatements</span></span>|<span data-ttu-id="53b30-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="53b30-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="53b30-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="53b30-166">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="53b30-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53b30-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53b30-167">JSON Representation</span></span>
<span data-ttu-id="53b30-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53b30-168">Here is a JSON representation of the resource.</span></span>
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



