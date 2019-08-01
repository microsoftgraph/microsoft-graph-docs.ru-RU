---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87e4e4707a1884e7d657bae9c6e41fee69dc831d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036920"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="a2317-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a2317-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="a2317-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a2317-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2317-105">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="a2317-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="a2317-106">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a2317-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2317-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a2317-107">Properties</span></span>
|<span data-ttu-id="a2317-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a2317-108">Property</span></span>|<span data-ttu-id="a2317-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a2317-109">Type</span></span>|<span data-ttu-id="a2317-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a2317-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2317-111">groupId</span><span class="sxs-lookup"><span data-stu-id="a2317-111">groupId</span></span>|<span data-ttu-id="a2317-112">String</span><span class="sxs-lookup"><span data-stu-id="a2317-112">String</span></span>|<span data-ttu-id="a2317-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="a2317-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2317-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="a2317-114">Relationships</span></span>
<span data-ttu-id="a2317-115">Нет</span><span class="sxs-lookup"><span data-stu-id="a2317-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2317-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a2317-116">JSON Representation</span></span>
<span data-ttu-id="a2317-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a2317-117">Here is a JSON representation of the resource.</span></span>
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



