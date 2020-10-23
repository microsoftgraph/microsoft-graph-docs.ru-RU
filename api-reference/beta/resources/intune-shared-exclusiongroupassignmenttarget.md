---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e17d73e4a7979b03ab7206267d8aebbab9556a23
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735129"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="6eb52-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6eb52-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="6eb52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6eb52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6eb52-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6eb52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6eb52-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6eb52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eb52-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="6eb52-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="6eb52-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6eb52-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6eb52-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb52-109">Properties</span></span>
|<span data-ttu-id="6eb52-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb52-110">Property</span></span>|<span data-ttu-id="6eb52-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb52-111">Type</span></span>|<span data-ttu-id="6eb52-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb52-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eb52-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="6eb52-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="6eb52-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6eb52-114">String</span></span>|<span data-ttu-id="6eb52-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="6eb52-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="6eb52-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6eb52-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="6eb52-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6eb52-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="6eb52-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="6eb52-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="6eb52-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="6eb52-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="6eb52-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="6eb52-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="6eb52-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="6eb52-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="6eb52-122">groupId</span><span class="sxs-lookup"><span data-stu-id="6eb52-122">groupId</span></span>|<span data-ttu-id="6eb52-123">String</span><span class="sxs-lookup"><span data-stu-id="6eb52-123">String</span></span>|<span data-ttu-id="6eb52-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="6eb52-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="6eb52-125">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="6eb52-125">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eb52-126">Связи</span><span class="sxs-lookup"><span data-stu-id="6eb52-126">Relationships</span></span>
<span data-ttu-id="6eb52-127">Нет</span><span class="sxs-lookup"><span data-stu-id="6eb52-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eb52-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eb52-128">JSON Representation</span></span>
<span data-ttu-id="6eb52-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb52-129">Here is a JSON representation of the resource.</span></span>
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





