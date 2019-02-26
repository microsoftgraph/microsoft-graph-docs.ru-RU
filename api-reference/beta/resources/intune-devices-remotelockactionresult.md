---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f90cbc46ca4bc9476ad5d9386581385ae7354261
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159026"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="e7085-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="e7085-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="e7085-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7085-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7085-106">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="e7085-106">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="e7085-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e7085-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e7085-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7085-108">Properties</span></span>
|<span data-ttu-id="e7085-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7085-109">Property</span></span>|<span data-ttu-id="e7085-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7085-110">Type</span></span>|<span data-ttu-id="e7085-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7085-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7085-112">actionName</span><span class="sxs-lookup"><span data-stu-id="e7085-112">actionName</span></span>|<span data-ttu-id="e7085-113">String</span><span class="sxs-lookup"><span data-stu-id="e7085-113">String</span></span>|<span data-ttu-id="e7085-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e7085-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7085-115">actionState</span><span class="sxs-lookup"><span data-stu-id="e7085-115">actionState</span></span>|[<span data-ttu-id="e7085-116">actionState</span><span class="sxs-lookup"><span data-stu-id="e7085-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="e7085-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="e7085-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="e7085-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="e7085-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="e7085-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e7085-119">startDateTime</span></span>|<span data-ttu-id="e7085-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7085-120">DateTimeOffset</span></span>|<span data-ttu-id="e7085-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e7085-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7085-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7085-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="e7085-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7085-123">DateTimeOffset</span></span>|<span data-ttu-id="e7085-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="e7085-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="e7085-125">unlockPin</span><span class="sxs-lookup"><span data-stu-id="e7085-125">unlockPin</span></span>|<span data-ttu-id="e7085-126">String</span><span class="sxs-lookup"><span data-stu-id="e7085-126">String</span></span>|<span data-ttu-id="e7085-127">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="e7085-127">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7085-128">Связи</span><span class="sxs-lookup"><span data-stu-id="e7085-128">Relationships</span></span>
<span data-ttu-id="e7085-129">Нет</span><span class="sxs-lookup"><span data-stu-id="e7085-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7085-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7085-130">JSON Representation</span></span>
<span data-ttu-id="e7085-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7085-131">Here is a JSON representation of the resource.</span></span>
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




