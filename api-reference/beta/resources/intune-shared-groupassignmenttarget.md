---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70b53e52db8a2dba6f5c8b426e684957b2271d62
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735122"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="37ae5-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="37ae5-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="37ae5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37ae5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37ae5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37ae5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37ae5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37ae5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37ae5-107">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="37ae5-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="37ae5-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="37ae5-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37ae5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="37ae5-109">Properties</span></span>
|<span data-ttu-id="37ae5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="37ae5-110">Property</span></span>|<span data-ttu-id="37ae5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="37ae5-111">Type</span></span>|<span data-ttu-id="37ae5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="37ae5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37ae5-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="37ae5-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="37ae5-114">Строка</span><span class="sxs-lookup"><span data-stu-id="37ae5-114">String</span></span>|<span data-ttu-id="37ae5-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="37ae5-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="37ae5-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="37ae5-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="37ae5-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="37ae5-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="37ae5-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="37ae5-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="37ae5-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="37ae5-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="37ae5-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="37ae5-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="37ae5-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="37ae5-121">Possible values are: `none`, `include`.</span></span>|
|<span data-ttu-id="37ae5-122">groupId</span><span class="sxs-lookup"><span data-stu-id="37ae5-122">groupId</span></span>|<span data-ttu-id="37ae5-123">String</span><span class="sxs-lookup"><span data-stu-id="37ae5-123">String</span></span>|<span data-ttu-id="37ae5-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="37ae5-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37ae5-125">Связи</span><span class="sxs-lookup"><span data-stu-id="37ae5-125">Relationships</span></span>
<span data-ttu-id="37ae5-126">Нет</span><span class="sxs-lookup"><span data-stu-id="37ae5-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37ae5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37ae5-127">JSON Representation</span></span>
<span data-ttu-id="37ae5-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37ae5-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```





