---
title: Тип ресурса networkManagementCondition
description: Содержит данные для определения состояния управления сети.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4eadaf4e67b7ffe5551fc82376c3a4bb58255f61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415763"
---
# <a name="networkmanagementcondition-resource-type"></a><span data-ttu-id="def3a-103">Тип ресурса networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="def3a-103">networkManagementCondition resource type</span></span>

> <span data-ttu-id="def3a-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="def3a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="def3a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="def3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="def3a-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="def3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def3a-107">Содержит данные для определения состояния управления сети.</span><span class="sxs-lookup"><span data-stu-id="def3a-107">Contains the information to define a network management condition.</span></span>


<span data-ttu-id="def3a-108">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-108">Inherits from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="def3a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="def3a-109">Methods</span></span>
|<span data-ttu-id="def3a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="def3a-110">Method</span></span>|<span data-ttu-id="def3a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="def3a-111">Return Type</span></span>|<span data-ttu-id="def3a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="def3a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="def3a-113">Список networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="def3a-113">List networkManagementConditions</span></span>](../api/intune-fencing-networkmanagementcondition-list.md)|<span data-ttu-id="def3a-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="def3a-114">[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) collection</span></span>|<span data-ttu-id="def3a-115">Свойства списка и связей объектов [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="def3a-115">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="def3a-116">Получение networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="def3a-116">Get networkManagementCondition</span></span>](../api/intune-fencing-networkmanagementcondition-get.md)|[<span data-ttu-id="def3a-117">networkManagementCondition</span><span class="sxs-lookup"><span data-stu-id="def3a-117">networkManagementCondition</span></span>](../resources/intune-fencing-networkmanagementcondition.md)|<span data-ttu-id="def3a-118">Чтение свойства и связи объекта [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) .</span><span class="sxs-lookup"><span data-stu-id="def3a-118">Read properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="def3a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="def3a-119">Properties</span></span>
|<span data-ttu-id="def3a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="def3a-120">Property</span></span>|<span data-ttu-id="def3a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="def3a-121">Type</span></span>|<span data-ttu-id="def3a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="def3a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def3a-123">id</span><span class="sxs-lookup"><span data-stu-id="def3a-123">id</span></span>|<span data-ttu-id="def3a-124">String</span><span class="sxs-lookup"><span data-stu-id="def3a-124">String</span></span>|<span data-ttu-id="def3a-125">Уникальный идентификатор для управления условия.</span><span class="sxs-lookup"><span data-stu-id="def3a-125">Unique identifier for the management condition.</span></span> <span data-ttu-id="def3a-126">Значение, назначенное при создании создаваемый системой.</span><span class="sxs-lookup"><span data-stu-id="def3a-126">System generated value assigned when created.</span></span> <span data-ttu-id="def3a-127">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-127">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-128">уникального имени</span><span class="sxs-lookup"><span data-stu-id="def3a-128">uniqueName</span></span>|<span data-ttu-id="def3a-129">String</span><span class="sxs-lookup"><span data-stu-id="def3a-129">String</span></span>|<span data-ttu-id="def3a-130">Уникальное имя для управления условия.</span><span class="sxs-lookup"><span data-stu-id="def3a-130">Unique name for the management condition.</span></span> <span data-ttu-id="def3a-131">Используется в выражениях условие управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-131">Used in management condition expressions.</span></span> <span data-ttu-id="def3a-132">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-132">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="def3a-133">displayName</span></span>|<span data-ttu-id="def3a-134">String</span><span class="sxs-lookup"><span data-stu-id="def3a-134">String</span></span>|<span data-ttu-id="def3a-135">Имя условия управления определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="def3a-135">The admin defined name of the management condition.</span></span> <span data-ttu-id="def3a-136">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-137">description</span><span class="sxs-lookup"><span data-stu-id="def3a-137">description</span></span>|<span data-ttu-id="def3a-138">String</span><span class="sxs-lookup"><span data-stu-id="def3a-138">String</span></span>|<span data-ttu-id="def3a-139">Описание управления условия, определенные администратором.</span><span class="sxs-lookup"><span data-stu-id="def3a-139">The admin defined description of the management condition.</span></span> <span data-ttu-id="def3a-140">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-140">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="def3a-141">createdDateTime</span></span>|<span data-ttu-id="def3a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="def3a-142">DateTimeOffset</span></span>|<span data-ttu-id="def3a-143">Время создания условие управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-143">The time the management condition was created.</span></span> <span data-ttu-id="def3a-144">Создан со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="def3a-144">Generated service side.</span></span> <span data-ttu-id="def3a-145">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="def3a-146">modifiedDateTime</span></span>|<span data-ttu-id="def3a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="def3a-147">DateTimeOffset</span></span>|<span data-ttu-id="def3a-148">Время последнего изменения условие управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-148">The time the management condition was last modified.</span></span> <span data-ttu-id="def3a-149">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="def3a-149">Updated service side.</span></span> <span data-ttu-id="def3a-150">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-151">eTag</span><span class="sxs-lookup"><span data-stu-id="def3a-151">eTag</span></span>|<span data-ttu-id="def3a-152">String</span><span class="sxs-lookup"><span data-stu-id="def3a-152">String</span></span>|<span data-ttu-id="def3a-153">ETag условие управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-153">ETag of the management condition.</span></span> <span data-ttu-id="def3a-154">Обновление со стороны службы.</span><span class="sxs-lookup"><span data-stu-id="def3a-154">Updated service side.</span></span> <span data-ttu-id="def3a-155">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="def3a-156">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="def3a-156">applicablePlatforms</span></span>|<span data-ttu-id="def3a-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="def3a-157">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="def3a-158">Применимые платформ для этого условия управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-158">The applicable platforms for this management condition.</span></span> <span data-ttu-id="def3a-159">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="def3a-160">Отношения</span><span class="sxs-lookup"><span data-stu-id="def3a-160">Relationships</span></span>
|<span data-ttu-id="def3a-161">Связь</span><span class="sxs-lookup"><span data-stu-id="def3a-161">Relationship</span></span>|<span data-ttu-id="def3a-162">Тип</span><span class="sxs-lookup"><span data-stu-id="def3a-162">Type</span></span>|<span data-ttu-id="def3a-163">Описание</span><span class="sxs-lookup"><span data-stu-id="def3a-163">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def3a-164">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="def3a-164">managementConditionStatements</span></span>|<span data-ttu-id="def3a-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="def3a-165">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="def3a-166">Операторы условие управления, связанные с условием управления.</span><span class="sxs-lookup"><span data-stu-id="def3a-166">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="def3a-167">Наследуется от [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="def3a-167">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="def3a-168">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="def3a-168">JSON Representation</span></span>
<span data-ttu-id="def3a-169">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="def3a-169">Here is a JSON representation of the resource.</span></span>
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




