---
title: Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт
description: Результат действия устройства Ротатебитлоккеркэйс
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4f4196c25146ba72e0b9fec5fc67dce9d521275d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299101"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="c77a2-103">Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="c77a2-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="c77a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c77a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c77a2-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c77a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c77a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c77a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c77a2-107">Результат действия устройства Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="c77a2-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="c77a2-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c77a2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c77a2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c77a2-109">Properties</span></span>
|<span data-ttu-id="c77a2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c77a2-110">Property</span></span>|<span data-ttu-id="c77a2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c77a2-111">Type</span></span>|<span data-ttu-id="c77a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c77a2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c77a2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c77a2-113">actionName</span></span>|<span data-ttu-id="c77a2-114">String</span><span class="sxs-lookup"><span data-stu-id="c77a2-114">String</span></span>|<span data-ttu-id="c77a2-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c77a2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c77a2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c77a2-116">actionState</span></span>|[<span data-ttu-id="c77a2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c77a2-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c77a2-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c77a2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c77a2-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c77a2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c77a2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c77a2-120">startDateTime</span></span>|<span data-ttu-id="c77a2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77a2-121">DateTimeOffset</span></span>|<span data-ttu-id="c77a2-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c77a2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c77a2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c77a2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c77a2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c77a2-124">DateTimeOffset</span></span>|<span data-ttu-id="c77a2-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c77a2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c77a2-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="c77a2-126">errorCode</span></span>|<span data-ttu-id="c77a2-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c77a2-127">Int32</span></span>|<span data-ttu-id="c77a2-128">Код ошибки действия Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="c77a2-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="c77a2-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c77a2-129">Relationships</span></span>
<span data-ttu-id="c77a2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c77a2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c77a2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c77a2-131">JSON Representation</span></span>
<span data-ttu-id="c77a2-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c77a2-132">Here is a JSON representation of the resource.</span></span>
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




