---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: tfitzmac
ms.openlocfilehash: 44d56b2ee20629d1cefbf965c72e5f6cc17fb0a2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353692"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="9b0db-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="9b0db-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="9b0db-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9b0db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9b0db-105">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="9b0db-105">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="9b0db-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b0db-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b0db-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b0db-107">Properties</span></span>
|<span data-ttu-id="9b0db-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b0db-108">Property</span></span>|<span data-ttu-id="9b0db-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9b0db-109">Type</span></span>|<span data-ttu-id="9b0db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b0db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b0db-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9b0db-111">actionName</span></span>|<span data-ttu-id="9b0db-112">String</span><span class="sxs-lookup"><span data-stu-id="9b0db-112">String</span></span>|<span data-ttu-id="9b0db-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b0db-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b0db-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9b0db-114">actionState</span></span>|[<span data-ttu-id="9b0db-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9b0db-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9b0db-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9b0db-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9b0db-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9b0db-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9b0db-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9b0db-118">startDateTime</span></span>|<span data-ttu-id="9b0db-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b0db-119">DateTimeOffset</span></span>|<span data-ttu-id="9b0db-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b0db-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b0db-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b0db-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9b0db-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b0db-122">DateTimeOffset</span></span>|<span data-ttu-id="9b0db-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9b0db-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9b0db-124">unlockPin</span><span class="sxs-lookup"><span data-stu-id="9b0db-124">unlockPin</span></span>|<span data-ttu-id="9b0db-125">String</span><span class="sxs-lookup"><span data-stu-id="9b0db-125">String</span></span>|<span data-ttu-id="9b0db-126">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="9b0db-126">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b0db-127">Связи</span><span class="sxs-lookup"><span data-stu-id="9b0db-127">Relationships</span></span>
<span data-ttu-id="9b0db-128">Нет</span><span class="sxs-lookup"><span data-stu-id="9b0db-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9b0db-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b0db-129">JSON Representation</span></span>
<span data-ttu-id="9b0db-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b0db-130">Here is a JSON representation of the resource.</span></span>
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



