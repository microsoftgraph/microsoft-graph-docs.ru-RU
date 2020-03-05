---
title: Тип ресурса Нетворкманажементкондитион
description: Содержит сведения для определения условия управления сетью.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bced41a40200cd79d58fe71a36cf1af5b1a65cc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528150"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="66551-103">Тип ресурса Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="66551-103">networkManagementCondition resource type</span></span>

<span data-ttu-id="66551-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="66551-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66551-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66551-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66551-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66551-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66551-107">Содержит сведения для определения условия управления сетью.</span><span class="sxs-lookup"><span data-stu-id="66551-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="66551-108">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="66551-109">Методы</span><span class="sxs-lookup"><span data-stu-id="66551-109">Methods</span></span>
|<span data-ttu-id="66551-110">Метод</span><span class="sxs-lookup"><span data-stu-id="66551-110">Method</span></span>|<span data-ttu-id="66551-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="66551-111">Return Type</span></span>|<span data-ttu-id="66551-112">Описание</span><span class="sxs-lookup"><span data-stu-id="66551-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66551-113">Список Нетворкманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="66551-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="66551-114">Коллекция [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="66551-115">Список свойств и связей объектов [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="66551-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="66551-116">Получение Нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="66551-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="66551-117">нетворкманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="66551-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="66551-118">Чтение свойств и связей объекта [нетворкманажементкондитион](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="66551-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="66551-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="66551-119">Properties</span></span>
|<span data-ttu-id="66551-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="66551-120">Property</span></span>|<span data-ttu-id="66551-121">Тип</span><span class="sxs-lookup"><span data-stu-id="66551-121">Type</span></span>|<span data-ttu-id="66551-122">Описание</span><span class="sxs-lookup"><span data-stu-id="66551-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66551-123">id</span><span class="sxs-lookup"><span data-stu-id="66551-123">id</span></span>|<span data-ttu-id="66551-124">String</span><span class="sxs-lookup"><span data-stu-id="66551-124">String</span></span>|<span data-ttu-id="66551-125">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="66551-126">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="66551-126">System generated value assigned when created.</span></span> <span data-ttu-id="66551-127">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="66551-128">uniqueName</span></span>|<span data-ttu-id="66551-129">String</span><span class="sxs-lookup"><span data-stu-id="66551-129">String</span></span>|<span data-ttu-id="66551-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-130">Unique name for the management condition.</span></span> <span data-ttu-id="66551-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-131">Used in management condition expressions.</span></span> <span data-ttu-id="66551-132">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-133">displayName</span><span class="sxs-lookup"><span data-stu-id="66551-133">displayName</span></span>|<span data-ttu-id="66551-134">Строка</span><span class="sxs-lookup"><span data-stu-id="66551-134">String</span></span>|<span data-ttu-id="66551-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="66551-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="66551-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-137">description</span><span class="sxs-lookup"><span data-stu-id="66551-137">description</span></span>|<span data-ttu-id="66551-138">String</span><span class="sxs-lookup"><span data-stu-id="66551-138">String</span></span>|<span data-ttu-id="66551-139">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="66551-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="66551-140">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66551-141">createdDateTime</span></span>|<span data-ttu-id="66551-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66551-142">DateTimeOffset</span></span>|<span data-ttu-id="66551-143">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-143">The time the management condition was created.</span></span> <span data-ttu-id="66551-144">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="66551-144">Generated service side.</span></span> <span data-ttu-id="66551-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66551-146">modifiedDateTime</span></span>|<span data-ttu-id="66551-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66551-147">DateTimeOffset</span></span>|<span data-ttu-id="66551-148">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-148">The time the management condition was last modified.</span></span> <span data-ttu-id="66551-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="66551-149">Updated service side.</span></span> <span data-ttu-id="66551-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-151">eTag</span><span class="sxs-lookup"><span data-stu-id="66551-151">eTag</span></span>|<span data-ttu-id="66551-152">String</span><span class="sxs-lookup"><span data-stu-id="66551-152">String</span></span>|<span data-ttu-id="66551-153">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-153">ETag of the management condition.</span></span> <span data-ttu-id="66551-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="66551-154">Updated service side.</span></span> <span data-ttu-id="66551-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="66551-156">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="66551-156">applicablePlatforms</span></span>|<span data-ttu-id="66551-157">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="66551-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="66551-158">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="66551-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="66551-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="66551-160">Связи</span><span class="sxs-lookup"><span data-stu-id="66551-160">Relationships</span></span>
|<span data-ttu-id="66551-161">Связь</span><span class="sxs-lookup"><span data-stu-id="66551-161">Relationship</span></span>|<span data-ttu-id="66551-162">Тип</span><span class="sxs-lookup"><span data-stu-id="66551-162">Type</span></span>|<span data-ttu-id="66551-163">Описание</span><span class="sxs-lookup"><span data-stu-id="66551-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66551-164">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="66551-164">managementConditionStatements</span></span>|<span data-ttu-id="66551-165">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="66551-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="66551-166">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="66551-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="66551-167">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="66551-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66551-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66551-168">JSON Representation</span></span>
<span data-ttu-id="66551-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66551-169">Here is a JSON representation of the resource.</span></span>
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



