---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85da1976d4935e6cc8e2ca4d3d3e08e2ddd007ac
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770076"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="fa9fc-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fa9fc-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="fa9fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa9fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa9fc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fa9fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa9fc-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="fa9fc-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="fa9fc-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="fa9fc-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa9fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fa9fc-108">Properties</span></span>
|<span data-ttu-id="fa9fc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fa9fc-109">Property</span></span>|<span data-ttu-id="fa9fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fa9fc-110">Type</span></span>|<span data-ttu-id="fa9fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fa9fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa9fc-112">groupId</span><span class="sxs-lookup"><span data-stu-id="fa9fc-112">groupId</span></span>|<span data-ttu-id="fa9fc-113">String</span><span class="sxs-lookup"><span data-stu-id="fa9fc-113">String</span></span>|<span data-ttu-id="fa9fc-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="fa9fc-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa9fc-115">Связи</span><span class="sxs-lookup"><span data-stu-id="fa9fc-115">Relationships</span></span>
<span data-ttu-id="fa9fc-116">Нет</span><span class="sxs-lookup"><span data-stu-id="fa9fc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa9fc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fa9fc-117">JSON Representation</span></span>
<span data-ttu-id="fa9fc-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa9fc-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



