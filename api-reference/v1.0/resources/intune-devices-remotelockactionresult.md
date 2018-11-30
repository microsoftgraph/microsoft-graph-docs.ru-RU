---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
ms.openlocfilehash: e0fff0a9ee389a1a73db1ad19ea3eba55a04989d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027014"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="af749-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="af749-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="af749-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="af749-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af749-105">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="af749-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="af749-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af749-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af749-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af749-107">Properties</span></span>
|<span data-ttu-id="af749-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af749-108">Property</span></span>|<span data-ttu-id="af749-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af749-109">Type</span></span>|<span data-ttu-id="af749-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af749-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af749-111">actionName</span><span class="sxs-lookup"><span data-stu-id="af749-111">actionName</span></span>|<span data-ttu-id="af749-112">String</span><span class="sxs-lookup"><span data-stu-id="af749-112">String</span></span>|<span data-ttu-id="af749-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af749-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af749-114">actionState</span><span class="sxs-lookup"><span data-stu-id="af749-114">actionState</span></span>|[<span data-ttu-id="af749-115">actionState</span><span class="sxs-lookup"><span data-stu-id="af749-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="af749-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="af749-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="af749-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="af749-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="af749-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="af749-118">startDateTime</span></span>|<span data-ttu-id="af749-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af749-119">DateTimeOffset</span></span>|<span data-ttu-id="af749-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af749-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af749-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="af749-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="af749-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af749-122">DateTimeOffset</span></span>|<span data-ttu-id="af749-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="af749-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="af749-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="af749-124">unlockPin</span></span>|<span data-ttu-id="af749-125">String</span><span class="sxs-lookup"><span data-stu-id="af749-125">String</span></span>|<span data-ttu-id="af749-126">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="af749-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="af749-127">Связи</span><span class="sxs-lookup"><span data-stu-id="af749-127">Relationships</span></span>
<span data-ttu-id="af749-128">Нет</span><span class="sxs-lookup"><span data-stu-id="af749-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="af749-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af749-129">JSON Representation</span></span>
<span data-ttu-id="af749-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af749-130">Here is a JSON representation of the resource.</span></span>
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



