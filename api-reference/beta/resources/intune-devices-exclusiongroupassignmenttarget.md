---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00e3fecab48e0c34e500dd7b3d9e7c114de0c8d8
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612327"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="bd884-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bd884-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="bd884-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd884-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd884-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd884-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd884-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd884-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd884-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="bd884-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="bd884-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bd884-108">Inherits from [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd884-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd884-109">Properties</span></span>
|<span data-ttu-id="bd884-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd884-110">Property</span></span>|<span data-ttu-id="bd884-111">Тип</span><span class="sxs-lookup"><span data-stu-id="bd884-111">Type</span></span>|<span data-ttu-id="bd884-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bd884-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd884-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="bd884-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="bd884-114">String</span><span class="sxs-lookup"><span data-stu-id="bd884-114">String</span></span>|<span data-ttu-id="bd884-115">Id фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="bd884-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="bd884-116">Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bd884-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="bd884-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="bd884-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="bd884-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="bd884-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="bd884-119">Тип фильтра целевого назначения, то есть исключить или включить.</span><span class="sxs-lookup"><span data-stu-id="bd884-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="bd884-120">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="bd884-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="bd884-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="bd884-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="bd884-122">groupId</span><span class="sxs-lookup"><span data-stu-id="bd884-122">groupId</span></span>|<span data-ttu-id="bd884-123">String</span><span class="sxs-lookup"><span data-stu-id="bd884-123">String</span></span>|<span data-ttu-id="bd884-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="bd884-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="bd884-125">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bd884-125">Inherited from [groupAssignmentTarget](../resources/intune-devices-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd884-126">Связи</span><span class="sxs-lookup"><span data-stu-id="bd884-126">Relationships</span></span>
<span data-ttu-id="bd884-127">Нет</span><span class="sxs-lookup"><span data-stu-id="bd884-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd884-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd884-128">JSON Representation</span></span>
<span data-ttu-id="bd884-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd884-129">Here is a JSON representation of the resource.</span></span>
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




