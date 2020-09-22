---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df962c30994a315f448ac41496037796b35dc24e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039365"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="1164a-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1164a-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="1164a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1164a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1164a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1164a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1164a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1164a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1164a-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="1164a-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="1164a-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1164a-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1164a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1164a-109">Properties</span></span>
|<span data-ttu-id="1164a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1164a-110">Property</span></span>|<span data-ttu-id="1164a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1164a-111">Type</span></span>|<span data-ttu-id="1164a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1164a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1164a-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="1164a-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="1164a-114">String</span><span class="sxs-lookup"><span data-stu-id="1164a-114">String</span></span>|<span data-ttu-id="1164a-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="1164a-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="1164a-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1164a-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="1164a-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1164a-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="1164a-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1164a-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="1164a-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="1164a-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="1164a-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="1164a-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="1164a-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="1164a-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="1164a-122">groupId</span><span class="sxs-lookup"><span data-stu-id="1164a-122">groupId</span></span>|<span data-ttu-id="1164a-123">String</span><span class="sxs-lookup"><span data-stu-id="1164a-123">String</span></span>|<span data-ttu-id="1164a-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="1164a-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="1164a-125">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1164a-125">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1164a-126">Отношения</span><span class="sxs-lookup"><span data-stu-id="1164a-126">Relationships</span></span>
<span data-ttu-id="1164a-127">Нет</span><span class="sxs-lookup"><span data-stu-id="1164a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1164a-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1164a-128">JSON Representation</span></span>
<span data-ttu-id="1164a-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1164a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```






