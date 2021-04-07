---
title: rotateBitLockerKeysDeviceActionResult resource type
description: Результат действия устройства RotateBitLockerKeys
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 527e90eab465045c5987830c08a6124ccacf16bf
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612044"
---
# <a name="rotatebitlockerkeysdeviceactionresult-resource-type"></a><span data-ttu-id="9db55-103">rotateBitLockerKeysDeviceActionResult resource type</span><span class="sxs-lookup"><span data-stu-id="9db55-103">rotateBitLockerKeysDeviceActionResult resource type</span></span>

<span data-ttu-id="9db55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9db55-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9db55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9db55-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9db55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9db55-107">Результат действия устройства RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="9db55-107">RotateBitLockerKeys device action result</span></span>


<span data-ttu-id="9db55-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9db55-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9db55-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9db55-109">Properties</span></span>
|<span data-ttu-id="9db55-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9db55-110">Property</span></span>|<span data-ttu-id="9db55-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9db55-111">Type</span></span>|<span data-ttu-id="9db55-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9db55-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9db55-113">actionName</span><span class="sxs-lookup"><span data-stu-id="9db55-113">actionName</span></span>|<span data-ttu-id="9db55-114">String</span><span class="sxs-lookup"><span data-stu-id="9db55-114">String</span></span>|<span data-ttu-id="9db55-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9db55-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9db55-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9db55-116">actionState</span></span>|[<span data-ttu-id="9db55-117">actionState</span><span class="sxs-lookup"><span data-stu-id="9db55-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9db55-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9db55-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9db55-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9db55-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9db55-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9db55-120">startDateTime</span></span>|<span data-ttu-id="9db55-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9db55-121">DateTimeOffset</span></span>|<span data-ttu-id="9db55-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9db55-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9db55-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9db55-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="9db55-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9db55-124">DateTimeOffset</span></span>|<span data-ttu-id="9db55-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9db55-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9db55-126">errorCode</span><span class="sxs-lookup"><span data-stu-id="9db55-126">errorCode</span></span>|<span data-ttu-id="9db55-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9db55-127">Int32</span></span>|<span data-ttu-id="9db55-128">Код ошибки действия RotateBitLockerKeys</span><span class="sxs-lookup"><span data-stu-id="9db55-128">RotateBitLockerKeys action error code</span></span>|

## <a name="relationships"></a><span data-ttu-id="9db55-129">Связи</span><span class="sxs-lookup"><span data-stu-id="9db55-129">Relationships</span></span>
<span data-ttu-id="9db55-130">Нет</span><span class="sxs-lookup"><span data-stu-id="9db55-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9db55-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9db55-131">JSON Representation</span></span>
<span data-ttu-id="9db55-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9db55-132">Here is a JSON representation of the resource.</span></span>
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




