---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbd211bec428ff3a03ff989fa9ece36e5c55c561
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525252"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="8ab33-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ab33-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="8ab33-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ab33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ab33-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8ab33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ab33-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="8ab33-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="8ab33-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="8ab33-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ab33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ab33-108">Properties</span></span>
|<span data-ttu-id="8ab33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ab33-109">Property</span></span>|<span data-ttu-id="8ab33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8ab33-110">Type</span></span>|<span data-ttu-id="8ab33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8ab33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ab33-112">groupId</span><span class="sxs-lookup"><span data-stu-id="8ab33-112">groupId</span></span>|<span data-ttu-id="8ab33-113">String</span><span class="sxs-lookup"><span data-stu-id="8ab33-113">String</span></span>|<span data-ttu-id="8ab33-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="8ab33-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="8ab33-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="8ab33-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ab33-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="8ab33-116">Relationships</span></span>
<span data-ttu-id="8ab33-117">Нет</span><span class="sxs-lookup"><span data-stu-id="8ab33-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ab33-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ab33-118">JSON Representation</span></span>
<span data-ttu-id="8ab33-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ab33-119">Here is a JSON representation of the resource.</span></span>
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





