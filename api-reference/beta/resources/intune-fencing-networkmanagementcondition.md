---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9a2c7435e626f7339268b514951552dbb2dd948b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298885"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="0c137-103">Тип ресурса Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="0c137-103">networkManagementCondition resource type</span></span>

<span data-ttu-id="0c137-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c137-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c137-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c137-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c137-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c137-107">Содержит сведения для определения условия управления сетью.</span><span class="sxs-lookup"><span data-stu-id="0c137-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="0c137-108">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0c137-109">Методы</span><span class="sxs-lookup"><span data-stu-id="0c137-109">Methods</span></span>
|<span data-ttu-id="0c137-110">Метод</span><span class="sxs-lookup"><span data-stu-id="0c137-110">Method</span></span>|<span data-ttu-id="0c137-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0c137-111">Return Type</span></span>|<span data-ttu-id="0c137-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0c137-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c137-113">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="0c137-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="0c137-114">Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="0c137-115">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0c137-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="0c137-116">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="0c137-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="0c137-117">нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="0c137-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="0c137-118">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="0c137-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0c137-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c137-119">Properties</span></span>
|<span data-ttu-id="0c137-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c137-120">Property</span></span>|<span data-ttu-id="0c137-121">Тип</span><span class="sxs-lookup"><span data-stu-id="0c137-121">Type</span></span>|<span data-ttu-id="0c137-122">Описание</span><span class="sxs-lookup"><span data-stu-id="0c137-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c137-123">id</span><span class="sxs-lookup"><span data-stu-id="0c137-123">id</span></span>|<span data-ttu-id="0c137-124">String</span><span class="sxs-lookup"><span data-stu-id="0c137-124">String</span></span>|<span data-ttu-id="0c137-125">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="0c137-126">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="0c137-126">System generated value assigned when created.</span></span> <span data-ttu-id="0c137-127">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="0c137-128">uniqueName</span></span>|<span data-ttu-id="0c137-129">String</span><span class="sxs-lookup"><span data-stu-id="0c137-129">String</span></span>|<span data-ttu-id="0c137-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-130">Unique name for the management condition.</span></span> <span data-ttu-id="0c137-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-131">Used in management condition expressions.</span></span> <span data-ttu-id="0c137-132">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-133">displayName</span><span class="sxs-lookup"><span data-stu-id="0c137-133">displayName</span></span>|<span data-ttu-id="0c137-134">String</span><span class="sxs-lookup"><span data-stu-id="0c137-134">String</span></span>|<span data-ttu-id="0c137-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="0c137-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="0c137-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-137">description</span><span class="sxs-lookup"><span data-stu-id="0c137-137">description</span></span>|<span data-ttu-id="0c137-138">String</span><span class="sxs-lookup"><span data-stu-id="0c137-138">String</span></span>|<span data-ttu-id="0c137-139">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="0c137-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="0c137-140">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c137-141">createdDateTime</span></span>|<span data-ttu-id="0c137-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c137-142">DateTimeOffset</span></span>|<span data-ttu-id="0c137-143">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-143">The time the management condition was created.</span></span> <span data-ttu-id="0c137-144">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="0c137-144">Generated service side.</span></span> <span data-ttu-id="0c137-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c137-146">modifiedDateTime</span></span>|<span data-ttu-id="0c137-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c137-147">DateTimeOffset</span></span>|<span data-ttu-id="0c137-148">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-148">The time the management condition was last modified.</span></span> <span data-ttu-id="0c137-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="0c137-149">Updated service side.</span></span> <span data-ttu-id="0c137-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-151">eTag</span><span class="sxs-lookup"><span data-stu-id="0c137-151">eTag</span></span>|<span data-ttu-id="0c137-152">String</span><span class="sxs-lookup"><span data-stu-id="0c137-152">String</span></span>|<span data-ttu-id="0c137-153">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-153">ETag of the management condition.</span></span> <span data-ttu-id="0c137-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="0c137-154">Updated service side.</span></span> <span data-ttu-id="0c137-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="0c137-156">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="0c137-156">applicablePlatforms</span></span>|<span data-ttu-id="0c137-157">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="0c137-158">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="0c137-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c137-160">Связи</span><span class="sxs-lookup"><span data-stu-id="0c137-160">Relationships</span></span>
|<span data-ttu-id="0c137-161">Связь</span><span class="sxs-lookup"><span data-stu-id="0c137-161">Relationship</span></span>|<span data-ttu-id="0c137-162">Тип</span><span class="sxs-lookup"><span data-stu-id="0c137-162">Type</span></span>|<span data-ttu-id="0c137-163">Описание</span><span class="sxs-lookup"><span data-stu-id="0c137-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c137-164">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="0c137-164">managementConditionStatements</span></span>|<span data-ttu-id="0c137-165">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="0c137-166">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="0c137-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="0c137-167">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="0c137-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c137-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c137-168">JSON Representation</span></span>
<span data-ttu-id="0c137-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c137-169">Here is a JSON representation of the resource.</span></span>
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




