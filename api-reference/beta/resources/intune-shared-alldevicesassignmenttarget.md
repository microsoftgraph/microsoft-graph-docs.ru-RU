---
title: Тип ресурса allDevicesAssignmentTarget
description: Представляет ресурс, назначенный всем управляемым устройствам в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69f5e1f77a1fed08d8139e63ffada76e3a948917
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793607"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="f84bc-103">Тип ресурса allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f84bc-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="f84bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f84bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f84bc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f84bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f84bc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f84bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f84bc-107">Представляет ресурс, назначенный всем управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="f84bc-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="f84bc-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f84bc-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f84bc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f84bc-109">Properties</span></span>
|<span data-ttu-id="f84bc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f84bc-110">Property</span></span>|<span data-ttu-id="f84bc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f84bc-111">Type</span></span>|<span data-ttu-id="f84bc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f84bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f84bc-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="f84bc-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="f84bc-114">String</span><span class="sxs-lookup"><span data-stu-id="f84bc-114">String</span></span>|<span data-ttu-id="f84bc-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="f84bc-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="f84bc-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="f84bc-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="f84bc-117">девицеандаппманажементассигнментфилтертипе</span><span class="sxs-lookup"><span data-stu-id="f84bc-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="f84bc-118">девицеандаппманажементассигнментфилтертипе</span><span class="sxs-lookup"><span data-stu-id="f84bc-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="f84bc-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="f84bc-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="f84bc-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="f84bc-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="f84bc-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="f84bc-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f84bc-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f84bc-122">Relationships</span></span>
<span data-ttu-id="f84bc-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f84bc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f84bc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f84bc-124">JSON Representation</span></span>
<span data-ttu-id="f84bc-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f84bc-125">Here is a JSON representation of the resource.</span></span>
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



