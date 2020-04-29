---
title: Тип ресурса deviceActionResult
description: Результат действия с устройством
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff9b34e6e84b8340e214f46f28ce7e243e72be5e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407045"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="9c9b2-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9c9b2-103">deviceActionResult resource type</span></span>

<span data-ttu-id="9c9b2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c9b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c9b2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c9b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c9b2-106">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="9c9b2-106">Device action result</span></span>

## <a name="properties"></a><span data-ttu-id="9c9b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c9b2-107">Properties</span></span>
|<span data-ttu-id="9c9b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c9b2-108">Property</span></span>|<span data-ttu-id="9c9b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9c9b2-109">Type</span></span>|<span data-ttu-id="9c9b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9c9b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c9b2-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9c9b2-111">actionName</span></span>|<span data-ttu-id="9c9b2-112">String</span><span class="sxs-lookup"><span data-stu-id="9c9b2-112">String</span></span>|<span data-ttu-id="9c9b2-113">Название действия</span><span class="sxs-lookup"><span data-stu-id="9c9b2-113">Action name</span></span>|
|<span data-ttu-id="9c9b2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9c9b2-114">actionState</span></span>|[<span data-ttu-id="9c9b2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9c9b2-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9c9b2-116">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="9c9b2-116">State of the action.</span></span> <span data-ttu-id="9c9b2-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9c9b2-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9c9b2-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9c9b2-118">startDateTime</span></span>|<span data-ttu-id="9c9b2-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c9b2-119">DateTimeOffset</span></span>|<span data-ttu-id="9c9b2-120">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="9c9b2-120">Time the action was initiated</span></span>|
|<span data-ttu-id="9c9b2-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c9b2-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9c9b2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c9b2-122">DateTimeOffset</span></span>|<span data-ttu-id="9c9b2-123">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="9c9b2-123">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c9b2-124">Связи</span><span class="sxs-lookup"><span data-stu-id="9c9b2-124">Relationships</span></span>
<span data-ttu-id="9c9b2-125">Нет</span><span class="sxs-lookup"><span data-stu-id="9c9b2-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c9b2-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c9b2-126">JSON Representation</span></span>
<span data-ttu-id="9c9b2-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c9b2-127">Here is a JSON representation of the resource.</span></span>
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







