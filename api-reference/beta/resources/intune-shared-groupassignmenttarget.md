---
title: Тип ресурса groupAssignmentTarget
description: Представляет назначение группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 68a276dc2a750db801b6f4ae893dbfc57ae66a97
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140308"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="daf14-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="daf14-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="daf14-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf14-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf14-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daf14-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf14-106">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="daf14-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="daf14-107">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="daf14-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="daf14-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="daf14-108">Properties</span></span>
|<span data-ttu-id="daf14-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="daf14-109">Property</span></span>|<span data-ttu-id="daf14-110">Тип</span><span class="sxs-lookup"><span data-stu-id="daf14-110">Type</span></span>|<span data-ttu-id="daf14-111">Описание</span><span class="sxs-lookup"><span data-stu-id="daf14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf14-112">groupId</span><span class="sxs-lookup"><span data-stu-id="daf14-112">groupId</span></span>|<span data-ttu-id="daf14-113">String</span><span class="sxs-lookup"><span data-stu-id="daf14-113">String</span></span>|<span data-ttu-id="daf14-114">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="daf14-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf14-115">Связи</span><span class="sxs-lookup"><span data-stu-id="daf14-115">Relationships</span></span>
<span data-ttu-id="daf14-116">Нет</span><span class="sxs-lookup"><span data-stu-id="daf14-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="daf14-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daf14-117">JSON Representation</span></span>
<span data-ttu-id="daf14-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daf14-118">Here is a JSON representation of the resource.</span></span>
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




