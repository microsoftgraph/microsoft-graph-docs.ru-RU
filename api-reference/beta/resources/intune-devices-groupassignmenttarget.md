---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 437d4c8ab11a0cf095e58b56b271aecb9e42729c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612326"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="fc2ff-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fc2ff-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="fc2ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc2ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc2ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc2ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2ff-107">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="fc2ff-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fc2ff-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc2ff-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc2ff-109">Properties</span></span>
|<span data-ttu-id="fc2ff-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc2ff-110">Property</span></span>|<span data-ttu-id="fc2ff-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fc2ff-111">Type</span></span>|<span data-ttu-id="fc2ff-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fc2ff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2ff-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="fc2ff-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="fc2ff-114">String</span><span class="sxs-lookup"><span data-stu-id="fc2ff-114">String</span></span>|<span data-ttu-id="fc2ff-115">Id фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="fc2ff-116">Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fc2ff-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="fc2ff-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="fc2ff-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="fc2ff-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="fc2ff-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="fc2ff-119">Тип фильтра целевого назначения, то есть исключить или включить.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="fc2ff-120">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="fc2ff-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="fc2ff-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="fc2ff-122">groupId</span><span class="sxs-lookup"><span data-stu-id="fc2ff-122">groupId</span></span>|<span data-ttu-id="fc2ff-123">String</span><span class="sxs-lookup"><span data-stu-id="fc2ff-123">String</span></span>|<span data-ttu-id="fc2ff-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc2ff-125">Связи</span><span class="sxs-lookup"><span data-stu-id="fc2ff-125">Relationships</span></span>
<span data-ttu-id="fc2ff-126">Нет</span><span class="sxs-lookup"><span data-stu-id="fc2ff-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc2ff-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc2ff-127">JSON Representation</span></span>
<span data-ttu-id="fc2ff-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc2ff-128">Here is a JSON representation of the resource.</span></span>
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




