---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: be8519adc44f7bb63379b0bfa821a067f3eee947
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985889"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="3fdde-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="3fdde-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="3fdde-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3fdde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fdde-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="3fdde-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="3fdde-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fdde-106">Properties</span></span>
|<span data-ttu-id="3fdde-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fdde-107">Property</span></span>|<span data-ttu-id="3fdde-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3fdde-108">Type</span></span>|<span data-ttu-id="3fdde-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3fdde-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fdde-110">actionName</span><span class="sxs-lookup"><span data-stu-id="3fdde-110">actionName</span></span>|<span data-ttu-id="3fdde-111">String</span><span class="sxs-lookup"><span data-stu-id="3fdde-111">String</span></span>|<span data-ttu-id="3fdde-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="3fdde-112">Action name</span></span>|
|<span data-ttu-id="3fdde-113">actionState</span><span class="sxs-lookup"><span data-stu-id="3fdde-113">actionState</span></span>|[<span data-ttu-id="3fdde-114">actionState</span><span class="sxs-lookup"><span data-stu-id="3fdde-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="3fdde-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="3fdde-115">State of the action.</span></span> <span data-ttu-id="3fdde-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="3fdde-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="3fdde-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3fdde-117">startDateTime</span></span>|<span data-ttu-id="3fdde-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fdde-118">DateTimeOffset</span></span>|<span data-ttu-id="3fdde-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="3fdde-119">Time the action was initiated</span></span>|
|<span data-ttu-id="3fdde-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fdde-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="3fdde-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fdde-121">DateTimeOffset</span></span>|<span data-ttu-id="3fdde-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="3fdde-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fdde-123">Связи</span><span class="sxs-lookup"><span data-stu-id="3fdde-123">Relationships</span></span>
<span data-ttu-id="3fdde-124">Нет</span><span class="sxs-lookup"><span data-stu-id="3fdde-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3fdde-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fdde-125">JSON Representation</span></span>
<span data-ttu-id="3fdde-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fdde-126">Here is a JSON representation of the resource.</span></span>
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



