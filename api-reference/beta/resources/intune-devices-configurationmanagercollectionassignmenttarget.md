---
title: тип ресурса configurationManagerCollectionAssignmentTarget
description: Представляет назначение коллекции диспетчера конфигурации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb43c23a0eafaefea0b9265102880de58008f153
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610884"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a><span data-ttu-id="a54f1-103">тип ресурса configurationManagerCollectionAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a54f1-103">configurationManagerCollectionAssignmentTarget resource type</span></span>

<span data-ttu-id="a54f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a54f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a54f1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a54f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a54f1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a54f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a54f1-107">Представляет назначение коллекции диспетчера конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a54f1-107">Represents an assignment to a Configuration Manager Collection.</span></span>


<span data-ttu-id="a54f1-108">Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a54f1-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a54f1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a54f1-109">Properties</span></span>
|<span data-ttu-id="a54f1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a54f1-110">Property</span></span>|<span data-ttu-id="a54f1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a54f1-111">Type</span></span>|<span data-ttu-id="a54f1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a54f1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a54f1-113">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="a54f1-113">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="a54f1-114">String</span><span class="sxs-lookup"><span data-stu-id="a54f1-114">String</span></span>|<span data-ttu-id="a54f1-115">Id фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="a54f1-115">The Id of the filter for the target assignment.</span></span> <span data-ttu-id="a54f1-116">Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="a54f1-116">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)</span></span>|
|<span data-ttu-id="a54f1-117">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="a54f1-117">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="a54f1-118">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="a54f1-118">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="a54f1-119">Тип фильтра целевого назначения, то есть исключить или включить.</span><span class="sxs-lookup"><span data-stu-id="a54f1-119">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="a54f1-120">Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span><span class="sxs-lookup"><span data-stu-id="a54f1-120">Inherited from [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md).</span></span> <span data-ttu-id="a54f1-121">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="a54f1-121">Possible values are: `none`, `include`, `exclude`.</span></span>|
|<span data-ttu-id="a54f1-122">collectionId</span><span class="sxs-lookup"><span data-stu-id="a54f1-122">collectionId</span></span>|<span data-ttu-id="a54f1-123">String</span><span class="sxs-lookup"><span data-stu-id="a54f1-123">String</span></span>|<span data-ttu-id="a54f1-124">Ид коллекции, который является объектом назначения.</span><span class="sxs-lookup"><span data-stu-id="a54f1-124">The collection Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a54f1-125">Связи</span><span class="sxs-lookup"><span data-stu-id="a54f1-125">Relationships</span></span>
<span data-ttu-id="a54f1-126">Нет</span><span class="sxs-lookup"><span data-stu-id="a54f1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a54f1-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a54f1-127">JSON Representation</span></span>
<span data-ttu-id="a54f1-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a54f1-128">Here is a JSON representation of the resource.</span></span>
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




