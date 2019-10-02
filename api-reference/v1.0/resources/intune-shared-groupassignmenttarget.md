---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7e4b97dd24c053af9aa65739e3c8a6db45044969
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354016"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="eb2ed-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="eb2ed-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="eb2ed-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eb2ed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb2ed-105">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="eb2ed-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="eb2ed-106">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="eb2ed-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb2ed-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb2ed-107">Properties</span></span>
|<span data-ttu-id="eb2ed-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb2ed-108">Property</span></span>|<span data-ttu-id="eb2ed-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eb2ed-109">Type</span></span>|<span data-ttu-id="eb2ed-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eb2ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb2ed-111">groupId</span><span class="sxs-lookup"><span data-stu-id="eb2ed-111">groupId</span></span>|<span data-ttu-id="eb2ed-112">String</span><span class="sxs-lookup"><span data-stu-id="eb2ed-112">String</span></span>|<span data-ttu-id="eb2ed-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="eb2ed-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb2ed-114">Связи</span><span class="sxs-lookup"><span data-stu-id="eb2ed-114">Relationships</span></span>
<span data-ttu-id="eb2ed-115">Нет</span><span class="sxs-lookup"><span data-stu-id="eb2ed-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb2ed-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb2ed-116">JSON Representation</span></span>
<span data-ttu-id="eb2ed-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb2ed-117">Here is a JSON representation of the resource.</span></span>
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




