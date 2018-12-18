---
title: Тип ресурса deviceActionResult
description: Результат действия, касающегося устройства
author: tfitzmac
ms.openlocfilehash: 48429e059616d9af0e3cbdac8544e68354b94fb5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320547"
---
# <a name="deviceactionresult-resource-type"></a><span data-ttu-id="8fbda-103">Тип ресурса deviceActionResult</span><span class="sxs-lookup"><span data-stu-id="8fbda-103">deviceActionResult resource type</span></span>

> <span data-ttu-id="8fbda-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8fbda-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8fbda-105">Результат действия, касающегося устройства</span><span class="sxs-lookup"><span data-stu-id="8fbda-105">Device action result</span></span>
## <a name="properties"></a><span data-ttu-id="8fbda-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fbda-106">Properties</span></span>
|<span data-ttu-id="8fbda-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fbda-107">Property</span></span>|<span data-ttu-id="8fbda-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8fbda-108">Type</span></span>|<span data-ttu-id="8fbda-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8fbda-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fbda-110">actionName</span><span class="sxs-lookup"><span data-stu-id="8fbda-110">actionName</span></span>|<span data-ttu-id="8fbda-111">String</span><span class="sxs-lookup"><span data-stu-id="8fbda-111">String</span></span>|<span data-ttu-id="8fbda-112">Название действия</span><span class="sxs-lookup"><span data-stu-id="8fbda-112">Action name</span></span>|
|<span data-ttu-id="8fbda-113">actionState</span><span class="sxs-lookup"><span data-stu-id="8fbda-113">actionState</span></span>|[<span data-ttu-id="8fbda-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8fbda-114">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8fbda-115">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="8fbda-115">State of the action.</span></span> <span data-ttu-id="8fbda-116">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8fbda-116">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8fbda-117">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8fbda-117">startDateTime</span></span>|<span data-ttu-id="8fbda-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fbda-118">DateTimeOffset</span></span>|<span data-ttu-id="8fbda-119">Время начала действия</span><span class="sxs-lookup"><span data-stu-id="8fbda-119">Time the action was initiated</span></span>|
|<span data-ttu-id="8fbda-120">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fbda-120">lastUpdatedDateTime</span></span>|<span data-ttu-id="8fbda-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fbda-121">DateTimeOffset</span></span>|<span data-ttu-id="8fbda-122">Время последнего обновления состояния действия</span><span class="sxs-lookup"><span data-stu-id="8fbda-122">Time the action state was last updated</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fbda-123">Связи</span><span class="sxs-lookup"><span data-stu-id="8fbda-123">Relationships</span></span>
<span data-ttu-id="8fbda-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8fbda-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8fbda-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fbda-125">JSON Representation</span></span>
<span data-ttu-id="8fbda-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fbda-126">Here is a JSON representation of the resource.</span></span>
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



