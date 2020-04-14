---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c92cbad6b9c09de3dc8e468ddcec9d2035cb254
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43408054"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="9e07a-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9e07a-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="9e07a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e07a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e07a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e07a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e07a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9e07a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e07a-107">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="9e07a-107">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="9e07a-108">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9e07a-108">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e07a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e07a-109">Properties</span></span>
|<span data-ttu-id="9e07a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e07a-110">Property</span></span>|<span data-ttu-id="9e07a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9e07a-111">Type</span></span>|<span data-ttu-id="9e07a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9e07a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e07a-113">groupId</span><span class="sxs-lookup"><span data-stu-id="9e07a-113">groupId</span></span>|<span data-ttu-id="9e07a-114">String</span><span class="sxs-lookup"><span data-stu-id="9e07a-114">String</span></span>|<span data-ttu-id="9e07a-115">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="9e07a-115">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="9e07a-116">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="9e07a-116">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e07a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9e07a-117">Relationships</span></span>
<span data-ttu-id="9e07a-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9e07a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e07a-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e07a-119">JSON Representation</span></span>
<span data-ttu-id="9e07a-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e07a-120">Here is a JSON representation of the resource.</span></span>
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



