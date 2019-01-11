---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 81a30b36ac418d5553c7387fea22a172926a73ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824859"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="98c1b-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="98c1b-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="98c1b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98c1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98c1b-105">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="98c1b-105">Reset passcode action result</span></span>

<span data-ttu-id="98c1b-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98c1b-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98c1b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="98c1b-107">Properties</span></span>
|<span data-ttu-id="98c1b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="98c1b-108">Property</span></span>|<span data-ttu-id="98c1b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="98c1b-109">Type</span></span>|<span data-ttu-id="98c1b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="98c1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98c1b-111">actionName</span><span class="sxs-lookup"><span data-stu-id="98c1b-111">actionName</span></span>|<span data-ttu-id="98c1b-112">String</span><span class="sxs-lookup"><span data-stu-id="98c1b-112">String</span></span>|<span data-ttu-id="98c1b-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98c1b-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98c1b-114">actionState</span><span class="sxs-lookup"><span data-stu-id="98c1b-114">actionState</span></span>|[<span data-ttu-id="98c1b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="98c1b-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="98c1b-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="98c1b-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="98c1b-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="98c1b-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="98c1b-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="98c1b-118">startDateTime</span></span>|<span data-ttu-id="98c1b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98c1b-119">DateTimeOffset</span></span>|<span data-ttu-id="98c1b-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98c1b-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98c1b-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="98c1b-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="98c1b-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98c1b-122">DateTimeOffset</span></span>|<span data-ttu-id="98c1b-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="98c1b-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="98c1b-124">passcode</span><span class="sxs-lookup"><span data-stu-id="98c1b-124">passcode</span></span>|<span data-ttu-id="98c1b-125">String</span><span class="sxs-lookup"><span data-stu-id="98c1b-125">String</span></span>|<span data-ttu-id="98c1b-126">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="98c1b-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="98c1b-127">Связи</span><span class="sxs-lookup"><span data-stu-id="98c1b-127">Relationships</span></span>
<span data-ttu-id="98c1b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="98c1b-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98c1b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98c1b-129">JSON Representation</span></span>
<span data-ttu-id="98c1b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98c1b-130">Here is a JSON representation of the resource.</span></span>
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



