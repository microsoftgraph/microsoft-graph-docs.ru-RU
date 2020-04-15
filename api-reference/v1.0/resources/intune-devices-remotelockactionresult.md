---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fcf663ad633f09a1198c901ffa1b82c2278b3ba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406828"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="a7d6d-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="a7d6d-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="a7d6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7d6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7d6d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7d6d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7d6d-106">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="a7d6d-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="a7d6d-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7d6d-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a7d6d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7d6d-108">Properties</span></span>
|<span data-ttu-id="a7d6d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d6d-109">Property</span></span>|<span data-ttu-id="a7d6d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d6d-110">Type</span></span>|<span data-ttu-id="a7d6d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d6d-112">actionName</span><span class="sxs-lookup"><span data-stu-id="a7d6d-112">actionName</span></span>|<span data-ttu-id="a7d6d-113">String</span><span class="sxs-lookup"><span data-stu-id="a7d6d-113">String</span></span>|<span data-ttu-id="a7d6d-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a7d6d-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7d6d-115">actionState</span><span class="sxs-lookup"><span data-stu-id="a7d6d-115">actionState</span></span>|[<span data-ttu-id="a7d6d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="a7d6d-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="a7d6d-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a7d6d-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="a7d6d-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="a7d6d-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="a7d6d-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="a7d6d-119">startDateTime</span></span>|<span data-ttu-id="a7d6d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7d6d-120">DateTimeOffset</span></span>|<span data-ttu-id="a7d6d-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="a7d6d-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7d6d-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7d6d-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="a7d6d-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7d6d-123">DateTimeOffset</span></span>|<span data-ttu-id="a7d6d-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="a7d6d-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="a7d6d-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="a7d6d-125">unlockPin</span></span>|<span data-ttu-id="a7d6d-126">String</span><span class="sxs-lookup"><span data-stu-id="a7d6d-126">String</span></span>|<span data-ttu-id="a7d6d-127">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="a7d6d-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7d6d-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="a7d6d-128">Relationships</span></span>
<span data-ttu-id="a7d6d-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a7d6d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7d6d-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7d6d-130">JSON Representation</span></span>
<span data-ttu-id="a7d6d-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7d6d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```







