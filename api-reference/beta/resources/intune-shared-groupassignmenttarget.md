---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8e624d7b3abcc8cc7472604883887bc960c1895f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348041"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="db7f6-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="db7f6-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="db7f6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db7f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db7f6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db7f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db7f6-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="db7f6-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="db7f6-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="db7f6-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db7f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="db7f6-108">Properties</span></span>
|<span data-ttu-id="db7f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="db7f6-109">Property</span></span>|<span data-ttu-id="db7f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="db7f6-110">Type</span></span>|<span data-ttu-id="db7f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db7f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db7f6-112">groupId</span><span class="sxs-lookup"><span data-stu-id="db7f6-112">groupId</span></span>|<span data-ttu-id="db7f6-113">String</span><span class="sxs-lookup"><span data-stu-id="db7f6-113">String</span></span>|<span data-ttu-id="db7f6-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="db7f6-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db7f6-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="db7f6-115">Relationships</span></span>
<span data-ttu-id="db7f6-116">Нет</span><span class="sxs-lookup"><span data-stu-id="db7f6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db7f6-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db7f6-117">JSON Representation</span></span>
<span data-ttu-id="db7f6-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db7f6-118">Here is a JSON representation of the resource.</span></span>
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



