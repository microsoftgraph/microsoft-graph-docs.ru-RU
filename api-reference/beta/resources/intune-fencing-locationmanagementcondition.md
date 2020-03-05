---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbbeec236d51d7e7a21321ba0386a473312a4b05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524527"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="aa6a2-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="aa6a2-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="aa6a2-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa6a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa6a2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa6a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa6a2-107">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="aa6a2-108">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="aa6a2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="aa6a2-109">Methods</span></span>
|<span data-ttu-id="aa6a2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="aa6a2-110">Method</span></span>|<span data-ttu-id="aa6a2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="aa6a2-111">Return Type</span></span>|<span data-ttu-id="aa6a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aa6a2-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa6a2-113">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="aa6a2-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="aa6a2-114">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="aa6a2-115">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="aa6a2-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="aa6a2-116">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="aa6a2-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="aa6a2-117">локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="aa6a2-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="aa6a2-118">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="aa6a2-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa6a2-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa6a2-119">Properties</span></span>
|<span data-ttu-id="aa6a2-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa6a2-120">Property</span></span>|<span data-ttu-id="aa6a2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="aa6a2-121">Type</span></span>|<span data-ttu-id="aa6a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aa6a2-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa6a2-123">id</span><span class="sxs-lookup"><span data-stu-id="aa6a2-123">id</span></span>|<span data-ttu-id="aa6a2-124">String</span><span class="sxs-lookup"><span data-stu-id="aa6a2-124">String</span></span>|<span data-ttu-id="aa6a2-125">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="aa6a2-126">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-126">System generated value assigned when created.</span></span> <span data-ttu-id="aa6a2-127">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="aa6a2-128">uniqueName</span></span>|<span data-ttu-id="aa6a2-129">String</span><span class="sxs-lookup"><span data-stu-id="aa6a2-129">String</span></span>|<span data-ttu-id="aa6a2-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-130">Unique name for the management condition.</span></span> <span data-ttu-id="aa6a2-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-131">Used in management condition expressions.</span></span> <span data-ttu-id="aa6a2-132">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="aa6a2-133">displayName</span></span>|<span data-ttu-id="aa6a2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="aa6a2-134">String</span></span>|<span data-ttu-id="aa6a2-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="aa6a2-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-137">description</span><span class="sxs-lookup"><span data-stu-id="aa6a2-137">description</span></span>|<span data-ttu-id="aa6a2-138">String</span><span class="sxs-lookup"><span data-stu-id="aa6a2-138">String</span></span>|<span data-ttu-id="aa6a2-139">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="aa6a2-140">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa6a2-141">createdDateTime</span></span>|<span data-ttu-id="aa6a2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa6a2-142">DateTimeOffset</span></span>|<span data-ttu-id="aa6a2-143">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-143">The time the management condition was created.</span></span> <span data-ttu-id="aa6a2-144">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-144">Generated service side.</span></span> <span data-ttu-id="aa6a2-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa6a2-146">modifiedDateTime</span></span>|<span data-ttu-id="aa6a2-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa6a2-147">DateTimeOffset</span></span>|<span data-ttu-id="aa6a2-148">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-148">The time the management condition was last modified.</span></span> <span data-ttu-id="aa6a2-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-149">Updated service side.</span></span> <span data-ttu-id="aa6a2-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-151">eTag</span><span class="sxs-lookup"><span data-stu-id="aa6a2-151">eTag</span></span>|<span data-ttu-id="aa6a2-152">String</span><span class="sxs-lookup"><span data-stu-id="aa6a2-152">String</span></span>|<span data-ttu-id="aa6a2-153">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-153">ETag of the management condition.</span></span> <span data-ttu-id="aa6a2-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-154">Updated service side.</span></span> <span data-ttu-id="aa6a2-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="aa6a2-156">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="aa6a2-156">applicablePlatforms</span></span>|<span data-ttu-id="aa6a2-157">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="aa6a2-158">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="aa6a2-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa6a2-160">Связи</span><span class="sxs-lookup"><span data-stu-id="aa6a2-160">Relationships</span></span>
|<span data-ttu-id="aa6a2-161">Связь</span><span class="sxs-lookup"><span data-stu-id="aa6a2-161">Relationship</span></span>|<span data-ttu-id="aa6a2-162">Тип</span><span class="sxs-lookup"><span data-stu-id="aa6a2-162">Type</span></span>|<span data-ttu-id="aa6a2-163">Описание</span><span class="sxs-lookup"><span data-stu-id="aa6a2-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa6a2-164">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="aa6a2-164">managementConditionStatements</span></span>|<span data-ttu-id="aa6a2-165">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="aa6a2-166">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="aa6a2-167">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="aa6a2-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa6a2-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa6a2-168">JSON Representation</span></span>
<span data-ttu-id="aa6a2-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa6a2-169">Here is a JSON representation of the resource.</span></span>
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



