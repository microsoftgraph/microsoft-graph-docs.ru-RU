---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c533d9590acba1518ac3d0dc791af804b9d84452
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550641"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="137a9-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="137a9-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="137a9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="137a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="137a9-105">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="137a9-105">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="137a9-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="137a9-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="137a9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="137a9-107">Properties</span></span>
|<span data-ttu-id="137a9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="137a9-108">Property</span></span>|<span data-ttu-id="137a9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="137a9-109">Type</span></span>|<span data-ttu-id="137a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="137a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="137a9-111">actionName</span><span class="sxs-lookup"><span data-stu-id="137a9-111">actionName</span></span>|<span data-ttu-id="137a9-112">String</span><span class="sxs-lookup"><span data-stu-id="137a9-112">String</span></span>|<span data-ttu-id="137a9-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="137a9-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="137a9-114">actionState</span><span class="sxs-lookup"><span data-stu-id="137a9-114">actionState</span></span>|[<span data-ttu-id="137a9-115">actionState</span><span class="sxs-lookup"><span data-stu-id="137a9-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="137a9-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="137a9-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="137a9-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="137a9-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="137a9-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="137a9-118">startDateTime</span></span>|<span data-ttu-id="137a9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="137a9-119">DateTimeOffset</span></span>|<span data-ttu-id="137a9-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="137a9-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="137a9-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="137a9-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="137a9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="137a9-122">DateTimeOffset</span></span>|<span data-ttu-id="137a9-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="137a9-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="137a9-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="137a9-124">unlockPin</span></span>|<span data-ttu-id="137a9-125">String</span><span class="sxs-lookup"><span data-stu-id="137a9-125">String</span></span>|<span data-ttu-id="137a9-126">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="137a9-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="137a9-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="137a9-127">Relationships</span></span>
<span data-ttu-id="137a9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="137a9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="137a9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="137a9-129">JSON Representation</span></span>
<span data-ttu-id="137a9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="137a9-130">Here is a JSON representation of the resource.</span></span>
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



