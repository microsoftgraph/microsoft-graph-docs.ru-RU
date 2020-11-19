---
title: Тип ресурса allDevicesAssignmentTarget
description: Представляет ресурс, назначенный всем управляемым устройствам в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f583f89f8ef3213f980b082cb6b15747722142b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49306949"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="6c3cc-103">Тип ресурса allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6c3cc-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="6c3cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c3cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c3cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c3cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3cc-107">Представляет ресурс, назначенный всем управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="6c3cc-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6c3cc-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6c3cc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6c3cc-109">Properties</span></span>
|<span data-ttu-id="6c3cc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6c3cc-110">Property</span></span>|<span data-ttu-id="6c3cc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6c3cc-111">Type</span></span>|<span data-ttu-id="6c3cc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6c3cc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c3cc-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="6c3cc-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="6c3cc-114">String</span><span class="sxs-lookup"><span data-stu-id="6c3cc-114">String</span></span>|<span data-ttu-id="6c3cc-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="6c3cc-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6c3cc-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="6c3cc-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6c3cc-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="6c3cc-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6c3cc-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="6c3cc-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="6c3cc-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="6c3cc-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="6c3cc-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c3cc-122">Связи</span><span class="sxs-lookup"><span data-stu-id="6c3cc-122">Relationships</span></span>
<span data-ttu-id="6c3cc-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6c3cc-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c3cc-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6c3cc-124">JSON Representation</span></span>
<span data-ttu-id="6c3cc-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6c3cc-125">Here is a JSON representation of the resource.</span></span>
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




