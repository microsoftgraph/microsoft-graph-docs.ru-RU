---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb7cd456b3a70bff2ea9d6e1de693d14f91205b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751260"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="11911-103">Тип ресурса exclusionGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="11911-103">exclusionGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="11911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11911-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11911-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11911-106">Представляет группу, которую следует исключить из назначения.</span><span class="sxs-lookup"><span data-stu-id="11911-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="11911-107">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="11911-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11911-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="11911-108">Properties</span></span>
|<span data-ttu-id="11911-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="11911-109">Property</span></span>|<span data-ttu-id="11911-110">Тип</span><span class="sxs-lookup"><span data-stu-id="11911-110">Type</span></span>|<span data-ttu-id="11911-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11911-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11911-112">groupId</span><span class="sxs-lookup"><span data-stu-id="11911-112">groupId</span></span>|<span data-ttu-id="11911-113">String</span><span class="sxs-lookup"><span data-stu-id="11911-113">String</span></span>|<span data-ttu-id="11911-114">Идентификатор группы-объекта назначения.</span><span class="sxs-lookup"><span data-stu-id="11911-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="11911-115">Наследуется от ресурса [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="11911-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="11911-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="11911-116">Relationships</span></span>
<span data-ttu-id="11911-117">Нет</span><span class="sxs-lookup"><span data-stu-id="11911-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11911-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11911-118">JSON Representation</span></span>
<span data-ttu-id="11911-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11911-119">Here is a JSON representation of the resource.</span></span>
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




