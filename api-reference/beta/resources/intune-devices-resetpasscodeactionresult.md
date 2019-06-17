---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5684d5bc61ecde5eb41b258b88e1ae1ff3502f4a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963851"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="99073-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="99073-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="99073-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99073-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99073-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="99073-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99073-106">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="99073-106">Reset passcode action result</span></span>


<span data-ttu-id="99073-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="99073-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99073-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="99073-108">Properties</span></span>
|<span data-ttu-id="99073-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="99073-109">Property</span></span>|<span data-ttu-id="99073-110">Тип</span><span class="sxs-lookup"><span data-stu-id="99073-110">Type</span></span>|<span data-ttu-id="99073-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99073-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99073-112">actionName</span><span class="sxs-lookup"><span data-stu-id="99073-112">actionName</span></span>|<span data-ttu-id="99073-113">String</span><span class="sxs-lookup"><span data-stu-id="99073-113">String</span></span>|<span data-ttu-id="99073-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="99073-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="99073-115">actionState</span><span class="sxs-lookup"><span data-stu-id="99073-115">actionState</span></span>|[<span data-ttu-id="99073-116">actionState</span><span class="sxs-lookup"><span data-stu-id="99073-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="99073-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="99073-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="99073-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="99073-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="99073-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="99073-119">startDateTime</span></span>|<span data-ttu-id="99073-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99073-120">DateTimeOffset</span></span>|<span data-ttu-id="99073-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="99073-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="99073-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="99073-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="99073-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99073-123">DateTimeOffset</span></span>|<span data-ttu-id="99073-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="99073-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="99073-125">passcode</span><span class="sxs-lookup"><span data-stu-id="99073-125">passcode</span></span>|<span data-ttu-id="99073-126">String</span><span class="sxs-lookup"><span data-stu-id="99073-126">String</span></span>|<span data-ttu-id="99073-127">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="99073-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="99073-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="99073-128">Relationships</span></span>
<span data-ttu-id="99073-129">Нет</span><span class="sxs-lookup"><span data-stu-id="99073-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99073-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99073-130">JSON Representation</span></span>
<span data-ttu-id="99073-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99073-131">Here is a JSON representation of the resource.</span></span>
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





