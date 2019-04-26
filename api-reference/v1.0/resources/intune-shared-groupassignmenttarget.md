---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ac3c4519cc074c3cce423ca5d0745c8a78d865
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571921"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="d3206-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d3206-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d3206-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3206-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3206-105">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="d3206-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="d3206-106">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d3206-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3206-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3206-107">Properties</span></span>
|<span data-ttu-id="d3206-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3206-108">Property</span></span>|<span data-ttu-id="d3206-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d3206-109">Type</span></span>|<span data-ttu-id="d3206-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3206-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3206-111">groupId</span><span class="sxs-lookup"><span data-stu-id="d3206-111">groupId</span></span>|<span data-ttu-id="d3206-112">String</span><span class="sxs-lookup"><span data-stu-id="d3206-112">String</span></span>|<span data-ttu-id="d3206-113">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="d3206-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3206-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="d3206-114">Relationships</span></span>
<span data-ttu-id="d3206-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d3206-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3206-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3206-116">JSON Representation</span></span>
<span data-ttu-id="d3206-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3206-117">Here is a JSON representation of the resource.</span></span>
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



