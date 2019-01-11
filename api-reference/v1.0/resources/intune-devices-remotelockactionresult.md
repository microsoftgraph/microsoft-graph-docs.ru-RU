---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cba3a5ab51f5283ce6f3ca61f7cda992eeca5b8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855155"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="0ddc5-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="0ddc5-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="0ddc5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ddc5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ddc5-105">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="0ddc5-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="0ddc5-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc5-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ddc5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ddc5-107">Properties</span></span>
|<span data-ttu-id="0ddc5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ddc5-108">Property</span></span>|<span data-ttu-id="0ddc5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ddc5-109">Type</span></span>|<span data-ttu-id="0ddc5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ddc5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ddc5-111">actionName</span><span class="sxs-lookup"><span data-stu-id="0ddc5-111">actionName</span></span>|<span data-ttu-id="0ddc5-112">String</span><span class="sxs-lookup"><span data-stu-id="0ddc5-112">String</span></span>|<span data-ttu-id="0ddc5-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc5-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0ddc5-114">actionState</span><span class="sxs-lookup"><span data-stu-id="0ddc5-114">actionState</span></span>|[<span data-ttu-id="0ddc5-115">actionState</span><span class="sxs-lookup"><span data-stu-id="0ddc5-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="0ddc5-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="0ddc5-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="0ddc5-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="0ddc5-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="0ddc5-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddc5-118">startDateTime</span></span>|<span data-ttu-id="0ddc5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddc5-119">DateTimeOffset</span></span>|<span data-ttu-id="0ddc5-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc5-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0ddc5-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ddc5-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="0ddc5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ddc5-122">DateTimeOffset</span></span>|<span data-ttu-id="0ddc5-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="0ddc5-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="0ddc5-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="0ddc5-124">unlockPin</span></span>|<span data-ttu-id="0ddc5-125">String</span><span class="sxs-lookup"><span data-stu-id="0ddc5-125">String</span></span>|<span data-ttu-id="0ddc5-126">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="0ddc5-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ddc5-127">Связи</span><span class="sxs-lookup"><span data-stu-id="0ddc5-127">Relationships</span></span>
<span data-ttu-id="0ddc5-128">Нет</span><span class="sxs-lookup"><span data-stu-id="0ddc5-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ddc5-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ddc5-129">JSON Representation</span></span>
<span data-ttu-id="0ddc5-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ddc5-130">Here is a JSON representation of the resource.</span></span>
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



