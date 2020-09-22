---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 759db547e2b1d33dbf8881cbd3ee5c5d5dfa3e4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091273"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="eeacf-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="eeacf-103">deviceActionResult resource type</span></span>

<span data-ttu-id="eeacf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eeacf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eeacf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eeacf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeacf-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="eeacf-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="eeacf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeacf-107">Properties</span></span>
|<span data-ttu-id="eeacf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeacf-108">Property</span></span>|<span data-ttu-id="eeacf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eeacf-109">Type</span></span>|<span data-ttu-id="eeacf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eeacf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeacf-111">actionName</span><span class="sxs-lookup"><span data-stu-id="eeacf-111">actionName</span></span>|<span data-ttu-id="eeacf-112">String</span><span class="sxs-lookup"><span data-stu-id="eeacf-112">String</span></span>|<span data-ttu-id="eeacf-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="eeacf-113">Action name</span></span>|
|<span data-ttu-id="eeacf-114">actionState</span><span class="sxs-lookup"><span data-stu-id="eeacf-114">actionState</span></span>|[<span data-ttu-id="eeacf-115">actionState</span><span class="sxs-lookup"><span data-stu-id="eeacf-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="eeacf-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="eeacf-116">State of the action.</span></span> <span data-ttu-id="eeacf-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="eeacf-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="eeacf-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="eeacf-118">startDateTime</span></span>|<span data-ttu-id="eeacf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeacf-119">DateTimeOffset</span></span>|<span data-ttu-id="eeacf-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="eeacf-120">Time the action was initiated</span></span>|
|<span data-ttu-id="eeacf-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeacf-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="eeacf-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeacf-122">DateTimeOffset</span></span>|<span data-ttu-id="eeacf-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="eeacf-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeacf-124">Связи</span><span class="sxs-lookup"><span data-stu-id="eeacf-124">Relationships</span></span>
<span data-ttu-id="eeacf-125">Нет</span><span class="sxs-lookup"><span data-stu-id="eeacf-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeacf-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeacf-126">JSON Representation</span></span>
<span data-ttu-id="eeacf-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeacf-127">Here is a JSON representation of the resource.</span></span>
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









