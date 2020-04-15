---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4467c312581307a6603f5c83e4aa2e4e7fa1fa8b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445712"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="7be19-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7be19-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="7be19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be19-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7be19-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7be19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7be19-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="7be19-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="7be19-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7be19-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7be19-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7be19-108">Properties</span></span>
|<span data-ttu-id="7be19-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7be19-109">Property</span></span>|<span data-ttu-id="7be19-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7be19-110">Type</span></span>|<span data-ttu-id="7be19-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7be19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be19-112">groupId</span><span class="sxs-lookup"><span data-stu-id="7be19-112">groupId</span></span>|<span data-ttu-id="7be19-113">String</span><span class="sxs-lookup"><span data-stu-id="7be19-113">String</span></span>|<span data-ttu-id="7be19-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="7be19-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be19-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="7be19-115">Relationships</span></span>
<span data-ttu-id="7be19-116">Нет</span><span class="sxs-lookup"><span data-stu-id="7be19-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be19-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7be19-117">JSON Representation</span></span>
<span data-ttu-id="7be19-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7be19-118">Here is a JSON representation of the resource.</span></span>
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







