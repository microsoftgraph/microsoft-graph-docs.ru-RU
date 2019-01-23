---
title: Тип ресурса locationManagementCondition
description: Содержит данные для определения условие управления расположение области интересов, мониторинг.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c2eddf43696bd9300cc8dcd3408dbcd6fc5a9e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422798"
---
# <a name="locationmanagementcondition-resource-type"></a><span data-ttu-id="ab739-103">Тип ресурса locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ab739-103">locationManagementCondition resource type</span></span>

> <span data-ttu-id="ab739-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab739-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab739-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab739-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab739-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab739-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab739-107">Содержит данные для определения условие управления расположение области интересов, мониторинг.</span><span class="sxs-lookup"><span data-stu-id="ab739-107">Contains the information to define a location management condition, an area of interest, to monitor.</span></span>


<span data-ttu-id="ab739-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ab739-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ab739-109">Methods</span></span>
|<span data-ttu-id="ab739-110">Метод</span><span class="sxs-lookup"><span data-stu-id="ab739-110">Method</span></span>|<span data-ttu-id="ab739-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ab739-111">Return Type</span></span>|<span data-ttu-id="ab739-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ab739-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab739-113">Список locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="ab739-113">List locationManagementConditions</span></span>](../api/intune-fencing-locationmanagementcondition-list.md)|<span data-ttu-id="ab739-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ab739-114">[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) collection</span></span>|<span data-ttu-id="ab739-115">Свойства списка и связей объектов [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ab739-115">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="ab739-116">Получение locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ab739-116">Get locationManagementCondition</span></span>](../api/intune-fencing-locationmanagementcondition-get.md)|[<span data-ttu-id="ab739-117">locationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="ab739-117">locationManagementCondition</span></span>](../resources/intune-fencing-locationmanagementcondition.md)|<span data-ttu-id="ab739-118">Чтение свойства и связи объекта [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="ab739-118">Read properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab739-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab739-119">Properties</span></span>
|<span data-ttu-id="ab739-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab739-120">Property</span></span>|<span data-ttu-id="ab739-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ab739-121">Type</span></span>|<span data-ttu-id="ab739-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ab739-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab739-123">id</span><span class="sxs-lookup"><span data-stu-id="ab739-123">id</span></span>|<span data-ttu-id="ab739-124">String</span><span class="sxs-lookup"><span data-stu-id="ab739-124">String</span></span>|<span data-ttu-id="ab739-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="ab739-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="ab739-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="ab739-126">System generated value assigned when created.</span></span> <span data-ttu-id="ab739-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="ab739-128">uniqueName</span></span>|<span data-ttu-id="ab739-129">String</span><span class="sxs-lookup"><span data-stu-id="ab739-129">String</span></span>|<span data-ttu-id="ab739-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="ab739-130">Unique name for the management condition.</span></span> <span data-ttu-id="ab739-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-131">Used in management condition expressions.</span></span> <span data-ttu-id="ab739-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ab739-133">displayName</span></span>|<span data-ttu-id="ab739-134">String</span><span class="sxs-lookup"><span data-stu-id="ab739-134">String</span></span>|<span data-ttu-id="ab739-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="ab739-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="ab739-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-137">description</span><span class="sxs-lookup"><span data-stu-id="ab739-137">description</span></span>|<span data-ttu-id="ab739-138">String</span><span class="sxs-lookup"><span data-stu-id="ab739-138">String</span></span>|<span data-ttu-id="ab739-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="ab739-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="ab739-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab739-141">createdDateTime</span></span>|<span data-ttu-id="ab739-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab739-142">DateTimeOffset</span></span>|<span data-ttu-id="ab739-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-143">The time the management condition was created.</span></span> <span data-ttu-id="ab739-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="ab739-144">Generated service side.</span></span> <span data-ttu-id="ab739-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab739-146">modifiedDateTime</span></span>|<span data-ttu-id="ab739-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab739-147">DateTimeOffset</span></span>|<span data-ttu-id="ab739-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-148">The time the management condition was last modified.</span></span> <span data-ttu-id="ab739-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="ab739-149">Updated service side.</span></span> <span data-ttu-id="ab739-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-151">eTag</span><span class="sxs-lookup"><span data-stu-id="ab739-151">eTag</span></span>|<span data-ttu-id="ab739-152">String</span><span class="sxs-lookup"><span data-stu-id="ab739-152">String</span></span>|<span data-ttu-id="ab739-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-153">ETag of the management condition.</span></span> <span data-ttu-id="ab739-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="ab739-154">Updated service side.</span></span> <span data-ttu-id="ab739-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="ab739-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="ab739-156">applicablePlatforms</span></span>|<span data-ttu-id="ab739-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ab739-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="ab739-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="ab739-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab739-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab739-160">Relationships</span></span>
|<span data-ttu-id="ab739-161">Связь</span><span class="sxs-lookup"><span data-stu-id="ab739-161">Relationship</span></span>|<span data-ttu-id="ab739-162">Тип</span><span class="sxs-lookup"><span data-stu-id="ab739-162">Type</span></span>|<span data-ttu-id="ab739-163">Описание</span><span class="sxs-lookup"><span data-stu-id="ab739-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab739-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="ab739-164">managementConditionStatements</span></span>|<span data-ttu-id="ab739-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="ab739-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="ab739-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="ab739-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="ab739-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="ab739-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab739-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab739-168">JSON Representation</span></span>
<span data-ttu-id="ab739-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab739-169">Here is a JSON representation of the resource.</span></span>
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




