---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ecb0028cd6e75d57f95868d16440881c4ac1bba4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030858"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="c9a75-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="c9a75-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="c9a75-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9a75-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9a75-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="c9a75-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="c9a75-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9a75-106">Properties</span></span>
|<span data-ttu-id="c9a75-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9a75-107">Property</span></span>|<span data-ttu-id="c9a75-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c9a75-108">Type</span></span>|<span data-ttu-id="c9a75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c9a75-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9a75-110">actionName</span><span class="sxs-lookup"><span data-stu-id="c9a75-110">actionName</span></span>|<span data-ttu-id="c9a75-111">String</span><span class="sxs-lookup"><span data-stu-id="c9a75-111">String</span></span>|<span data-ttu-id="c9a75-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="c9a75-112">Action name</span></span>|
|<span data-ttu-id="c9a75-113">actionState</span><span class="sxs-lookup"><span data-stu-id="c9a75-113">actionState</span></span>|[<span data-ttu-id="c9a75-114">actionState</span><span class="sxs-lookup"><span data-stu-id="c9a75-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="c9a75-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="c9a75-115">State of the action.</span></span> <span data-ttu-id="c9a75-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c9a75-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c9a75-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c9a75-117">startDateTime</span></span>|<span data-ttu-id="c9a75-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9a75-118">DateTimeOffset</span></span>|<span data-ttu-id="c9a75-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="c9a75-119">Time the action was initiated</span></span>|
|<span data-ttu-id="c9a75-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9a75-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="c9a75-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9a75-121">DateTimeOffset</span></span>|<span data-ttu-id="c9a75-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="c9a75-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9a75-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="c9a75-123">Relationships</span></span>
<span data-ttu-id="c9a75-124">Нет</span><span class="sxs-lookup"><span data-stu-id="c9a75-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9a75-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9a75-125">JSON Representation</span></span>
<span data-ttu-id="c9a75-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9a75-126">Here is a JSON representation of the resource.</span></span>
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



