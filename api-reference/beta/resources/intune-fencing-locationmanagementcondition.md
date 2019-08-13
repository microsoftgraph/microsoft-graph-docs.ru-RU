---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3b8f18b36383b9a7bfee6fa541a60248d9f5c851
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331710"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="077fe-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="077fe-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="077fe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="077fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="077fe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="077fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="077fe-106">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="077fe-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="077fe-107">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="077fe-108">Методы</span><span class="sxs-lookup"><span data-stu-id="077fe-108">Methods</span></span>
|<span data-ttu-id="077fe-109">Метод</span><span class="sxs-lookup"><span data-stu-id="077fe-109">Method</span></span>|<span data-ttu-id="077fe-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="077fe-110">Return Type</span></span>|<span data-ttu-id="077fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="077fe-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="077fe-112">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="077fe-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="077fe-113">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="077fe-114">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="077fe-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="077fe-115">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="077fe-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="077fe-116">локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="077fe-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="077fe-117">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="077fe-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="077fe-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="077fe-118">Properties</span></span>
|<span data-ttu-id="077fe-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="077fe-119">Property</span></span>|<span data-ttu-id="077fe-120">Тип</span><span class="sxs-lookup"><span data-stu-id="077fe-120">Type</span></span>|<span data-ttu-id="077fe-121">Описание</span><span class="sxs-lookup"><span data-stu-id="077fe-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="077fe-122">id</span><span class="sxs-lookup"><span data-stu-id="077fe-122">id</span></span>|<span data-ttu-id="077fe-123">String</span><span class="sxs-lookup"><span data-stu-id="077fe-123">String</span></span>|<span data-ttu-id="077fe-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="077fe-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="077fe-125">System generated value assigned when created.</span></span> <span data-ttu-id="077fe-126">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="077fe-127">uniqueName</span></span>|<span data-ttu-id="077fe-128">String</span><span class="sxs-lookup"><span data-stu-id="077fe-128">String</span></span>|<span data-ttu-id="077fe-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-129">Unique name for the management condition.</span></span> <span data-ttu-id="077fe-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-130">Used in management condition expressions.</span></span> <span data-ttu-id="077fe-131">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-132">displayName</span><span class="sxs-lookup"><span data-stu-id="077fe-132">displayName</span></span>|<span data-ttu-id="077fe-133">Строка</span><span class="sxs-lookup"><span data-stu-id="077fe-133">String</span></span>|<span data-ttu-id="077fe-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="077fe-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="077fe-135">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-136">description</span><span class="sxs-lookup"><span data-stu-id="077fe-136">description</span></span>|<span data-ttu-id="077fe-137">String</span><span class="sxs-lookup"><span data-stu-id="077fe-137">String</span></span>|<span data-ttu-id="077fe-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="077fe-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="077fe-139">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="077fe-140">createdDateTime</span></span>|<span data-ttu-id="077fe-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="077fe-141">DateTimeOffset</span></span>|<span data-ttu-id="077fe-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-142">The time the management condition was created.</span></span> <span data-ttu-id="077fe-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="077fe-143">Generated service side.</span></span> <span data-ttu-id="077fe-144">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="077fe-145">modifiedDateTime</span></span>|<span data-ttu-id="077fe-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="077fe-146">DateTimeOffset</span></span>|<span data-ttu-id="077fe-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-147">The time the management condition was last modified.</span></span> <span data-ttu-id="077fe-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="077fe-148">Updated service side.</span></span> <span data-ttu-id="077fe-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-150">eTag</span><span class="sxs-lookup"><span data-stu-id="077fe-150">eTag</span></span>|<span data-ttu-id="077fe-151">String</span><span class="sxs-lookup"><span data-stu-id="077fe-151">String</span></span>|<span data-ttu-id="077fe-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-152">ETag of the management condition.</span></span> <span data-ttu-id="077fe-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="077fe-153">Updated service side.</span></span> <span data-ttu-id="077fe-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="077fe-155">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="077fe-155">applicablePlatforms</span></span>|<span data-ttu-id="077fe-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="077fe-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="077fe-158">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="077fe-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="077fe-159">Relationships</span></span>
|<span data-ttu-id="077fe-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="077fe-160">Relationship</span></span>|<span data-ttu-id="077fe-161">Тип</span><span class="sxs-lookup"><span data-stu-id="077fe-161">Type</span></span>|<span data-ttu-id="077fe-162">Описание</span><span class="sxs-lookup"><span data-stu-id="077fe-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="077fe-163">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="077fe-163">managementConditionStatements</span></span>|<span data-ttu-id="077fe-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="077fe-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="077fe-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="077fe-166">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="077fe-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="077fe-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="077fe-167">JSON Representation</span></span>
<span data-ttu-id="077fe-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="077fe-168">Here is a JSON representation of the resource.</span></span>
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



