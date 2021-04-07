---
title: Тип ресурса allDevicesAssignmentTarget
description: Представляет ресурс, назначенный всем управляемым устройствам в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ca3d3b4dbbe534189c66eba09ecbc6e99258936
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612303"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="b0e72-103">Тип ресурса allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0e72-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="b0e72-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0e72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0e72-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0e72-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0e72-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0e72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0e72-107">Представляет ресурс, назначенный всем управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b0e72-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="b0e72-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="b0e72-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0e72-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0e72-109">Properties</span></span>
|<span data-ttu-id="b0e72-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0e72-110">Property</span></span>|<span data-ttu-id="b0e72-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b0e72-111">Type</span></span>|<span data-ttu-id="b0e72-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b0e72-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e72-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="b0e72-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="b0e72-114">String</span><span class="sxs-lookup"><span data-stu-id="b0e72-114">String</span></span>|<span data-ttu-id="b0e72-115">Id фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="b0e72-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="b0e72-116">Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="b0e72-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="b0e72-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="b0e72-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="b0e72-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="b0e72-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="b0e72-119">Тип фильтра целевого назначения, то есть исключить или включить.</span><span class="sxs-lookup"><span data-stu-id="b0e72-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="b0e72-120">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="b0e72-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="b0e72-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="b0e72-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0e72-122">Связи</span><span class="sxs-lookup"><span data-stu-id="b0e72-122">Relationships</span></span>
<span data-ttu-id="b0e72-123">Нет</span><span class="sxs-lookup"><span data-stu-id="b0e72-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0e72-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0e72-124">JSON Representation</span></span>
<span data-ttu-id="b0e72-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0e72-125">Here is a JSON representation of the resource.</span></span>
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




