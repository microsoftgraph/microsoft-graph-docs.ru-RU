---
title: Тип ресурса allLicensedUsersAssignmentTarget
description: Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 68edbb68b250d7f653d3469f0d6b725a5d11aa62
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612302"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="21e64-103">Тип ресурса allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21e64-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="21e64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21e64-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21e64-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21e64-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21e64-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21e64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21e64-107">Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.</span><span class="sxs-lookup"><span data-stu-id="21e64-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="21e64-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="21e64-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21e64-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="21e64-109">Properties</span></span>
|<span data-ttu-id="21e64-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="21e64-110">Property</span></span>|<span data-ttu-id="21e64-111">Тип</span><span class="sxs-lookup"><span data-stu-id="21e64-111">Type</span></span>|<span data-ttu-id="21e64-112">Описание</span><span class="sxs-lookup"><span data-stu-id="21e64-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21e64-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="21e64-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="21e64-114">String</span><span class="sxs-lookup"><span data-stu-id="21e64-114">String</span></span>|<span data-ttu-id="21e64-115">Id фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="21e64-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="21e64-116">Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="21e64-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="21e64-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="21e64-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="21e64-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="21e64-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="21e64-119">Тип фильтра целевого назначения, то есть исключить или включить.</span><span class="sxs-lookup"><span data-stu-id="21e64-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="21e64-120">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="21e64-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="21e64-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="21e64-121">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21e64-122">Связи</span><span class="sxs-lookup"><span data-stu-id="21e64-122">Relationships</span></span>
<span data-ttu-id="21e64-123">Нет</span><span class="sxs-lookup"><span data-stu-id="21e64-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21e64-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21e64-124">JSON Representation</span></span>
<span data-ttu-id="21e64-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21e64-125">Here is a JSON representation of the resource.</span></span>
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




