---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61f70e9de99b831e650fa08d3d59e5359a9d93ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941781"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="b5ab4-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="b5ab4-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="b5ab4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5ab4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5ab4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b5ab4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5ab4-106">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="b5ab4-106">Reset passcode action result</span></span>


<span data-ttu-id="b5ab4-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b5ab4-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5ab4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5ab4-108">Properties</span></span>
|<span data-ttu-id="b5ab4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5ab4-109">Property</span></span>|<span data-ttu-id="b5ab4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b5ab4-110">Type</span></span>|<span data-ttu-id="b5ab4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b5ab4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5ab4-112">actionName</span><span class="sxs-lookup"><span data-stu-id="b5ab4-112">actionName</span></span>|<span data-ttu-id="b5ab4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b5ab4-113">String</span></span>|<span data-ttu-id="b5ab4-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5ab4-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5ab4-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b5ab4-115">actionState</span></span>|[<span data-ttu-id="b5ab4-116">actionState</span><span class="sxs-lookup"><span data-stu-id="b5ab4-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="b5ab4-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5ab4-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b5ab4-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b5ab4-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b5ab4-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b5ab4-119">startDateTime</span></span>|<span data-ttu-id="b5ab4-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5ab4-120">DateTimeOffset</span></span>|<span data-ttu-id="b5ab4-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b5ab4-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5ab4-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5ab4-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="b5ab4-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5ab4-123">DateTimeOffset</span></span>|<span data-ttu-id="b5ab4-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b5ab4-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b5ab4-125">passcode</span><span class="sxs-lookup"><span data-stu-id="b5ab4-125">passcode</span></span>|<span data-ttu-id="b5ab4-126">String</span><span class="sxs-lookup"><span data-stu-id="b5ab4-126">String</span></span>|<span data-ttu-id="b5ab4-127">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="b5ab4-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5ab4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="b5ab4-128">Relationships</span></span>
<span data-ttu-id="b5ab4-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b5ab4-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5ab4-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5ab4-130">JSON Representation</span></span>
<span data-ttu-id="b5ab4-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5ab4-131">Here is a JSON representation of the resource.</span></span>
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




