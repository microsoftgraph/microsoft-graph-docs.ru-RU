---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0dda74257a3596ad72470806cdcc4f169fd935d9
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157514"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="1f32a-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1f32a-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="1f32a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f32a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f32a-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f32a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f32a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f32a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f32a-107">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="1f32a-107">Represents an assignment to a group.</span></span>


<span data-ttu-id="1f32a-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1f32a-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f32a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f32a-109">Properties</span></span>
|<span data-ttu-id="1f32a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f32a-110">Property</span></span>|<span data-ttu-id="1f32a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1f32a-111">Type</span></span>|<span data-ttu-id="1f32a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1f32a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f32a-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="1f32a-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="1f32a-114">String</span><span class="sxs-lookup"><span data-stu-id="1f32a-114">String</span></span>|<span data-ttu-id="1f32a-115">ИД фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="1f32a-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="1f32a-116">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1f32a-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="1f32a-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1f32a-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="1f32a-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="1f32a-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="1f32a-119">Тип фильтра целевого назначения, например "Исключить" или "Включить".</span><span class="sxs-lookup"><span data-stu-id="1f32a-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="1f32a-120">Наследуется [от deviceAndAppManagementAssignmentTarget.](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1f32a-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="1f32a-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="1f32a-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="1f32a-122">groupId</span><span class="sxs-lookup"><span data-stu-id="1f32a-122">groupId</span></span>|<span data-ttu-id="1f32a-123">String</span><span class="sxs-lookup"><span data-stu-id="1f32a-123">String</span></span>|<span data-ttu-id="1f32a-124">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="1f32a-124">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f32a-125">Связи</span><span class="sxs-lookup"><span data-stu-id="1f32a-125">Relationships</span></span>
<span data-ttu-id="1f32a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1f32a-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f32a-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f32a-127">JSON Representation</span></span>
<span data-ttu-id="1f32a-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f32a-128">Here is a JSON representation of the resource.</span></span>
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




