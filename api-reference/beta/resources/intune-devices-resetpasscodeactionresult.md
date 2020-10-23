---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a8d38fc68a9ce02645892810bc4029ea126198d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48691332"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="9df5e-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="9df5e-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="9df5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9df5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9df5e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9df5e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9df5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9df5e-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="9df5e-107">Reset passcode action result</span></span>


<span data-ttu-id="9df5e-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9df5e-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9df5e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9df5e-109">Properties</span></span>
|<span data-ttu-id="9df5e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9df5e-110">Property</span></span>|<span data-ttu-id="9df5e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9df5e-111">Type</span></span>|<span data-ttu-id="9df5e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9df5e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9df5e-113">actionName</span><span class="sxs-lookup"><span data-stu-id="9df5e-113">actionName</span></span>|<span data-ttu-id="9df5e-114">String</span><span class="sxs-lookup"><span data-stu-id="9df5e-114">String</span></span>|<span data-ttu-id="9df5e-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9df5e-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9df5e-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9df5e-116">actionState</span></span>|[<span data-ttu-id="9df5e-117">actionState</span><span class="sxs-lookup"><span data-stu-id="9df5e-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9df5e-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9df5e-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9df5e-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9df5e-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9df5e-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9df5e-120">startDateTime</span></span>|<span data-ttu-id="9df5e-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df5e-121">DateTimeOffset</span></span>|<span data-ttu-id="9df5e-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9df5e-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9df5e-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9df5e-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="9df5e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9df5e-124">DateTimeOffset</span></span>|<span data-ttu-id="9df5e-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9df5e-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9df5e-126">passcode</span><span class="sxs-lookup"><span data-stu-id="9df5e-126">passcode</span></span>|<span data-ttu-id="9df5e-127">String</span><span class="sxs-lookup"><span data-stu-id="9df5e-127">String</span></span>|<span data-ttu-id="9df5e-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="9df5e-128">Newly generated passcode for the device</span></span> |
|<span data-ttu-id="9df5e-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="9df5e-129">errorCode</span></span>|<span data-ttu-id="9df5e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="9df5e-130">Int32</span></span>|<span data-ttu-id="9df5e-131">Код ошибки действия Ротатебитлоккеркэйс.</span><span class="sxs-lookup"><span data-stu-id="9df5e-131">RotateBitLockerKeys action error code.</span></span> <span data-ttu-id="9df5e-132">Допустимые значения — от 0 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="9df5e-132">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="9df5e-133">Связи</span><span class="sxs-lookup"><span data-stu-id="9df5e-133">Relationships</span></span>
<span data-ttu-id="9df5e-134">Нет</span><span class="sxs-lookup"><span data-stu-id="9df5e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df5e-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9df5e-135">JSON Representation</span></span>
<span data-ttu-id="9df5e-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9df5e-136">Here is a JSON representation of the resource.</span></span>
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
  "passcode": "String",
  "errorCode": 1024
}
```





