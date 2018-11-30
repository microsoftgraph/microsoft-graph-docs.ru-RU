---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
ms.openlocfilehash: 9d7804b994474778f0f06c52079e09ed5887a09f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027202"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="f33b2-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="f33b2-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="f33b2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f33b2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f33b2-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="f33b2-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="f33b2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f33b2-106">Properties</span></span>
|<span data-ttu-id="f33b2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f33b2-107">Property</span></span>|<span data-ttu-id="f33b2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f33b2-108">Type</span></span>|<span data-ttu-id="f33b2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f33b2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f33b2-110">actionName</span><span class="sxs-lookup"><span data-stu-id="f33b2-110">actionName</span></span>|<span data-ttu-id="f33b2-111">String</span><span class="sxs-lookup"><span data-stu-id="f33b2-111">String</span></span>|<span data-ttu-id="f33b2-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="f33b2-112">Action name</span></span>|
|<span data-ttu-id="f33b2-113">actionState</span><span class="sxs-lookup"><span data-stu-id="f33b2-113">actionState</span></span>|[<span data-ttu-id="f33b2-114">actionState</span><span class="sxs-lookup"><span data-stu-id="f33b2-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="f33b2-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="f33b2-115">State of the action.</span></span> <span data-ttu-id="f33b2-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f33b2-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f33b2-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f33b2-117">startDateTime</span></span>|<span data-ttu-id="f33b2-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f33b2-118">DateTimeOffset</span></span>|<span data-ttu-id="f33b2-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="f33b2-119">Time the action was initiated</span></span>|
|<span data-ttu-id="f33b2-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f33b2-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="f33b2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f33b2-121">DateTimeOffset</span></span>|<span data-ttu-id="f33b2-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="f33b2-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="f33b2-123">Связи</span><span class="sxs-lookup"><span data-stu-id="f33b2-123">Relationships</span></span>
<span data-ttu-id="f33b2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f33b2-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f33b2-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f33b2-125">JSON Representation</span></span>
<span data-ttu-id="f33b2-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f33b2-126">Here is a JSON representation of the resource.</span></span>
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



