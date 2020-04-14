---
title: Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт
description: Результат действия устройства Ротатебитлоккеркэйс
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91f21809f7ba1ab0af27a969fb1646b571ea87ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43383082"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="0a951-103">Тип ресурса Ротатебитлоккеркэйсдевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="0a951-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="0a951-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a951-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0a951-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a951-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a951-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a951-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a951-107">Результат действия устройства Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="0a951-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="0a951-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0a951-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a951-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a951-109">Properties</span></span>
|<span data-ttu-id="0a951-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a951-110">Property</span></span>|<span data-ttu-id="0a951-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0a951-111">Type</span></span>|<span data-ttu-id="0a951-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0a951-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a951-113">actionName</span><span class="sxs-lookup"><span data-stu-id="0a951-113">actionName</span></span>|<span data-ttu-id="0a951-114">String</span><span class="sxs-lookup"><span data-stu-id="0a951-114">String</span></span>|<span data-ttu-id="0a951-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0a951-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0a951-116">actionState</span><span class="sxs-lookup"><span data-stu-id="0a951-116">actionState</span></span>|[<span data-ttu-id="0a951-117">actionState</span><span class="sxs-lookup"><span data-stu-id="0a951-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="0a951-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0a951-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0a951-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0a951-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0a951-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0a951-120">startDateTime</span></span>|<span data-ttu-id="0a951-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a951-121">DateTimeOffset</span></span>|<span data-ttu-id="0a951-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0a951-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0a951-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a951-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="0a951-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a951-124">DateTimeOffset</span></span>|<span data-ttu-id="0a951-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0a951-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0a951-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="0a951-126">errorCode</span></span>|<span data-ttu-id="0a951-127">Int32</span><span class="sxs-lookup"><span data-stu-id="0a951-127">Int32</span></span>|<span data-ttu-id="0a951-128">Код ошибки действия Ротатебитлоккеркэйс</span><span class="sxs-lookup"><span data-stu-id="0a951-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a951-129">Связи</span><span class="sxs-lookup"><span data-stu-id="0a951-129">Relationships</span></span>
<span data-ttu-id="0a951-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0a951-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a951-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a951-131">JSON Representation</span></span>
<span data-ttu-id="0a951-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a951-132">Here is a JSON representation of the resource.</span></span>
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



