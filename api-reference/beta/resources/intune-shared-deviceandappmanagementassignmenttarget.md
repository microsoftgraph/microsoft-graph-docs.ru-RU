---
title: Тип ресурса deviceAndAppManagementAssignmentTarget
description: Базовый тип для объектов назначения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4194d5afb7f7c90f658c558d8609badef2d89cfc
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793495"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="cd1ff-103">Тип ресурса deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cd1ff-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="cd1ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd1ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd1ff-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd1ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd1ff-107">Базовый тип для объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="cd1ff-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd1ff-108">Properties</span></span>
|<span data-ttu-id="cd1ff-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd1ff-109">Property</span></span>|<span data-ttu-id="cd1ff-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cd1ff-110">Type</span></span>|<span data-ttu-id="cd1ff-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cd1ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd1ff-112">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="cd1ff-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="cd1ff-113">String</span><span class="sxs-lookup"><span data-stu-id="cd1ff-113">String</span></span>|<span data-ttu-id="cd1ff-114">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="cd1ff-115">девицеандаппманажементассигнментфилтертипе</span><span class="sxs-lookup"><span data-stu-id="cd1ff-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="cd1ff-116">девицеандаппманажементассигнментфилтертипе</span><span class="sxs-lookup"><span data-stu-id="cd1ff-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="cd1ff-117">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="cd1ff-118">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-118">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd1ff-119">Связи</span><span class="sxs-lookup"><span data-stu-id="cd1ff-119">Relationships</span></span>
<span data-ttu-id="cd1ff-120">Нет</span><span class="sxs-lookup"><span data-stu-id="cd1ff-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd1ff-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd1ff-121">JSON Representation</span></span>
<span data-ttu-id="cd1ff-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd1ff-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```



