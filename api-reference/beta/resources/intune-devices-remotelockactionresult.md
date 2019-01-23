---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7e57949e689f3d8e26c5217acec1a36662145b1a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416470"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="33ffc-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="33ffc-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="33ffc-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="33ffc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33ffc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="33ffc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33ffc-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33ffc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33ffc-107">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="33ffc-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="33ffc-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="33ffc-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33ffc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="33ffc-109">Properties</span></span>
|<span data-ttu-id="33ffc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="33ffc-110">Property</span></span>|<span data-ttu-id="33ffc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="33ffc-111">Type</span></span>|<span data-ttu-id="33ffc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="33ffc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33ffc-113">actionName</span><span class="sxs-lookup"><span data-stu-id="33ffc-113">actionName</span></span>|<span data-ttu-id="33ffc-114">String</span><span class="sxs-lookup"><span data-stu-id="33ffc-114">String</span></span>|<span data-ttu-id="33ffc-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="33ffc-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33ffc-116">actionState</span><span class="sxs-lookup"><span data-stu-id="33ffc-116">actionState</span></span>|[<span data-ttu-id="33ffc-117">actionState</span><span class="sxs-lookup"><span data-stu-id="33ffc-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="33ffc-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="33ffc-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="33ffc-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="33ffc-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="33ffc-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="33ffc-120">startDateTime</span></span>|<span data-ttu-id="33ffc-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ffc-121">DateTimeOffset</span></span>|<span data-ttu-id="33ffc-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="33ffc-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33ffc-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="33ffc-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="33ffc-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33ffc-124">DateTimeOffset</span></span>|<span data-ttu-id="33ffc-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="33ffc-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="33ffc-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="33ffc-126">unlockPin</span></span>|<span data-ttu-id="33ffc-127">String</span><span class="sxs-lookup"><span data-stu-id="33ffc-127">String</span></span>|<span data-ttu-id="33ffc-128">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="33ffc-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="33ffc-129">Связи</span><span class="sxs-lookup"><span data-stu-id="33ffc-129">Relationships</span></span>
<span data-ttu-id="33ffc-130">Нет</span><span class="sxs-lookup"><span data-stu-id="33ffc-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33ffc-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33ffc-131">JSON Representation</span></span>
<span data-ttu-id="33ffc-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33ffc-132">Here is a JSON representation of the resource.</span></span>
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




