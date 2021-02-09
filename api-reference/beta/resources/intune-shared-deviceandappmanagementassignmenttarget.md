---
title: Тип ресурса deviceAndAppManagementAssignmentTarget
description: Базовый тип для объектов назначения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ec96f18f16a40182bccfc00efbe70c84568fae33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158095"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a><span data-ttu-id="32654-103">Тип ресурса deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="32654-103">deviceAndAppManagementAssignmentTarget resource type</span></span>

<span data-ttu-id="32654-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="32654-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32654-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32654-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="32654-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32654-107">Базовый тип для объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="32654-107">Base type for assignment targets.</span></span>

## <a name="properties"></a><span data-ttu-id="32654-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="32654-108">Properties</span></span>
|<span data-ttu-id="32654-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="32654-109">Property</span></span>|<span data-ttu-id="32654-110">Тип</span><span class="sxs-lookup"><span data-stu-id="32654-110">Type</span></span>|<span data-ttu-id="32654-111">Описание</span><span class="sxs-lookup"><span data-stu-id="32654-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32654-112">deviceAndAppManagementAssignmentFilterId</span><span class="sxs-lookup"><span data-stu-id="32654-112">deviceAndAppManagementAssignmentFilterId</span></span>|<span data-ttu-id="32654-113">String</span><span class="sxs-lookup"><span data-stu-id="32654-113">String</span></span>|<span data-ttu-id="32654-114">ИД фильтра для целевого назначения.</span><span class="sxs-lookup"><span data-stu-id="32654-114">The Id of the filter for the target assignment.</span></span>|
|<span data-ttu-id="32654-115">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="32654-115">deviceAndAppManagementAssignmentFilterType</span></span>|[<span data-ttu-id="32654-116">deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="32654-116">deviceAndAppManagementAssignmentFilterType</span></span>](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|<span data-ttu-id="32654-117">Тип фильтра целевого назначения, например "Исключить" или "Включить".</span><span class="sxs-lookup"><span data-stu-id="32654-117">The type of filter of the target assignment i.e. Exclude or Include.</span></span> <span data-ttu-id="32654-118">Возможные значения: `none`, `include`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="32654-118">Possible values are: `none`, `include`, `exclude`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32654-119">Связи</span><span class="sxs-lookup"><span data-stu-id="32654-119">Relationships</span></span>
<span data-ttu-id="32654-120">Нет</span><span class="sxs-lookup"><span data-stu-id="32654-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32654-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="32654-121">JSON Representation</span></span>
<span data-ttu-id="32654-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32654-122">Here is a JSON representation of the resource.</span></span>
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




