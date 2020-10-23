---
title: Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт
description: Результат действия устройства Ротатебитлоккеркэйс
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6457b87007fe24084c35b27c1b658de564767984
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724497"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="2ff88-103">Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="2ff88-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="2ff88-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ff88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ff88-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2ff88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ff88-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ff88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff88-107">Результат действия устройства Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="2ff88-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="2ff88-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2ff88-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ff88-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ff88-109">Properties</span></span>
|<span data-ttu-id="2ff88-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ff88-110">Property</span></span>|<span data-ttu-id="2ff88-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2ff88-111">Type</span></span>|<span data-ttu-id="2ff88-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2ff88-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff88-113">actionName</span><span class="sxs-lookup"><span data-stu-id="2ff88-113">actionName</span></span>|<span data-ttu-id="2ff88-114">String</span><span class="sxs-lookup"><span data-stu-id="2ff88-114">String</span></span>|<span data-ttu-id="2ff88-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2ff88-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2ff88-116">actionState</span><span class="sxs-lookup"><span data-stu-id="2ff88-116">actionState</span></span>|[<span data-ttu-id="2ff88-117">actionState</span><span class="sxs-lookup"><span data-stu-id="2ff88-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="2ff88-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2ff88-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="2ff88-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="2ff88-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="2ff88-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff88-120">startDateTime</span></span>|<span data-ttu-id="2ff88-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff88-121">DateTimeOffset</span></span>|<span data-ttu-id="2ff88-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2ff88-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2ff88-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff88-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="2ff88-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff88-124">DateTimeOffset</span></span>|<span data-ttu-id="2ff88-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="2ff88-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="2ff88-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="2ff88-126">errorCode</span></span>|<span data-ttu-id="2ff88-127">Int32</span><span class="sxs-lookup"><span data-stu-id="2ff88-127">Int32</span></span>|<span data-ttu-id="2ff88-128">Код ошибки действия Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="2ff88-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ff88-129">Связи</span><span class="sxs-lookup"><span data-stu-id="2ff88-129">Relationships</span></span>
<span data-ttu-id="2ff88-130">Нет</span><span class="sxs-lookup"><span data-stu-id="2ff88-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ff88-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ff88-131">JSON Representation</span></span>
<span data-ttu-id="2ff88-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ff88-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "errorCode": 1024
}
```





