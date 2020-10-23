---
title: Тип ресурса deviceAndAppManagementAssignmentTarget
description: Базовый тип для объектов назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3a4e45685acffb6523bfc7dc77cebbff4796530
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707586"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="2905b-103">Тип ресурса deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2905b-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="2905b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2905b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2905b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2905b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2905b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2905b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2905b-107">Базовый тип для объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="2905b-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="2905b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2905b-108">Properties</span></span>
|<span data-ttu-id="2905b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2905b-109">Property</span></span>|<span data-ttu-id="2905b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2905b-110">Type</span></span>|<span data-ttu-id="2905b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2905b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2905b-112">девицеандаппманажементассигнментфилтерид</span><span class="sxs-lookup"><span data-stu-id="2905b-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="2905b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2905b-113">String</span></span>|<span data-ttu-id="2905b-114">Идентификатор фильтра для назначения назначения.</span><span class="sxs-lookup"><span data-stu-id="2905b-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="2905b-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2905b-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="2905b-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="2905b-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="2905b-117">Тип фильтра целевого назначения, например, Exclude или include.</span><span class="sxs-lookup"><span data-stu-id="2905b-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="2905b-118">Возможные значения: `none`, `include`.</span><span class="sxs-lookup"><span data-stu-id="2905b-118">Possible values are: `none`, `include`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2905b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="2905b-119">Relationships</span></span>
<span data-ttu-id="2905b-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2905b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2905b-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2905b-121">JSON Representation</span></span>
<span data-ttu-id="2905b-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2905b-122">Here is a JSON representation of the resource.</span></span>
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





