---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f11c23b7e01636fb49273465e340b1085d9b3b2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302707"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="dc821-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="dc821-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="dc821-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc821-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc821-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc821-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc821-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dc821-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc821-107">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="dc821-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="dc821-108">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="dc821-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dc821-109">Methods</span></span>
|<span data-ttu-id="dc821-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dc821-110">Method</span></span>|<span data-ttu-id="dc821-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dc821-111">Return Type</span></span>|<span data-ttu-id="dc821-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dc821-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dc821-113">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="dc821-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="dc821-114">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="dc821-115">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="dc821-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="dc821-116">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="dc821-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="dc821-117">локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="dc821-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="dc821-118">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="dc821-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dc821-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc821-119">Properties</span></span>
|<span data-ttu-id="dc821-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc821-120">Property</span></span>|<span data-ttu-id="dc821-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dc821-121">Type</span></span>|<span data-ttu-id="dc821-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc821-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc821-123">id</span><span class="sxs-lookup"><span data-stu-id="dc821-123">id</span></span>|<span data-ttu-id="dc821-124">String</span><span class="sxs-lookup"><span data-stu-id="dc821-124">String</span></span>|<span data-ttu-id="dc821-125">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="dc821-126">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="dc821-126">System generated value assigned when created.</span></span> <span data-ttu-id="dc821-127">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="dc821-128">uniqueName</span></span>|<span data-ttu-id="dc821-129">String</span><span class="sxs-lookup"><span data-stu-id="dc821-129">String</span></span>|<span data-ttu-id="dc821-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-130">Unique name for the management condition.</span></span> <span data-ttu-id="dc821-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-131">Used in management condition expressions.</span></span> <span data-ttu-id="dc821-132">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-133">displayName</span><span class="sxs-lookup"><span data-stu-id="dc821-133">displayName</span></span>|<span data-ttu-id="dc821-134">String</span><span class="sxs-lookup"><span data-stu-id="dc821-134">String</span></span>|<span data-ttu-id="dc821-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="dc821-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="dc821-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-137">description</span><span class="sxs-lookup"><span data-stu-id="dc821-137">description</span></span>|<span data-ttu-id="dc821-138">String</span><span class="sxs-lookup"><span data-stu-id="dc821-138">String</span></span>|<span data-ttu-id="dc821-139">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="dc821-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="dc821-140">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc821-141">createdDateTime</span></span>|<span data-ttu-id="dc821-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc821-142">DateTimeOffset</span></span>|<span data-ttu-id="dc821-143">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-143">The time the management condition was created.</span></span> <span data-ttu-id="dc821-144">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="dc821-144">Generated service side.</span></span> <span data-ttu-id="dc821-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc821-146">modifiedDateTime</span></span>|<span data-ttu-id="dc821-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc821-147">DateTimeOffset</span></span>|<span data-ttu-id="dc821-148">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-148">The time the management condition was last modified.</span></span> <span data-ttu-id="dc821-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="dc821-149">Updated service side.</span></span> <span data-ttu-id="dc821-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-151">eTag</span><span class="sxs-lookup"><span data-stu-id="dc821-151">eTag</span></span>|<span data-ttu-id="dc821-152">String</span><span class="sxs-lookup"><span data-stu-id="dc821-152">String</span></span>|<span data-ttu-id="dc821-153">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-153">ETag of the management condition.</span></span> <span data-ttu-id="dc821-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="dc821-154">Updated service side.</span></span> <span data-ttu-id="dc821-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="dc821-156">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="dc821-156">applicablePlatforms</span></span>|<span data-ttu-id="dc821-157">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="dc821-158">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="dc821-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc821-160">Связи</span><span class="sxs-lookup"><span data-stu-id="dc821-160">Relationships</span></span>
|<span data-ttu-id="dc821-161">Связь</span><span class="sxs-lookup"><span data-stu-id="dc821-161">Relationship</span></span>|<span data-ttu-id="dc821-162">Тип</span><span class="sxs-lookup"><span data-stu-id="dc821-162">Type</span></span>|<span data-ttu-id="dc821-163">Описание</span><span class="sxs-lookup"><span data-stu-id="dc821-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc821-164">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="dc821-164">managementConditionStatements</span></span>|<span data-ttu-id="dc821-165">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="dc821-166">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="dc821-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="dc821-167">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="dc821-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc821-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc821-168">JSON Representation</span></span>
<span data-ttu-id="dc821-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc821-169">Here is a JSON representation of the resource.</span></span>
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




