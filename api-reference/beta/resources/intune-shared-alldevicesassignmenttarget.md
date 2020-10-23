---
title: Тип ресурса allDevicesAssignmentTarget
description: Представляет ресурс, назначенный всем управляемым устройствам в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba478c5505796f9039b6ab121fbbd5f9bf30edd4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733163"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="e3d3a-103">Тип ресурса allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e3d3a-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="e3d3a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3d3a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3d3a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3d3a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3d3a-107">Представляет ресурс, назначенный всем управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="e3d3a-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e3d3a-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e3d3a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3d3a-109">Properties</span></span>
|<span data-ttu-id="e3d3a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3d3a-110">Property</span></span>|<span data-ttu-id="e3d3a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e3d3a-111">Type</span></span>|<span data-ttu-id="e3d3a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d3a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d3a-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="e3d3a-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="e3d3a-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e3d3a-114">String</span></span>|<span data-ttu-id="e3d3a-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="e3d3a-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="e3d3a-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="e3d3a-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e3d3a-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="e3d3a-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="e3d3a-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="e3d3a-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="e3d3a-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="e3d3a-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="e3d3a-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3d3a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="e3d3a-122">Relationships</span></span>
<span data-ttu-id="e3d3a-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e3d3a-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3d3a-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3d3a-124">JSON Representation</span></span>
<span data-ttu-id="e3d3a-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3d3a-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allDevicesAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allDevicesAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```





