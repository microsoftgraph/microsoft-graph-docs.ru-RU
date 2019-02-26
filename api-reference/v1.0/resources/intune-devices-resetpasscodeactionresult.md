---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e23c3e7d39566df98ab57258a54ab6f637439d1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257003"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="77eb9-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="77eb9-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="77eb9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77eb9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77eb9-105">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="77eb9-105">Reset passcode action result</span></span>


<span data-ttu-id="77eb9-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77eb9-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77eb9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="77eb9-107">Properties</span></span>
|<span data-ttu-id="77eb9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="77eb9-108">Property</span></span>|<span data-ttu-id="77eb9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77eb9-109">Type</span></span>|<span data-ttu-id="77eb9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77eb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77eb9-111">actionName</span><span class="sxs-lookup"><span data-stu-id="77eb9-111">actionName</span></span>|<span data-ttu-id="77eb9-112">String</span><span class="sxs-lookup"><span data-stu-id="77eb9-112">String</span></span>|<span data-ttu-id="77eb9-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77eb9-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77eb9-114">actionState</span><span class="sxs-lookup"><span data-stu-id="77eb9-114">actionState</span></span>|[<span data-ttu-id="77eb9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="77eb9-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="77eb9-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="77eb9-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="77eb9-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="77eb9-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="77eb9-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="77eb9-118">startDateTime</span></span>|<span data-ttu-id="77eb9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77eb9-119">DateTimeOffset</span></span>|<span data-ttu-id="77eb9-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77eb9-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77eb9-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="77eb9-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="77eb9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77eb9-122">DateTimeOffset</span></span>|<span data-ttu-id="77eb9-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="77eb9-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="77eb9-124">passcode</span><span class="sxs-lookup"><span data-stu-id="77eb9-124">passcode</span></span>|<span data-ttu-id="77eb9-125">String</span><span class="sxs-lookup"><span data-stu-id="77eb9-125">String</span></span>|<span data-ttu-id="77eb9-126">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="77eb9-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="77eb9-127">Связи</span><span class="sxs-lookup"><span data-stu-id="77eb9-127">Relationships</span></span>
<span data-ttu-id="77eb9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="77eb9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77eb9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77eb9-129">JSON Representation</span></span>
<span data-ttu-id="77eb9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77eb9-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



