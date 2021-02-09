---
title: Тип ресурса deviceManagementConfigurationPolicyAssignment
description: Объект DeviceManagementConfigurationPolicyAssignment назначает определенное deviceManagementConfigurationPolicy группе AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e571983c36c2832aef5c43478d1cccca7361aca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157668"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a><span data-ttu-id="03c17-103">Тип ресурса deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-103">deviceManagementConfigurationPolicyAssignment resource type</span></span>

<span data-ttu-id="03c17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03c17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03c17-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03c17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03c17-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="03c17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03c17-107">Объект DeviceManagementConfigurationPolicyAssignment назначает определенное deviceManagementConfigurationPolicy группе AAD.</span><span class="sxs-lookup"><span data-stu-id="03c17-107">The DeviceManagementConfigurationPolicyAssignment entity assigns a specific DeviceManagementConfigurationPolicy to an AAD group.</span></span>

## <a name="methods"></a><span data-ttu-id="03c17-108">Методы</span><span class="sxs-lookup"><span data-stu-id="03c17-108">Methods</span></span>
|<span data-ttu-id="03c17-109">Метод</span><span class="sxs-lookup"><span data-stu-id="03c17-109">Method</span></span>|<span data-ttu-id="03c17-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03c17-110">Return Type</span></span>|<span data-ttu-id="03c17-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03c17-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03c17-112">Список deviceManagementConfigurationPolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="03c17-112">List deviceManagementConfigurationPolicyAssignments</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|<span data-ttu-id="03c17-113">[Коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-113">[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) collection</span></span>|<span data-ttu-id="03c17-114">Список свойств и связей объектов [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-114">List properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) objects.</span></span>|
|[<span data-ttu-id="03c17-115">Get deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-115">Get deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[<span data-ttu-id="03c17-116">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-116">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="03c17-117">Чтение свойств и связей объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-117">Read properties and relationships of the [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="03c17-118">Создание deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-118">Create deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[<span data-ttu-id="03c17-119">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-119">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="03c17-120">Создание объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-120">Create a new [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|
|[<span data-ttu-id="03c17-121">Удаление deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-121">Delete deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|<span data-ttu-id="03c17-122">Нет</span><span class="sxs-lookup"><span data-stu-id="03c17-122">None</span></span>|<span data-ttu-id="03c17-123">Удаляет [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-123">Deletes a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).</span></span>|
|[<span data-ttu-id="03c17-124">Обновление deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-124">Update deviceManagementConfigurationPolicyAssignment</span></span>](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[<span data-ttu-id="03c17-125">deviceManagementConfigurationPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="03c17-125">deviceManagementConfigurationPolicyAssignment</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|<span data-ttu-id="03c17-126">Обновление свойств объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03c17-126">Update the properties of a [deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03c17-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="03c17-127">Properties</span></span>
|<span data-ttu-id="03c17-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="03c17-128">Property</span></span>|<span data-ttu-id="03c17-129">Тип</span><span class="sxs-lookup"><span data-stu-id="03c17-129">Type</span></span>|<span data-ttu-id="03c17-130">Описание</span><span class="sxs-lookup"><span data-stu-id="03c17-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03c17-131">id</span><span class="sxs-lookup"><span data-stu-id="03c17-131">id</span></span>|<span data-ttu-id="03c17-132">String</span><span class="sxs-lookup"><span data-stu-id="03c17-132">String</span></span>|<span data-ttu-id="03c17-133">Ключ назначения.</span><span class="sxs-lookup"><span data-stu-id="03c17-133">The key of the assignment.</span></span>|
|<span data-ttu-id="03c17-134">target</span><span class="sxs-lookup"><span data-stu-id="03c17-134">target</span></span>|[<span data-ttu-id="03c17-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="03c17-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="03c17-136">Целевой объект назначения для DeviceManagementConfigurationPolicy.</span><span class="sxs-lookup"><span data-stu-id="03c17-136">The assignment target for the DeviceManagementConfigurationPolicy.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03c17-137">Связи</span><span class="sxs-lookup"><span data-stu-id="03c17-137">Relationships</span></span>
<span data-ttu-id="03c17-138">Нет</span><span class="sxs-lookup"><span data-stu-id="03c17-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03c17-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03c17-139">JSON Representation</span></span>
<span data-ttu-id="03c17-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03c17-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




