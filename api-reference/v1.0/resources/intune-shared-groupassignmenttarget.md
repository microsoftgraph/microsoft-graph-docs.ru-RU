---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46297a1670136ffc1c7de07c4e4640121a50434
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967508"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="bfa57-103">Тип ресурса groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bfa57-103">groupAssignmentTarget resource type</span></span>

<span data-ttu-id="bfa57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfa57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bfa57-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfa57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa57-106">Представляет ресурс, назначенный группе.</span><span class="sxs-lookup"><span data-stu-id="bfa57-106">Represents an assignment to a group.</span></span>


<span data-ttu-id="bfa57-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="bfa57-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bfa57-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfa57-108">Properties</span></span>
|<span data-ttu-id="bfa57-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfa57-109">Property</span></span>|<span data-ttu-id="bfa57-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bfa57-110">Type</span></span>|<span data-ttu-id="bfa57-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bfa57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa57-112">groupId</span><span class="sxs-lookup"><span data-stu-id="bfa57-112">groupId</span></span>|<span data-ttu-id="bfa57-113">String</span><span class="sxs-lookup"><span data-stu-id="bfa57-113">String</span></span>|<span data-ttu-id="bfa57-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="bfa57-114">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfa57-115">Связи</span><span class="sxs-lookup"><span data-stu-id="bfa57-115">Relationships</span></span>
<span data-ttu-id="bfa57-116">Нет</span><span class="sxs-lookup"><span data-stu-id="bfa57-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfa57-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfa57-117">JSON Representation</span></span>
<span data-ttu-id="bfa57-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfa57-118">Here is a JSON representation of the resource.</span></span>
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









