---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 93e271ff5628a6b5fc57333c5044bfce34376558
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938908"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="21bae-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="21bae-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="21bae-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bae-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bae-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="21bae-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="21bae-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="21bae-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21bae-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21bae-108">Properties</span></span>
|<span data-ttu-id="21bae-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21bae-109">Property</span></span>|<span data-ttu-id="21bae-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21bae-110">Type</span></span>|<span data-ttu-id="21bae-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21bae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bae-112">groupId</span><span class="sxs-lookup"><span data-stu-id="21bae-112">groupId</span></span>|<span data-ttu-id="21bae-113">String</span><span class="sxs-lookup"><span data-stu-id="21bae-113">String</span></span>|<span data-ttu-id="21bae-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="21bae-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="21bae-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="21bae-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="21bae-116">Связи</span><span class="sxs-lookup"><span data-stu-id="21bae-116">Relationships</span></span>
<span data-ttu-id="21bae-117">Нет</span><span class="sxs-lookup"><span data-stu-id="21bae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21bae-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21bae-118">JSON Representation</span></span>
<span data-ttu-id="21bae-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21bae-119">Here is a JSON representation of the resource.</span></span>
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




