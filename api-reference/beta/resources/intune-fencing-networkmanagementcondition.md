---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61b5165fb57080bc8568c7f09f1ee9e601d24297
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780121"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="1e21a-103">Тип ресурса Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="1e21a-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="1e21a-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e21a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e21a-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1e21a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e21a-106">Содержит сведения для определения условия управления сетью.</span><span class="sxs-lookup"><span data-stu-id="1e21a-106">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="1e21a-107">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1e21a-108">Методы</span><span class="sxs-lookup"><span data-stu-id="1e21a-108">Methods</span></span>
|<span data-ttu-id="1e21a-109">Метод</span><span class="sxs-lookup"><span data-stu-id="1e21a-109">Method</span></span>|<span data-ttu-id="1e21a-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1e21a-110">Return Type</span></span>|<span data-ttu-id="1e21a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1e21a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e21a-112">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="1e21a-112">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="1e21a-113">Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-113">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="1e21a-114">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1e21a-114">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="1e21a-115">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="1e21a-115">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="1e21a-116">Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="1e21a-116">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="1e21a-117">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="1e21a-117">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1e21a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e21a-118">Properties</span></span>
|<span data-ttu-id="1e21a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e21a-119">Property</span></span>|<span data-ttu-id="1e21a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="1e21a-120">Type</span></span>|<span data-ttu-id="1e21a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="1e21a-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e21a-122">id</span><span class="sxs-lookup"><span data-stu-id="1e21a-122">id</span></span>|<span data-ttu-id="1e21a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="1e21a-123">String</span></span>|<span data-ttu-id="1e21a-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="1e21a-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="1e21a-125">System generated value assigned when created.</span></span> <span data-ttu-id="1e21a-126">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="1e21a-127">uniqueName</span></span>|<span data-ttu-id="1e21a-128">String</span><span class="sxs-lookup"><span data-stu-id="1e21a-128">String</span></span>|<span data-ttu-id="1e21a-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-129">Unique name for the management condition.</span></span> <span data-ttu-id="1e21a-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-130">Used in management condition expressions.</span></span> <span data-ttu-id="1e21a-131">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1e21a-132">displayName</span></span>|<span data-ttu-id="1e21a-133">String</span><span class="sxs-lookup"><span data-stu-id="1e21a-133">String</span></span>|<span data-ttu-id="1e21a-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="1e21a-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="1e21a-135">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-136">description</span><span class="sxs-lookup"><span data-stu-id="1e21a-136">description</span></span>|<span data-ttu-id="1e21a-137">String</span><span class="sxs-lookup"><span data-stu-id="1e21a-137">String</span></span>|<span data-ttu-id="1e21a-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="1e21a-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="1e21a-139">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e21a-140">createdDateTime</span></span>|<span data-ttu-id="1e21a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e21a-141">DateTimeOffset</span></span>|<span data-ttu-id="1e21a-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-142">The time the management condition was created.</span></span> <span data-ttu-id="1e21a-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1e21a-143">Generated service side.</span></span> <span data-ttu-id="1e21a-144">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e21a-145">modifiedDateTime</span></span>|<span data-ttu-id="1e21a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e21a-146">DateTimeOffset</span></span>|<span data-ttu-id="1e21a-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-147">The time the management condition was last modified.</span></span> <span data-ttu-id="1e21a-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1e21a-148">Updated service side.</span></span> <span data-ttu-id="1e21a-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-150">eTag</span><span class="sxs-lookup"><span data-stu-id="1e21a-150">eTag</span></span>|<span data-ttu-id="1e21a-151">String</span><span class="sxs-lookup"><span data-stu-id="1e21a-151">String</span></span>|<span data-ttu-id="1e21a-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-152">ETag of the management condition.</span></span> <span data-ttu-id="1e21a-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="1e21a-153">Updated service side.</span></span> <span data-ttu-id="1e21a-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="1e21a-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="1e21a-155">applicablePlatforms</span></span>|<span data-ttu-id="1e21a-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="1e21a-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="1e21a-158">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e21a-159">Связи</span><span class="sxs-lookup"><span data-stu-id="1e21a-159">Relationships</span></span>
|<span data-ttu-id="1e21a-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="1e21a-160">Relationship</span></span>|<span data-ttu-id="1e21a-161">Тип</span><span class="sxs-lookup"><span data-stu-id="1e21a-161">Type</span></span>|<span data-ttu-id="1e21a-162">Описание</span><span class="sxs-lookup"><span data-stu-id="1e21a-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e21a-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="1e21a-163">managementConditionStatements</span></span>|<span data-ttu-id="1e21a-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="1e21a-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="1e21a-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="1e21a-166">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="1e21a-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e21a-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e21a-167">JSON Representation</span></span>
<span data-ttu-id="1e21a-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1e21a-168">Here is a JSON representation of the resource.</span></span>
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





