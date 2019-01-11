---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1b802d1b09fbe65e9e1e72e4c34a387462e12113
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861126"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="19f79-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="19f79-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="19f79-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19f79-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19f79-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="19f79-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="19f79-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="19f79-106">Properties</span></span>
|<span data-ttu-id="19f79-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="19f79-107">Property</span></span>|<span data-ttu-id="19f79-108">Тип</span><span class="sxs-lookup"><span data-stu-id="19f79-108">Type</span></span>|<span data-ttu-id="19f79-109">Описание</span><span class="sxs-lookup"><span data-stu-id="19f79-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19f79-110">actionName</span><span class="sxs-lookup"><span data-stu-id="19f79-110">actionName</span></span>|<span data-ttu-id="19f79-111">String</span><span class="sxs-lookup"><span data-stu-id="19f79-111">String</span></span>|<span data-ttu-id="19f79-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="19f79-112">Action name</span></span>|
|<span data-ttu-id="19f79-113">actionState</span><span class="sxs-lookup"><span data-stu-id="19f79-113">actionState</span></span>|[<span data-ttu-id="19f79-114">actionState</span><span class="sxs-lookup"><span data-stu-id="19f79-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="19f79-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="19f79-115">State of the action.</span></span> <span data-ttu-id="19f79-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="19f79-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="19f79-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="19f79-117">startDateTime</span></span>|<span data-ttu-id="19f79-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19f79-118">DateTimeOffset</span></span>|<span data-ttu-id="19f79-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="19f79-119">Time the action was initiated</span></span>|
|<span data-ttu-id="19f79-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="19f79-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="19f79-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19f79-121">DateTimeOffset</span></span>|<span data-ttu-id="19f79-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="19f79-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="19f79-123">Связи</span><span class="sxs-lookup"><span data-stu-id="19f79-123">Relationships</span></span>
<span data-ttu-id="19f79-124">Нет</span><span class="sxs-lookup"><span data-stu-id="19f79-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19f79-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19f79-125">JSON Representation</span></span>
<span data-ttu-id="19f79-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19f79-126">Here is a JSON representation of the resource.</span></span>
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



