---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e03e4c1d31fec4fbcff4f3f610710c1120a6a47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722882"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="f09c3-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="f09c3-103">locationManagementCondition resource type</span></span>

<span data-ttu-id="f09c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f09c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f09c3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f09c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f09c3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f09c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f09c3-107">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="f09c3-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="f09c3-108">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f09c3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="f09c3-109">Methods</span></span>
|<span data-ttu-id="f09c3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="f09c3-110">Method</span></span>|<span data-ttu-id="f09c3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f09c3-111">Return Type</span></span>|<span data-ttu-id="f09c3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f09c3-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f09c3-113">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="f09c3-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="f09c3-114">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="f09c3-115">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f09c3-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="f09c3-116">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="f09c3-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="f09c3-117">локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="f09c3-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="f09c3-118">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="f09c3-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f09c3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f09c3-119">Properties</span></span>
|<span data-ttu-id="f09c3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f09c3-120">Property</span></span>|<span data-ttu-id="f09c3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f09c3-121">Type</span></span>|<span data-ttu-id="f09c3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f09c3-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f09c3-123">id</span><span class="sxs-lookup"><span data-stu-id="f09c3-123">id</span></span>|<span data-ttu-id="f09c3-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f09c3-124">String</span></span>|<span data-ttu-id="f09c3-125">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="f09c3-126">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="f09c3-126">System generated value assigned when created.</span></span> <span data-ttu-id="f09c3-127">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-128">uniqueName</span><span class="sxs-lookup"><span data-stu-id="f09c3-128">uniqueName</span></span>|<span data-ttu-id="f09c3-129">Строка</span><span class="sxs-lookup"><span data-stu-id="f09c3-129">String</span></span>|<span data-ttu-id="f09c3-130">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-130">Unique name for the management condition.</span></span> <span data-ttu-id="f09c3-131">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-131">Used in management condition expressions.</span></span> <span data-ttu-id="f09c3-132">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f09c3-133">displayName</span></span>|<span data-ttu-id="f09c3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f09c3-134">String</span></span>|<span data-ttu-id="f09c3-135">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="f09c3-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="f09c3-136">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-137">description</span><span class="sxs-lookup"><span data-stu-id="f09c3-137">description</span></span>|<span data-ttu-id="f09c3-138">Строка</span><span class="sxs-lookup"><span data-stu-id="f09c3-138">String</span></span>|<span data-ttu-id="f09c3-139">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="f09c3-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="f09c3-140">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f09c3-141">createdDateTime</span></span>|<span data-ttu-id="f09c3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f09c3-142">DateTimeOffset</span></span>|<span data-ttu-id="f09c3-143">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-143">The time the management condition was created.</span></span> <span data-ttu-id="f09c3-144">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f09c3-144">Generated service side.</span></span> <span data-ttu-id="f09c3-145">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f09c3-146">modifiedDateTime</span></span>|<span data-ttu-id="f09c3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f09c3-147">DateTimeOffset</span></span>|<span data-ttu-id="f09c3-148">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-148">The time the management condition was last modified.</span></span> <span data-ttu-id="f09c3-149">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f09c3-149">Updated service side.</span></span> <span data-ttu-id="f09c3-150">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-151">eTag</span><span class="sxs-lookup"><span data-stu-id="f09c3-151">eTag</span></span>|<span data-ttu-id="f09c3-152">String</span><span class="sxs-lookup"><span data-stu-id="f09c3-152">String</span></span>|<span data-ttu-id="f09c3-153">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-153">ETag of the management condition.</span></span> <span data-ttu-id="f09c3-154">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="f09c3-154">Updated service side.</span></span> <span data-ttu-id="f09c3-155">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="f09c3-156">аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="f09c3-156">applicablePlatforms</span></span>|<span data-ttu-id="f09c3-157">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f09c3-158">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="f09c3-159">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f09c3-160">Связи</span><span class="sxs-lookup"><span data-stu-id="f09c3-160">Relationships</span></span>
|<span data-ttu-id="f09c3-161">Связь</span><span class="sxs-lookup"><span data-stu-id="f09c3-161">Relationship</span></span>|<span data-ttu-id="f09c3-162">Тип</span><span class="sxs-lookup"><span data-stu-id="f09c3-162">Type</span></span>|<span data-ttu-id="f09c3-163">Описание</span><span class="sxs-lookup"><span data-stu-id="f09c3-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f09c3-164">манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="f09c3-164">managementConditionStatements</span></span>|<span data-ttu-id="f09c3-165">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="f09c3-166">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="f09c3-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="f09c3-167">Наследуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="f09c3-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f09c3-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f09c3-168">JSON Representation</span></span>
<span data-ttu-id="f09c3-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f09c3-169">Here is a JSON representation of the resource.</span></span>
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





