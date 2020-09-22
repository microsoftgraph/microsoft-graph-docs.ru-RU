---
title: Тип ресурса allLicensedUsersAssignmentTarget
description: Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5289f6ff6205f58a998fe5e69c7d7f5a73b8480f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067253"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="3681c-103">Тип ресурса allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3681c-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="3681c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3681c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3681c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3681c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3681c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3681c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3681c-107">Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.</span><span class="sxs-lookup"><span data-stu-id="3681c-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="3681c-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3681c-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3681c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3681c-109">Properties</span></span>
|<span data-ttu-id="3681c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3681c-110">Property</span></span>|<span data-ttu-id="3681c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3681c-111">Type</span></span>|<span data-ttu-id="3681c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3681c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3681c-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="3681c-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="3681c-114">String</span><span class="sxs-lookup"><span data-stu-id="3681c-114">String</span></span>|<span data-ttu-id="3681c-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="3681c-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="3681c-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3681c-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="3681c-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3681c-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="3681c-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="3681c-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="3681c-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="3681c-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="3681c-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="3681c-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="3681c-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="3681c-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3681c-122">Связи</span><span class="sxs-lookup"><span data-stu-id="3681c-122">Relationships</span></span>
<span data-ttu-id="3681c-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3681c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3681c-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3681c-124">JSON Representation</span></span>
<span data-ttu-id="3681c-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3681c-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```






