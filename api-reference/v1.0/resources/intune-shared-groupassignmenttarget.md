---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f103315cc0c0499545a7fe3adb8bc31f9d24880
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447838"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="aa253-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aa253-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="aa253-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="aa253-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa253-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa253-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="aa253-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="aa253-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="aa253-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa253-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa253-108">Properties</span></span>
|<span data-ttu-id="aa253-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa253-109">Property</span></span>|<span data-ttu-id="aa253-110">Тип</span><span class="sxs-lookup"><span data-stu-id="aa253-110">Type</span></span>|<span data-ttu-id="aa253-111">Описание</span><span class="sxs-lookup"><span data-stu-id="aa253-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa253-112">groupId</span><span class="sxs-lookup"><span data-stu-id="aa253-112">groupId</span></span>|<span data-ttu-id="aa253-113">String</span><span class="sxs-lookup"><span data-stu-id="aa253-113">String</span></span>|<span data-ttu-id="aa253-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="aa253-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa253-115">Связи</span><span class="sxs-lookup"><span data-stu-id="aa253-115">Relationships</span></span>
<span data-ttu-id="aa253-116">Нет</span><span class="sxs-lookup"><span data-stu-id="aa253-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa253-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa253-117">JSON Representation</span></span>
<span data-ttu-id="aa253-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa253-118">Here is a JSON representation of the resource.</span></span>
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




