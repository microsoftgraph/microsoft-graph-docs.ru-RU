---
title: Тип ресурса groupAssignmentTarget
description: Представляет назначение группе.
ms.openlocfilehash: 0ebb41b1f737a20a37d322bac7ab5ae6ab2a248f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026658"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="78178-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="78178-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="78178-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="78178-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78178-105">Представляет назначение группе.</span><span class="sxs-lookup"><span data-stu-id="78178-105">Represents an assignment to a group.</span></span>

<span data-ttu-id="78178-106">Наследуется от типа [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="78178-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78178-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="78178-107">Properties</span></span>
|<span data-ttu-id="78178-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="78178-108">Property</span></span>|<span data-ttu-id="78178-109">Тип</span><span class="sxs-lookup"><span data-stu-id="78178-109">Type</span></span>|<span data-ttu-id="78178-110">Описание</span><span class="sxs-lookup"><span data-stu-id="78178-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78178-111">groupId</span><span class="sxs-lookup"><span data-stu-id="78178-111">groupId</span></span>|<span data-ttu-id="78178-112">String</span><span class="sxs-lookup"><span data-stu-id="78178-112">String</span></span>|<span data-ttu-id="78178-113">ИД группы, являющейся объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="78178-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78178-114">Связи</span><span class="sxs-lookup"><span data-stu-id="78178-114">Relationships</span></span>
<span data-ttu-id="78178-115">Нет</span><span class="sxs-lookup"><span data-stu-id="78178-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="78178-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78178-116">JSON Representation</span></span>
<span data-ttu-id="78178-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78178-117">Here is a JSON representation of the resource.</span></span>
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



