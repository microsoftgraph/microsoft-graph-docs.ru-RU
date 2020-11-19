---
title: Тип ресурса allLicensedUsersAssignmentTarget
description: Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c9d799aeb602f1b06c7429e8c69483a238a059ad
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300880"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a><span data-ttu-id="38190-103">Тип ресурса allLicensedUsersAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="38190-103">allLicensedUsersAssignmentTarget resource type</span></span>

<span data-ttu-id="38190-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38190-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38190-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38190-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38190-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38190-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38190-107">Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.</span><span class="sxs-lookup"><span data-stu-id="38190-107">Represents an assignment to all licensed users in the tenant.</span></span>


<span data-ttu-id="38190-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="38190-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38190-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="38190-109">Properties</span></span>
|<span data-ttu-id="38190-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="38190-110">Property</span></span>|<span data-ttu-id="38190-111">Тип</span><span class="sxs-lookup"><span data-stu-id="38190-111">Type</span></span>|<span data-ttu-id="38190-112">Описание</span><span class="sxs-lookup"><span data-stu-id="38190-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38190-113">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="38190-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="38190-114">String</span><span class="sxs-lookup"><span data-stu-id="38190-114">String</span></span>|<span data-ttu-id="38190-115">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="38190-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="38190-116">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="38190-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="38190-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="38190-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="38190-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="38190-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="38190-119">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="38190-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="38190-120">Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="38190-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="38190-121">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="38190-121">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38190-122">Связи</span><span class="sxs-lookup"><span data-stu-id="38190-122">Relationships</span></span>
<span data-ttu-id="38190-123">Нет</span><span class="sxs-lookup"><span data-stu-id="38190-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38190-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38190-124">JSON Representation</span></span>
<span data-ttu-id="38190-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38190-125">Here is a JSON representation of the resource.</span></span>
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




