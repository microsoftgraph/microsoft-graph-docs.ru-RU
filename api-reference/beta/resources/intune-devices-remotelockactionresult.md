---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31af22f66b87d8102eeaf81d68d211640326f3fd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963858"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="194e2-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="194e2-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="194e2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="194e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="194e2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="194e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="194e2-106">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="194e2-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="194e2-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="194e2-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="194e2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="194e2-108">Properties</span></span>
|<span data-ttu-id="194e2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="194e2-109">Property</span></span>|<span data-ttu-id="194e2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="194e2-110">Type</span></span>|<span data-ttu-id="194e2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="194e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="194e2-112">actionName</span><span class="sxs-lookup"><span data-stu-id="194e2-112">actionName</span></span>|<span data-ttu-id="194e2-113">String</span><span class="sxs-lookup"><span data-stu-id="194e2-113">String</span></span>|<span data-ttu-id="194e2-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="194e2-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="194e2-115">actionState</span><span class="sxs-lookup"><span data-stu-id="194e2-115">actionState</span></span>|[<span data-ttu-id="194e2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="194e2-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="194e2-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="194e2-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="194e2-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="194e2-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="194e2-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="194e2-119">startDateTime</span></span>|<span data-ttu-id="194e2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="194e2-120">DateTimeOffset</span></span>|<span data-ttu-id="194e2-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="194e2-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="194e2-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="194e2-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="194e2-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="194e2-123">DateTimeOffset</span></span>|<span data-ttu-id="194e2-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="194e2-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="194e2-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="194e2-125">unlockPin</span></span>|<span data-ttu-id="194e2-126">String</span><span class="sxs-lookup"><span data-stu-id="194e2-126">String</span></span>|<span data-ttu-id="194e2-127">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="194e2-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="194e2-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="194e2-128">Relationships</span></span>
<span data-ttu-id="194e2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="194e2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="194e2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="194e2-130">JSON Representation</span></span>
<span data-ttu-id="194e2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="194e2-131">Here is a JSON representation of the resource.</span></span>
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





