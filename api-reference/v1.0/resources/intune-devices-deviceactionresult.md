---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 593df6737c83b46f560d983f031bfadc12fb18c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356991"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="5af11-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="5af11-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="5af11-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5af11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5af11-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="5af11-105">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="5af11-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5af11-106">Properties</span></span>
|<span data-ttu-id="5af11-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5af11-107">Property</span></span>|<span data-ttu-id="5af11-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5af11-108">Type</span></span>|<span data-ttu-id="5af11-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5af11-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af11-110">actionName</span><span class="sxs-lookup"><span data-stu-id="5af11-110">actionName</span></span>|<span data-ttu-id="5af11-111">String</span><span class="sxs-lookup"><span data-stu-id="5af11-111">String</span></span>|<span data-ttu-id="5af11-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="5af11-112">Action name</span></span>|
|<span data-ttu-id="5af11-113">actionState</span><span class="sxs-lookup"><span data-stu-id="5af11-113">actionState</span></span>|[<span data-ttu-id="5af11-114">actionState</span><span class="sxs-lookup"><span data-stu-id="5af11-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="5af11-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="5af11-115">State of the action.</span></span> <span data-ttu-id="5af11-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="5af11-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5af11-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="5af11-117">startDateTime</span></span>|<span data-ttu-id="5af11-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af11-118">DateTimeOffset</span></span>|<span data-ttu-id="5af11-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="5af11-119">Time the action was initiated</span></span>|
|<span data-ttu-id="5af11-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="5af11-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="5af11-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af11-121">DateTimeOffset</span></span>|<span data-ttu-id="5af11-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="5af11-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="5af11-123">Связи</span><span class="sxs-lookup"><span data-stu-id="5af11-123">Relationships</span></span>
<span data-ttu-id="5af11-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5af11-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5af11-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5af11-125">JSON Representation</span></span>
<span data-ttu-id="5af11-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5af11-126">Here is a JSON representation of the resource.</span></span>
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




