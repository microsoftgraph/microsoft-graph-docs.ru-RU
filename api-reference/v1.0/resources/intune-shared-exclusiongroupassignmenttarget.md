---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3b0048cccfa9461bed2f1b25600b677512d45a47
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967515"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="77211-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="77211-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="77211-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77211-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77211-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77211-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77211-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="77211-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="77211-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="77211-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77211-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="77211-108">Properties</span></span>
|<span data-ttu-id="77211-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="77211-109">Property</span></span>|<span data-ttu-id="77211-110">Тип</span><span class="sxs-lookup"><span data-stu-id="77211-110">Type</span></span>|<span data-ttu-id="77211-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77211-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77211-112">groupId</span><span class="sxs-lookup"><span data-stu-id="77211-112">groupId</span></span>|<span data-ttu-id="77211-113">String</span><span class="sxs-lookup"><span data-stu-id="77211-113">String</span></span>|<span data-ttu-id="77211-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="77211-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="77211-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="77211-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="77211-116">Связи</span><span class="sxs-lookup"><span data-stu-id="77211-116">Relationships</span></span>
<span data-ttu-id="77211-117">Нет</span><span class="sxs-lookup"><span data-stu-id="77211-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77211-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77211-118">JSON Representation</span></span>
<span data-ttu-id="77211-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77211-119">Here is a JSON representation of the resource.</span></span>
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









