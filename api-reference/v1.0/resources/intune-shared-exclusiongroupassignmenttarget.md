---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523765"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="46366-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="46366-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="46366-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46366-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46366-105">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="46366-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="46366-106">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="46366-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="46366-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="46366-107">Properties</span></span>
|<span data-ttu-id="46366-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="46366-108">Property</span></span>|<span data-ttu-id="46366-109">Тип</span><span class="sxs-lookup"><span data-stu-id="46366-109">Type</span></span>|<span data-ttu-id="46366-110">Описание</span><span class="sxs-lookup"><span data-stu-id="46366-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46366-111">groupId</span><span class="sxs-lookup"><span data-stu-id="46366-111">groupId</span></span>|<span data-ttu-id="46366-112">String</span><span class="sxs-lookup"><span data-stu-id="46366-112">String</span></span>|<span data-ttu-id="46366-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="46366-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="46366-114">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="46366-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="46366-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="46366-115">Relationships</span></span>
<span data-ttu-id="46366-116">Нет</span><span class="sxs-lookup"><span data-stu-id="46366-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46366-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46366-117">JSON Representation</span></span>
<span data-ttu-id="46366-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46366-118">Here is a JSON representation of the resource.</span></span>
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



