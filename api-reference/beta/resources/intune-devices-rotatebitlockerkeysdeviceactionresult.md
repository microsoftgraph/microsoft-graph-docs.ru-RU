---
title: Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт
description: Результат действия устройства Ротатебитлоккеркэйс
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28e78b43a29f3fce7ba02da058f7e96d6358c39f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783874"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="d5ddd-103">Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="d5ddd-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

> <span data-ttu-id="d5ddd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5ddd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5ddd-106">Результат действия устройства Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="d5ddd-106">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="d5ddd-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d5ddd-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5ddd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5ddd-108">Properties</span></span>
|<span data-ttu-id="d5ddd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5ddd-109">Property</span></span>|<span data-ttu-id="d5ddd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d5ddd-110">Type</span></span>|<span data-ttu-id="d5ddd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d5ddd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5ddd-112">actionName</span><span class="sxs-lookup"><span data-stu-id="d5ddd-112">actionName</span></span>|<span data-ttu-id="d5ddd-113">String</span><span class="sxs-lookup"><span data-stu-id="d5ddd-113">String</span></span>|<span data-ttu-id="d5ddd-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d5ddd-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d5ddd-115">actionState</span><span class="sxs-lookup"><span data-stu-id="d5ddd-115">actionState</span></span>|[<span data-ttu-id="d5ddd-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d5ddd-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d5ddd-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d5ddd-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d5ddd-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d5ddd-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d5ddd-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d5ddd-119">startDateTime</span></span>|<span data-ttu-id="d5ddd-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5ddd-120">DateTimeOffset</span></span>|<span data-ttu-id="d5ddd-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d5ddd-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d5ddd-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5ddd-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="d5ddd-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5ddd-123">DateTimeOffset</span></span>|<span data-ttu-id="d5ddd-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d5ddd-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d5ddd-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5ddd-125">errorCode</span></span>|<span data-ttu-id="d5ddd-126">Int32</span><span class="sxs-lookup"><span data-stu-id="d5ddd-126">Int32</span></span>|<span data-ttu-id="d5ddd-127">Код ошибки действия Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="d5ddd-127">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5ddd-128">Связи</span><span class="sxs-lookup"><span data-stu-id="d5ddd-128">Relationships</span></span>
<span data-ttu-id="d5ddd-129">Нет</span><span class="sxs-lookup"><span data-stu-id="d5ddd-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5ddd-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5ddd-130">JSON Representation</span></span>
<span data-ttu-id="d5ddd-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5ddd-131">Here is a JSON representation of the resource.</span></span>
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



