---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 062d287aec9f0a0be8acbf380a5300458367f014
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356907"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="aafbe-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="aafbe-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="aafbe-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aafbe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aafbe-105">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="aafbe-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="aafbe-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="aafbe-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aafbe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aafbe-107">Properties</span></span>
|<span data-ttu-id="aafbe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aafbe-108">Property</span></span>|<span data-ttu-id="aafbe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aafbe-109">Type</span></span>|<span data-ttu-id="aafbe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aafbe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aafbe-111">actionName</span><span class="sxs-lookup"><span data-stu-id="aafbe-111">actionName</span></span>|<span data-ttu-id="aafbe-112">String</span><span class="sxs-lookup"><span data-stu-id="aafbe-112">String</span></span>|<span data-ttu-id="aafbe-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="aafbe-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="aafbe-114">actionState</span><span class="sxs-lookup"><span data-stu-id="aafbe-114">actionState</span></span>|[<span data-ttu-id="aafbe-115">actionState</span><span class="sxs-lookup"><span data-stu-id="aafbe-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="aafbe-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="aafbe-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="aafbe-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="aafbe-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="aafbe-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aafbe-118">startDateTime</span></span>|<span data-ttu-id="aafbe-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aafbe-119">DateTimeOffset</span></span>|<span data-ttu-id="aafbe-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="aafbe-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="aafbe-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="aafbe-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="aafbe-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aafbe-122">DateTimeOffset</span></span>|<span data-ttu-id="aafbe-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="aafbe-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="aafbe-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="aafbe-124">unlockPin</span></span>|<span data-ttu-id="aafbe-125">String</span><span class="sxs-lookup"><span data-stu-id="aafbe-125">String</span></span>|<span data-ttu-id="aafbe-126">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="aafbe-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="aafbe-127">Связи</span><span class="sxs-lookup"><span data-stu-id="aafbe-127">Relationships</span></span>
<span data-ttu-id="aafbe-128">Нет</span><span class="sxs-lookup"><span data-stu-id="aafbe-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aafbe-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aafbe-129">JSON Representation</span></span>
<span data-ttu-id="aafbe-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aafbe-130">Here is a JSON representation of the resource.</span></span>
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




