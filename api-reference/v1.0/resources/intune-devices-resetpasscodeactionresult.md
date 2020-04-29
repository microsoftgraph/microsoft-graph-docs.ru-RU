---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8510dcb20fa0af50df1db24927b97c32afb1188
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439444"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="0582f-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="0582f-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="0582f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0582f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0582f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0582f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0582f-106">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="0582f-106">Reset passcode action result</span></span>


<span data-ttu-id="0582f-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0582f-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0582f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0582f-108">Properties</span></span>
|<span data-ttu-id="0582f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0582f-109">Property</span></span>|<span data-ttu-id="0582f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0582f-110">Type</span></span>|<span data-ttu-id="0582f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0582f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0582f-112">actionName</span><span class="sxs-lookup"><span data-stu-id="0582f-112">actionName</span></span>|<span data-ttu-id="0582f-113">String</span><span class="sxs-lookup"><span data-stu-id="0582f-113">String</span></span>|<span data-ttu-id="0582f-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0582f-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0582f-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0582f-115">actionState</span></span>|[<span data-ttu-id="0582f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0582f-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="0582f-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0582f-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0582f-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0582f-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0582f-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0582f-119">startDateTime</span></span>|<span data-ttu-id="0582f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0582f-120">DateTimeOffset</span></span>|<span data-ttu-id="0582f-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0582f-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0582f-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0582f-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="0582f-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0582f-123">DateTimeOffset</span></span>|<span data-ttu-id="0582f-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0582f-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0582f-125">passcode</span><span class="sxs-lookup"><span data-stu-id="0582f-125">passcode</span></span>|<span data-ttu-id="0582f-126">String</span><span class="sxs-lookup"><span data-stu-id="0582f-126">String</span></span>|<span data-ttu-id="0582f-127">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="0582f-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="0582f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0582f-128">Relationships</span></span>
<span data-ttu-id="0582f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0582f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0582f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0582f-130">JSON Representation</span></span>
<span data-ttu-id="0582f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0582f-131">Here is a JSON representation of the resource.</span></span>
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







