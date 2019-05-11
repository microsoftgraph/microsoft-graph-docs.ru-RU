---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e33b91b2fdd4b17ebfeef61a2e6917d24edf589d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942131"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="590ef-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="590ef-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="590ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="590ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="590ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="590ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="590ef-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="590ef-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="590ef-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="590ef-107">Properties</span></span>
|<span data-ttu-id="590ef-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="590ef-108">Property</span></span>|<span data-ttu-id="590ef-109">Тип</span><span class="sxs-lookup"><span data-stu-id="590ef-109">Type</span></span>|<span data-ttu-id="590ef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="590ef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="590ef-111">actionName</span><span class="sxs-lookup"><span data-stu-id="590ef-111">actionName</span></span>|<span data-ttu-id="590ef-112">String</span><span class="sxs-lookup"><span data-stu-id="590ef-112">String</span></span>|<span data-ttu-id="590ef-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="590ef-113">Action name</span></span>|
|<span data-ttu-id="590ef-114">actionState</span><span class="sxs-lookup"><span data-stu-id="590ef-114">actionState</span></span>|[<span data-ttu-id="590ef-115">actionState</span><span class="sxs-lookup"><span data-stu-id="590ef-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="590ef-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="590ef-116">State of the action.</span></span> <span data-ttu-id="590ef-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="590ef-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="590ef-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="590ef-118">startDateTime</span></span>|<span data-ttu-id="590ef-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590ef-119">DateTimeOffset</span></span>|<span data-ttu-id="590ef-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="590ef-120">Time the action was initiated</span></span>|
|<span data-ttu-id="590ef-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="590ef-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="590ef-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="590ef-122">DateTimeOffset</span></span>|<span data-ttu-id="590ef-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="590ef-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="590ef-124">Связи</span><span class="sxs-lookup"><span data-stu-id="590ef-124">Relationships</span></span>
<span data-ttu-id="590ef-125">Нет</span><span class="sxs-lookup"><span data-stu-id="590ef-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="590ef-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="590ef-126">JSON Representation</span></span>
<span data-ttu-id="590ef-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="590ef-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```




