---
title: Тип ресурса allDevicesAssignmentTarget
description: Представляет ресурс, назначенный всем управляемым устройствам в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e018d766074db808f123882ab54f590958f95bd
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156751"
---
# <a name="alldevicesassignmenttarget-resource-type"></a><span data-ttu-id="7f1b8-103">Тип ресурса allDevicesAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7f1b8-103">allDevicesAssignmentTarget resource type</span></span>

<span data-ttu-id="7f1b8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f1b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f1b8-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f1b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f1b8-107">Представляет ресурс, назначенный всем управляемым устройствам в клиенте.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-107">Represents an assignment to all managed devices in the tenant.</span></span>


<span data-ttu-id="7f1b8-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f1b8-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f1b8-109">Properties</span></span>
|<span data-ttu-id="7f1b8-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f1b8-110">Property</span></span>|<span data-ttu-id="7f1b8-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7f1b8-111">Type</span></span>|<span data-ttu-id="7f1b8-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7f1b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f1b8-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="7f1b8-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="7f1b8-114">String</span><span class="sxs-lookup"><span data-stu-id="7f1b8-114">String</span></span>|<span data-ttu-id="7f1b8-115">ИД фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="7f1b8-116">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="7f1b8-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="7f1b8-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="7f1b8-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="7f1b8-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="7f1b8-119">Тип фильтра целевого назначения, например "Исключить" или "Включить".</span><span class="sxs-lookup"><span data-stu-id="7f1b8-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="7f1b8-120">Наследуется [от deviceAndAppManagementAssignmentTarget.](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="7f1b8-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f1b8-122">Связи</span><span class="sxs-lookup"><span data-stu-id="7f1b8-122">Relationships</span></span>
<span data-ttu-id="7f1b8-123">Нет</span><span class="sxs-lookup"><span data-stu-id="7f1b8-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f1b8-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f1b8-124">JSON Representation</span></span>
<span data-ttu-id="7f1b8-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-125">Here is a JSON representation of the resource.</span></span>
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




