---
title: тип ресурса configurationManagerCollectionAssignmentTarget
description: Представляет назначение коллекции диспетчера конфигурации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 28aa1e4e7fbb0d65a74f9a7b84bc48df19f3201c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752009"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="05dbe-103">тип ресурса configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="05dbe-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="05dbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05dbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="05dbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="05dbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05dbe-106">Представляет назначение коллекции диспетчера конфигурации.</span><span class="sxs-lookup"><span data-stu-id="05dbe-106">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="05dbe-107">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="05dbe-107">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05dbe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="05dbe-108">Properties</span></span>
|<span data-ttu-id="05dbe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="05dbe-109">Property</span></span>|<span data-ttu-id="05dbe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="05dbe-110">Type</span></span>|<span data-ttu-id="05dbe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05dbe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05dbe-112">collectionId</span><span class="sxs-lookup"><span data-stu-id="05dbe-112">collectionId</span></span>|<span data-ttu-id="05dbe-113">String</span><span class="sxs-lookup"><span data-stu-id="05dbe-113">String</span></span>|<span data-ttu-id="05dbe-114">Ид коллекции, который является объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="05dbe-114">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05dbe-115">Связи</span><span class="sxs-lookup"><span data-stu-id="05dbe-115">Relationships</span></span>
<span data-ttu-id="05dbe-116">Нет</span><span class="sxs-lookup"><span data-stu-id="05dbe-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05dbe-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05dbe-117">JSON Representation</span></span>
<span data-ttu-id="05dbe-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05dbe-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "collectionId": "String"
}
```




