---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6725e0a51ad9b4053278dcf03c91236a7d820665
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091021"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="7bbb3-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="7bbb3-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="7bbb3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bbb3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bbb3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bbb3-106">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="7bbb3-106">Reset passcode action result</span></span>


<span data-ttu-id="7bbb3-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7bbb3-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bbb3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bbb3-108">Properties</span></span>
|<span data-ttu-id="7bbb3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bbb3-109">Property</span></span>|<span data-ttu-id="7bbb3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7bbb3-110">Type</span></span>|<span data-ttu-id="7bbb3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7bbb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bbb3-112">actionName</span><span class="sxs-lookup"><span data-stu-id="7bbb3-112">actionName</span></span>|<span data-ttu-id="7bbb3-113">String</span><span class="sxs-lookup"><span data-stu-id="7bbb3-113">String</span></span>|<span data-ttu-id="7bbb3-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7bbb3-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7bbb3-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7bbb3-115">actionState</span></span>|[<span data-ttu-id="7bbb3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7bbb3-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7bbb3-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7bbb3-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7bbb3-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7bbb3-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7bbb3-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7bbb3-119">startDateTime</span></span>|<span data-ttu-id="7bbb3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bbb3-120">DateTimeOffset</span></span>|<span data-ttu-id="7bbb3-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7bbb3-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7bbb3-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7bbb3-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="7bbb3-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bbb3-123">DateTimeOffset</span></span>|<span data-ttu-id="7bbb3-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7bbb3-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7bbb3-125">passcode</span><span class="sxs-lookup"><span data-stu-id="7bbb3-125">passcode</span></span>|<span data-ttu-id="7bbb3-126">String</span><span class="sxs-lookup"><span data-stu-id="7bbb3-126">String</span></span>|<span data-ttu-id="7bbb3-127">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="7bbb3-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="7bbb3-128">Связи</span><span class="sxs-lookup"><span data-stu-id="7bbb3-128">Relationships</span></span>
<span data-ttu-id="7bbb3-129">Нет</span><span class="sxs-lookup"><span data-stu-id="7bbb3-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bbb3-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bbb3-130">JSON Representation</span></span>
<span data-ttu-id="7bbb3-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bbb3-131">Here is a JSON representation of the resource.</span></span>
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









