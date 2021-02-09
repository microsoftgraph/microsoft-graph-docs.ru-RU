---
title: Тип ресурса configurationManagerCollectionAssignmentTarget
description: Представляет назначение коллекции Configuration Manager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d32813e7c5c7cdae889406d694f686630311166
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161012"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="ff0b3-103">Тип ресурса configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ff0b3-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="ff0b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff0b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff0b3-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff0b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff0b3-107">Представляет назначение коллекции Configuration Manager.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-107">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="ff0b3-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ff0b3-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff0b3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff0b3-109">Properties</span></span>
|<span data-ttu-id="ff0b3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff0b3-110">Property</span></span>|<span data-ttu-id="ff0b3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ff0b3-111">Type</span></span>|<span data-ttu-id="ff0b3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ff0b3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff0b3-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="ff0b3-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="ff0b3-114">String</span><span class="sxs-lookup"><span data-stu-id="ff0b3-114">String</span></span>|<span data-ttu-id="ff0b3-115">ИД фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="ff0b3-116">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ff0b3-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="ff0b3-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ff0b3-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="ff0b3-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="ff0b3-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="ff0b3-119">Тип фильтра целевого назначения, например Exclude или Include.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="ff0b3-120">Наследуется [от deviceAndAppManagementAssignmentTarget.](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="ff0b3-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="ff0b3-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="ff0b3-122">collectionId</span><span class="sxs-lookup"><span data-stu-id="ff0b3-122">collectionId</span></span>|<span data-ttu-id="ff0b3-123">String</span><span class="sxs-lookup"><span data-stu-id="ff0b3-123">String</span></span>|<span data-ttu-id="ff0b3-124">ИД коллекции, которая является целевым объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-124">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff0b3-125">Связи</span><span class="sxs-lookup"><span data-stu-id="ff0b3-125">Relationships</span></span>
<span data-ttu-id="ff0b3-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ff0b3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0b3-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff0b3-127">JSON Representation</span></span>
<span data-ttu-id="ff0b3-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff0b3-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "collectionId": "String"
}
```




