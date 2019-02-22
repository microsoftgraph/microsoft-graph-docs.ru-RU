---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 909eaa89a8303948cd97ba47299146b575e32c9f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164836"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="967c5-103">Тип ресурса Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="967c5-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="967c5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="967c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="967c5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="967c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="967c5-106">Содержит сведения для определения условия управления сетью.</span><span class="sxs-lookup"><span data-stu-id="967c5-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="967c5-107">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="967c5-108">Методы</span><span class="sxs-lookup"><span data-stu-id="967c5-108">Methods</span></span>
|<span data-ttu-id="967c5-109">Метод</span><span class="sxs-lookup"><span data-stu-id="967c5-109">Method</span></span>|<span data-ttu-id="967c5-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="967c5-110">Return Type</span></span>|<span data-ttu-id="967c5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="967c5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="967c5-112">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="967c5-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="967c5-113">Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="967c5-114">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="967c5-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="967c5-115">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="967c5-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="967c5-116">Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="967c5-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="967c5-117">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="967c5-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="967c5-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="967c5-118">Properties</span></span>
|<span data-ttu-id="967c5-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="967c5-119">Property</span></span>|<span data-ttu-id="967c5-120">Тип</span><span class="sxs-lookup"><span data-stu-id="967c5-120">Type</span></span>|<span data-ttu-id="967c5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="967c5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="967c5-122">id</span><span class="sxs-lookup"><span data-stu-id="967c5-122">id</span></span>|<span data-ttu-id="967c5-123">String</span><span class="sxs-lookup"><span data-stu-id="967c5-123">String</span></span>|<span data-ttu-id="967c5-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="967c5-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="967c5-125">System generated value assigned when created.</span></span> <span data-ttu-id="967c5-126">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="967c5-127">uniqueName</span></span>|<span data-ttu-id="967c5-128">String</span><span class="sxs-lookup"><span data-stu-id="967c5-128">String</span></span>|<span data-ttu-id="967c5-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-129">Unique name for the management condition.</span></span> <span data-ttu-id="967c5-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-130">Used in management condition expressions.</span></span> <span data-ttu-id="967c5-131">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="967c5-132">displayName</span></span>|<span data-ttu-id="967c5-133">String</span><span class="sxs-lookup"><span data-stu-id="967c5-133">String</span></span>|<span data-ttu-id="967c5-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="967c5-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="967c5-135">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-136">description</span><span class="sxs-lookup"><span data-stu-id="967c5-136">description</span></span>|<span data-ttu-id="967c5-137">Строка</span><span class="sxs-lookup"><span data-stu-id="967c5-137">String</span></span>|<span data-ttu-id="967c5-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="967c5-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="967c5-139">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="967c5-140">createdDateTime</span></span>|<span data-ttu-id="967c5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="967c5-141">DateTimeOffset</span></span>|<span data-ttu-id="967c5-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-142">The time the management condition was created.</span></span> <span data-ttu-id="967c5-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="967c5-143">Generated service side.</span></span> <span data-ttu-id="967c5-144">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="967c5-145">modifiedDateTime</span></span>|<span data-ttu-id="967c5-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="967c5-146">DateTimeOffset</span></span>|<span data-ttu-id="967c5-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-147">The time the management condition was last modified.</span></span> <span data-ttu-id="967c5-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="967c5-148">Updated service side.</span></span> <span data-ttu-id="967c5-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-150">eTag</span><span class="sxs-lookup"><span data-stu-id="967c5-150">eTag</span></span>|<span data-ttu-id="967c5-151">String</span><span class="sxs-lookup"><span data-stu-id="967c5-151">String</span></span>|<span data-ttu-id="967c5-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-152">ETag of the management condition.</span></span> <span data-ttu-id="967c5-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="967c5-153">Updated service side.</span></span> <span data-ttu-id="967c5-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="967c5-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="967c5-155">applicablePlatforms</span></span>|<span data-ttu-id="967c5-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="967c5-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="967c5-158">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="967c5-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="967c5-159">Relationships</span></span>
|<span data-ttu-id="967c5-160">Связь</span><span class="sxs-lookup"><span data-stu-id="967c5-160">Relationship</span></span>|<span data-ttu-id="967c5-161">Тип</span><span class="sxs-lookup"><span data-stu-id="967c5-161">Type</span></span>|<span data-ttu-id="967c5-162">Описание</span><span class="sxs-lookup"><span data-stu-id="967c5-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="967c5-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="967c5-163">managementConditionStatements</span></span>|<span data-ttu-id="967c5-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="967c5-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="967c5-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="967c5-166">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="967c5-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="967c5-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="967c5-167">JSON Representation</span></span>
<span data-ttu-id="967c5-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="967c5-168">Here is a JSON representation of the resource.</span></span>
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




