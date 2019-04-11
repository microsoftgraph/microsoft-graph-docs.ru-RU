---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d67b7789f30dd1226c7918e734d615db4ee83ac
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773296"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="b0b49-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0b49-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b0b49-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0b49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0b49-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0b49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0b49-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="b0b49-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="b0b49-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="b0b49-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0b49-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0b49-108">Properties</span></span>
|<span data-ttu-id="b0b49-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0b49-109">Property</span></span>|<span data-ttu-id="b0b49-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0b49-110">Type</span></span>|<span data-ttu-id="b0b49-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0b49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0b49-112">groupId</span><span class="sxs-lookup"><span data-stu-id="b0b49-112">groupId</span></span>|<span data-ttu-id="b0b49-113">String</span><span class="sxs-lookup"><span data-stu-id="b0b49-113">String</span></span>|<span data-ttu-id="b0b49-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="b0b49-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0b49-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="b0b49-115">Relationships</span></span>
<span data-ttu-id="b0b49-116">Нет</span><span class="sxs-lookup"><span data-stu-id="b0b49-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0b49-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0b49-117">JSON Representation</span></span>
<span data-ttu-id="b0b49-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0b49-118">Here is a JSON representation of the resource.</span></span>
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





