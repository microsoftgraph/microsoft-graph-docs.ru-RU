---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2926f127bdf018333135a60c92d2b4a93e17530b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159509"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="4444f-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4444f-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="4444f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4444f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4444f-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4444f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4444f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4444f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4444f-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="4444f-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="4444f-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4444f-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4444f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4444f-109">Properties</span></span>
|<span data-ttu-id="4444f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4444f-110">Property</span></span>|<span data-ttu-id="4444f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4444f-111">Type</span></span>|<span data-ttu-id="4444f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4444f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4444f-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="4444f-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="4444f-114">String</span><span class="sxs-lookup"><span data-stu-id="4444f-114">String</span></span>|<span data-ttu-id="4444f-115">ИД фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="4444f-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="4444f-116">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4444f-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="4444f-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="4444f-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="4444f-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="4444f-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="4444f-119">Тип фильтра целевого назначения, например Exclude или Include.</span><span class="sxs-lookup"><span data-stu-id="4444f-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="4444f-120">Наследуется [от deviceAndAppManagementAssignmentTarget.](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4444f-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="4444f-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="4444f-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="4444f-122">groupId</span><span class="sxs-lookup"><span data-stu-id="4444f-122">groupId</span></span>|<span data-ttu-id="4444f-123">String</span><span class="sxs-lookup"><span data-stu-id="4444f-123">String</span></span>|<span data-ttu-id="4444f-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="4444f-124">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="4444f-125">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4444f-125">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4444f-126">Связи</span><span class="sxs-lookup"><span data-stu-id="4444f-126">Relationships</span></span>
<span data-ttu-id="4444f-127">Нет</span><span class="sxs-lookup"><span data-stu-id="4444f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4444f-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4444f-128">JSON Representation</span></span>
<span data-ttu-id="4444f-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4444f-129">Here is a JSON representation of the resource.</span></span>
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




