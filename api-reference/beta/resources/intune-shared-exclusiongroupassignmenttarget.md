---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0397a3f3def5be86b10f17e50617d488bf6a1512
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175397"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="24418-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="24418-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="24418-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24418-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24418-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24418-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24418-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="24418-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="24418-107">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="24418-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24418-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24418-108">Properties</span></span>
|<span data-ttu-id="24418-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="24418-109">Property</span></span>|<span data-ttu-id="24418-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24418-110">Type</span></span>|<span data-ttu-id="24418-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24418-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24418-112">groupId</span><span class="sxs-lookup"><span data-stu-id="24418-112">groupId</span></span>|<span data-ttu-id="24418-113">String</span><span class="sxs-lookup"><span data-stu-id="24418-113">String</span></span>|<span data-ttu-id="24418-114">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="24418-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="24418-115">Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="24418-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="24418-116">Связи</span><span class="sxs-lookup"><span data-stu-id="24418-116">Relationships</span></span>
<span data-ttu-id="24418-117">Нет</span><span class="sxs-lookup"><span data-stu-id="24418-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24418-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24418-118">JSON Representation</span></span>
<span data-ttu-id="24418-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24418-119">Here is a JSON representation of the resource.</span></span>
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




