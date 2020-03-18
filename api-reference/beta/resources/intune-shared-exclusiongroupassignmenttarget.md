---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d2484d601de3c200cfe300a77245e873502ecc0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770125"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="70aa4-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="70aa4-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="70aa4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70aa4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70aa4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70aa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70aa4-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="70aa4-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="70aa4-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="70aa4-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70aa4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="70aa4-108">Properties</span></span>
|<span data-ttu-id="70aa4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="70aa4-109">Property</span></span>|<span data-ttu-id="70aa4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="70aa4-110">Type</span></span>|<span data-ttu-id="70aa4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="70aa4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70aa4-112">groupId</span><span class="sxs-lookup"><span data-stu-id="70aa4-112">groupId</span></span>|<span data-ttu-id="70aa4-113">String</span><span class="sxs-lookup"><span data-stu-id="70aa4-113">String</span></span>|<span data-ttu-id="70aa4-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="70aa4-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="70aa4-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="70aa4-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="70aa4-116">Связи</span><span class="sxs-lookup"><span data-stu-id="70aa4-116">Relationships</span></span>
<span data-ttu-id="70aa4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="70aa4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70aa4-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70aa4-118">JSON Representation</span></span>
<span data-ttu-id="70aa4-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70aa4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



