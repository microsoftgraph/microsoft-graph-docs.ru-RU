---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 805f2f1dbcab8751d564fbde3f6747b6e77f6d09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036927"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="3ec06-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="3ec06-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="3ec06-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ec06-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ec06-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="3ec06-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="3ec06-106">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3ec06-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ec06-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ec06-107">Properties</span></span>
|<span data-ttu-id="3ec06-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ec06-108">Property</span></span>|<span data-ttu-id="3ec06-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3ec06-109">Type</span></span>|<span data-ttu-id="3ec06-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3ec06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ec06-111">groupId</span><span class="sxs-lookup"><span data-stu-id="3ec06-111">groupId</span></span>|<span data-ttu-id="3ec06-112">String</span><span class="sxs-lookup"><span data-stu-id="3ec06-112">String</span></span>|<span data-ttu-id="3ec06-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="3ec06-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="3ec06-114">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3ec06-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ec06-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ec06-115">Relationships</span></span>
<span data-ttu-id="3ec06-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3ec06-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ec06-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ec06-117">JSON Representation</span></span>
<span data-ttu-id="3ec06-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ec06-118">Here is a JSON representation of the resource.</span></span>
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



