---
title: Тип ресурса Локатионманажементкондитион
description: Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2560309e937bb1b2e6ffd436cec5988fd38dbf2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568838"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="2dce4-103">Тип ресурса Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="2dce4-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="2dce4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2dce4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dce4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2dce4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dce4-106">Содержит сведения, определяющие условие управления размещением, область интересов для мониторинга.</span><span class="sxs-lookup"><span data-stu-id="2dce4-106">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="2dce4-107">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-107">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2dce4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="2dce4-108">Methods</span></span>
|<span data-ttu-id="2dce4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="2dce4-109">Method</span></span>|<span data-ttu-id="2dce4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2dce4-110">Return Type</span></span>|<span data-ttu-id="2dce4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2dce4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2dce4-112">Список Локатионманажементкондитионс</span><span class="sxs-lookup"><span data-stu-id="2dce4-112">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="2dce4-113">Коллекция [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-113">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="2dce4-114">Список свойств и связей объектов [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="2dce4-114">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="2dce4-115">Получение Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="2dce4-115">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="2dce4-116">Локатионманажементкондитион</span><span class="sxs-lookup"><span data-stu-id="2dce4-116">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="2dce4-117">Чтение свойств и связей объекта [локатионманажементкондитион](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="2dce4-117">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2dce4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="2dce4-118">Properties</span></span>
|<span data-ttu-id="2dce4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="2dce4-119">Property</span></span>|<span data-ttu-id="2dce4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="2dce4-120">Type</span></span>|<span data-ttu-id="2dce4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="2dce4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dce4-122">id</span><span class="sxs-lookup"><span data-stu-id="2dce4-122">id</span></span>|<span data-ttu-id="2dce4-123">Строка</span><span class="sxs-lookup"><span data-stu-id="2dce4-123">String</span></span>|<span data-ttu-id="2dce4-124">Уникальный идентификатор для условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-124">Unique identifier for the management condition.</span></span> <span data-ttu-id="2dce4-125">Созданное системой значение, назначаемое при создании.</span><span class="sxs-lookup"><span data-stu-id="2dce4-125">System generated value assigned when created.</span></span> <span data-ttu-id="2dce4-126">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-126">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-127">uniqueName</span><span class="sxs-lookup"><span data-stu-id="2dce4-127">uniqueName</span></span>|<span data-ttu-id="2dce4-128">String</span><span class="sxs-lookup"><span data-stu-id="2dce4-128">String</span></span>|<span data-ttu-id="2dce4-129">Уникальное имя условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-129">Unique name for the management condition.</span></span> <span data-ttu-id="2dce4-130">Используется в выражениях условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-130">Used in management condition expressions.</span></span> <span data-ttu-id="2dce4-131">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-131">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2dce4-132">displayName</span></span>|<span data-ttu-id="2dce4-133">String</span><span class="sxs-lookup"><span data-stu-id="2dce4-133">String</span></span>|<span data-ttu-id="2dce4-134">Имя условия управления, определенное администратором.</span><span class="sxs-lookup"><span data-stu-id="2dce4-134">The admin defined name of the management condition.</span></span> <span data-ttu-id="2dce4-135">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-135">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-136">description</span><span class="sxs-lookup"><span data-stu-id="2dce4-136">description</span></span>|<span data-ttu-id="2dce4-137">String</span><span class="sxs-lookup"><span data-stu-id="2dce4-137">String</span></span>|<span data-ttu-id="2dce4-138">Описание условия управления, заданное администратором.</span><span class="sxs-lookup"><span data-stu-id="2dce4-138">The admin defined description of the management condition.</span></span> <span data-ttu-id="2dce4-139">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-139">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dce4-140">createdDateTime</span></span>|<span data-ttu-id="2dce4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dce4-141">DateTimeOffset</span></span>|<span data-ttu-id="2dce4-142">Время создания условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-142">The time the management condition was created.</span></span> <span data-ttu-id="2dce4-143">Созданная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="2dce4-143">Generated service side.</span></span> <span data-ttu-id="2dce4-144">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-144">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-145">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dce4-145">modifiedDateTime</span></span>|<span data-ttu-id="2dce4-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dce4-146">DateTimeOffset</span></span>|<span data-ttu-id="2dce4-147">Время последнего изменения условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-147">The time the management condition was last modified.</span></span> <span data-ttu-id="2dce4-148">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="2dce4-148">Updated service side.</span></span> <span data-ttu-id="2dce4-149">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-150">eTag</span><span class="sxs-lookup"><span data-stu-id="2dce4-150">eTag</span></span>|<span data-ttu-id="2dce4-151">String</span><span class="sxs-lookup"><span data-stu-id="2dce4-151">String</span></span>|<span data-ttu-id="2dce4-152">Тег ETag условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-152">ETag of the management condition.</span></span> <span data-ttu-id="2dce4-153">Обновленная сторона службы.</span><span class="sxs-lookup"><span data-stu-id="2dce4-153">Updated service side.</span></span> <span data-ttu-id="2dce4-154">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="2dce4-155">Аппликаблеплатформс</span><span class="sxs-lookup"><span data-stu-id="2dce4-155">applicablePlatforms</span></span>|<span data-ttu-id="2dce4-156">Коллекция [девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-156">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="2dce4-157">Соответствующие платформы для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-157">The applicable platforms for this management condition.</span></span> <span data-ttu-id="2dce4-158">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-158">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dce4-159">Связи</span><span class="sxs-lookup"><span data-stu-id="2dce4-159">Relationships</span></span>
|<span data-ttu-id="2dce4-160">Отношение</span><span class="sxs-lookup"><span data-stu-id="2dce4-160">Relationship</span></span>|<span data-ttu-id="2dce4-161">Тип</span><span class="sxs-lookup"><span data-stu-id="2dce4-161">Type</span></span>|<span data-ttu-id="2dce4-162">Описание</span><span class="sxs-lookup"><span data-stu-id="2dce4-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dce4-163">Манажементкондитионстатементс</span><span class="sxs-lookup"><span data-stu-id="2dce4-163">managementConditionStatements</span></span>|<span data-ttu-id="2dce4-164">Коллекция [манажементкондитионстатемент](../resources/intune-fencing-managementconditionstatement.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-164">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="2dce4-165">Операторы условия управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="2dce4-165">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="2dce4-166">НаСледуется от [манажементкондитион](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="2dce4-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dce4-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2dce4-167">JSON Representation</span></span>
<span data-ttu-id="2dce4-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2dce4-168">Here is a JSON representation of the resource.</span></span>
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





