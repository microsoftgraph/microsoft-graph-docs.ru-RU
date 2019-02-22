---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c435241056f5e29166355829d1c40438b525a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151431"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="7aa32-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="7aa32-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="7aa32-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7aa32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7aa32-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7aa32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aa32-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="7aa32-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="7aa32-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7aa32-107">Properties</span></span>
|<span data-ttu-id="7aa32-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7aa32-108">Property</span></span>|<span data-ttu-id="7aa32-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7aa32-109">Type</span></span>|<span data-ttu-id="7aa32-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aa32-111">actionName</span><span class="sxs-lookup"><span data-stu-id="7aa32-111">actionName</span></span>|<span data-ttu-id="7aa32-112">String</span><span class="sxs-lookup"><span data-stu-id="7aa32-112">String</span></span>|<span data-ttu-id="7aa32-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="7aa32-113">Action name</span></span>|
|<span data-ttu-id="7aa32-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7aa32-114">actionState</span></span>|[<span data-ttu-id="7aa32-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7aa32-115">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="7aa32-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="7aa32-116">State of the action.</span></span> <span data-ttu-id="7aa32-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7aa32-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7aa32-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa32-118">startDateTime</span></span>|<span data-ttu-id="7aa32-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa32-119">DateTimeOffset</span></span>|<span data-ttu-id="7aa32-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="7aa32-120">Time the action was initiated</span></span>|
|<span data-ttu-id="7aa32-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7aa32-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="7aa32-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aa32-122">DateTimeOffset</span></span>|<span data-ttu-id="7aa32-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="7aa32-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="7aa32-124">Связи</span><span class="sxs-lookup"><span data-stu-id="7aa32-124">Relationships</span></span>
<span data-ttu-id="7aa32-125">Нет</span><span class="sxs-lookup"><span data-stu-id="7aa32-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aa32-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7aa32-126">JSON Representation</span></span>
<span data-ttu-id="7aa32-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7aa32-127">Here is a JSON representation of the resource.</span></span>
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




