---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52dcbfe4337fdc5993f6f2b9499244f87a10b953
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354023"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="1c6c4-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1c6c4-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="1c6c4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c6c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c6c4-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="1c6c4-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="1c6c4-106">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1c6c4-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c6c4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c6c4-107">Properties</span></span>
|<span data-ttu-id="1c6c4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c6c4-108">Property</span></span>|<span data-ttu-id="1c6c4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1c6c4-109">Type</span></span>|<span data-ttu-id="1c6c4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1c6c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c6c4-111">groupId</span><span class="sxs-lookup"><span data-stu-id="1c6c4-111">groupId</span></span>|<span data-ttu-id="1c6c4-112">String</span><span class="sxs-lookup"><span data-stu-id="1c6c4-112">String</span></span>|<span data-ttu-id="1c6c4-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="1c6c4-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="1c6c4-114">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="1c6c4-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c6c4-115">Связи</span><span class="sxs-lookup"><span data-stu-id="1c6c4-115">Relationships</span></span>
<span data-ttu-id="1c6c4-116">Нет</span><span class="sxs-lookup"><span data-stu-id="1c6c4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c6c4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c6c4-117">JSON Representation</span></span>
<span data-ttu-id="1c6c4-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c6c4-118">Here is a JSON representation of the resource.</span></span>
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




