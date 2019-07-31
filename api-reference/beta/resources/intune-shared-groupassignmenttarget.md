---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62de6a0a085fda974d9f8140aa2961e6a3610cb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967429"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="c1278-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c1278-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="c1278-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1278-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1278-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="c1278-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="c1278-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="c1278-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1278-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1278-108">Properties</span></span>
|<span data-ttu-id="c1278-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1278-109">Property</span></span>|<span data-ttu-id="c1278-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1278-110">Type</span></span>|<span data-ttu-id="c1278-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1278-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1278-112">groupId</span><span class="sxs-lookup"><span data-stu-id="c1278-112">groupId</span></span>|<span data-ttu-id="c1278-113">String</span><span class="sxs-lookup"><span data-stu-id="c1278-113">String</span></span>|<span data-ttu-id="c1278-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="c1278-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1278-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1278-115">Relationships</span></span>
<span data-ttu-id="c1278-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c1278-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1278-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1278-117">JSON Representation</span></span>
<span data-ttu-id="c1278-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1278-118">Here is a JSON representation of the resource.</span></span>
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





