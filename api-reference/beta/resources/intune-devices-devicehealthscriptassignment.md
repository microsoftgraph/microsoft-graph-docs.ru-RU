---
title: Тип ресурса Девицехеалсскриптассигнмент
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a37d36fd5b36384d62ef656b9d36a7ed870e3586
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539094"
---
# <a name="devicehealthscriptassignment-resource-type"></a><span data-ttu-id="27995-103">Тип ресурса Девицехеалсскриптассигнмент</span><span class="sxs-lookup"><span data-stu-id="27995-103">deviceHealthScriptAssignment resource type</span></span>

> <span data-ttu-id="27995-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27995-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27995-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27995-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27995-106">Содержит свойства, используемые для назначения скрипта управления устройствами группе.</span><span class="sxs-lookup"><span data-stu-id="27995-106">Contains properties used to assign a device management script to a group.</span></span>

## <a name="methods"></a><span data-ttu-id="27995-107">Методы</span><span class="sxs-lookup"><span data-stu-id="27995-107">Methods</span></span>
|<span data-ttu-id="27995-108">Метод</span><span class="sxs-lookup"><span data-stu-id="27995-108">Method</span></span>|<span data-ttu-id="27995-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="27995-109">Return Type</span></span>|<span data-ttu-id="27995-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27995-110">Description</span></span>|
|:---|:---|:---|
<span data-ttu-id="27995-111">Нет</span><span class="sxs-lookup"><span data-stu-id="27995-111">None</span></span>

## <a name="properties"></a><span data-ttu-id="27995-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="27995-112">Properties</span></span>
|<span data-ttu-id="27995-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="27995-113">Property</span></span>|<span data-ttu-id="27995-114">Тип</span><span class="sxs-lookup"><span data-stu-id="27995-114">Type</span></span>|<span data-ttu-id="27995-115">Описание</span><span class="sxs-lookup"><span data-stu-id="27995-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27995-116">id</span><span class="sxs-lookup"><span data-stu-id="27995-116">id</span></span>|<span data-ttu-id="27995-117">String</span><span class="sxs-lookup"><span data-stu-id="27995-117">String</span></span>|<span data-ttu-id="27995-118">Ключ объекта назначения сценария работоспособности устройства</span><span class="sxs-lookup"><span data-stu-id="27995-118">Key of the device health script assignment entity</span></span>|
|<span data-ttu-id="27995-119">target</span><span class="sxs-lookup"><span data-stu-id="27995-119">target</span></span>|[<span data-ttu-id="27995-120">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="27995-120">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="27995-121">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="27995-121">The Azure Active Directory group we are targeting the script to</span></span>|
|<span data-ttu-id="27995-122">рунремедиатионскрипт</span><span class="sxs-lookup"><span data-stu-id="27995-122">runRemediationScript</span></span>|<span data-ttu-id="27995-123">Логический</span><span class="sxs-lookup"><span data-stu-id="27995-123">Boolean</span></span>|<span data-ttu-id="27995-124">Определите, нужно ли выполнять сценарий обнаружения или сценарий обнаружения и устранения неполадок.</span><span class="sxs-lookup"><span data-stu-id="27995-124">Determine whether we want to run detection script only or run both detection script and remediation script</span></span>|
|<span data-ttu-id="27995-125">runSchedule</span><span class="sxs-lookup"><span data-stu-id="27995-125">runSchedule</span></span>|[<span data-ttu-id="27995-126">runSchedule</span><span class="sxs-lookup"><span data-stu-id="27995-126">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="27995-127">Группа Azure Active Directory, на которую мы нацелены на скрипт</span><span class="sxs-lookup"><span data-stu-id="27995-127">The Azure Active Directory group we are targeting the script to</span></span>|

## <a name="relationships"></a><span data-ttu-id="27995-128">Связи</span><span class="sxs-lookup"><span data-stu-id="27995-128">Relationships</span></span>
<span data-ttu-id="27995-129">Нет</span><span class="sxs-lookup"><span data-stu-id="27995-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27995-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27995-130">JSON Representation</span></span>
<span data-ttu-id="27995-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27995-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
      "@odata.type": "microsoft.graph.runSchedule"
  }
}
```



