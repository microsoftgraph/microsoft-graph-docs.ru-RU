---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46e32312dc501219d887fcebb5da435ad2690031
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987742"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="de96f-103">Тип ресурса Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="de96f-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="de96f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de96f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de96f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="de96f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de96f-106">Содержит сведения для определения условия управления сетью.</span><span class="sxs-lookup"><span data-stu-id="de96f-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="de96f-107">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="de96f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="de96f-108">Methods</span></span>
|<span data-ttu-id="de96f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="de96f-109">Method</span></span>|<span data-ttu-id="de96f-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="de96f-110">Return Type</span></span>|<span data-ttu-id="de96f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="de96f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="de96f-112">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="de96f-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="de96f-113">Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="de96f-114">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="de96f-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="de96f-115">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="de96f-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="de96f-116">Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="de96f-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="de96f-117">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="de96f-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="de96f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="de96f-118">Properties</span></span>
|<span data-ttu-id="de96f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="de96f-119">Property</span></span>|<span data-ttu-id="de96f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="de96f-120">Type</span></span>|<span data-ttu-id="de96f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="de96f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de96f-122">id</span><span class="sxs-lookup"><span data-stu-id="de96f-122">id</span></span>|<span data-ttu-id="de96f-123">String</span><span class="sxs-lookup"><span data-stu-id="de96f-123">String</span></span>|<span data-ttu-id="de96f-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="de96f-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="de96f-125">System generated value assigned when created.</span></span> <span data-ttu-id="de96f-126">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="de96f-127">uniqueName</span></span>|<span data-ttu-id="de96f-128">String</span><span class="sxs-lookup"><span data-stu-id="de96f-128">String</span></span>|<span data-ttu-id="de96f-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-129">Unique name for the management condition.</span></span> <span data-ttu-id="de96f-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-130">Used in management condition expressions.</span></span> <span data-ttu-id="de96f-131">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="de96f-132">displayName</span></span>|<span data-ttu-id="de96f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="de96f-133">String</span></span>|<span data-ttu-id="de96f-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="de96f-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="de96f-135">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-136">description</span><span class="sxs-lookup"><span data-stu-id="de96f-136">description</span></span>|<span data-ttu-id="de96f-137">String</span><span class="sxs-lookup"><span data-stu-id="de96f-137">String</span></span>|<span data-ttu-id="de96f-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="de96f-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="de96f-139">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de96f-140">createdDateTime</span></span>|<span data-ttu-id="de96f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de96f-141">DateTimeOffset</span></span>|<span data-ttu-id="de96f-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-142">The time the management condition was created.</span></span> <span data-ttu-id="de96f-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="de96f-143">Generated service side.</span></span> <span data-ttu-id="de96f-144">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de96f-145">modifiedDateTime</span></span>|<span data-ttu-id="de96f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de96f-146">DateTimeOffset</span></span>|<span data-ttu-id="de96f-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-147">The time the management condition was last modified.</span></span> <span data-ttu-id="de96f-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="de96f-148">Updated service side.</span></span> <span data-ttu-id="de96f-149">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-150">eTag</span><span class="sxs-lookup"><span data-stu-id="de96f-150">eTag</span></span>|<span data-ttu-id="de96f-151">String</span><span class="sxs-lookup"><span data-stu-id="de96f-151">String</span></span>|<span data-ttu-id="de96f-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-152">ETag of the management condition.</span></span> <span data-ttu-id="de96f-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="de96f-153">Updated service side.</span></span> <span data-ttu-id="de96f-154">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="de96f-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="de96f-155">applicablePlatforms</span></span>|<span data-ttu-id="de96f-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="de96f-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="de96f-158">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="de96f-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="de96f-159">Relationships</span></span>
|<span data-ttu-id="de96f-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="de96f-160">Relationship</span></span>|<span data-ttu-id="de96f-161">Тип</span><span class="sxs-lookup"><span data-stu-id="de96f-161">Type</span></span>|<span data-ttu-id="de96f-162">Описание</span><span class="sxs-lookup"><span data-stu-id="de96f-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de96f-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="de96f-163">managementConditionStatements</span></span>|<span data-ttu-id="de96f-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="de96f-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="de96f-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="de96f-166">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="de96f-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de96f-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="de96f-167">JSON Representation</span></span>
<span data-ttu-id="de96f-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="de96f-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkManagementCondition",
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





