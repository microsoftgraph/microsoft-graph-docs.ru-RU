---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 49131d0ba78a37a33879ad29d2f01a78835d8b2b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081092"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="6700a-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="6700a-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="6700a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6700a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6700a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6700a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6700a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6700a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6700a-107">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="6700a-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="6700a-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6700a-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6700a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6700a-109">Properties</span></span>
|<span data-ttu-id="6700a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6700a-110">Property</span></span>|<span data-ttu-id="6700a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6700a-111">Type</span></span>|<span data-ttu-id="6700a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6700a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6700a-113">actionName</span><span class="sxs-lookup"><span data-stu-id="6700a-113">actionName</span></span>|<span data-ttu-id="6700a-114">String</span><span class="sxs-lookup"><span data-stu-id="6700a-114">String</span></span>|<span data-ttu-id="6700a-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6700a-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6700a-116">actionState</span><span class="sxs-lookup"><span data-stu-id="6700a-116">actionState</span></span>|[<span data-ttu-id="6700a-117">actionState</span><span class="sxs-lookup"><span data-stu-id="6700a-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6700a-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6700a-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="6700a-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6700a-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6700a-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6700a-120">startDateTime</span></span>|<span data-ttu-id="6700a-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6700a-121">DateTimeOffset</span></span>|<span data-ttu-id="6700a-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="6700a-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6700a-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6700a-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="6700a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6700a-124">DateTimeOffset</span></span>|<span data-ttu-id="6700a-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6700a-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="6700a-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="6700a-126">unlockPin</span></span>|<span data-ttu-id="6700a-127">String</span><span class="sxs-lookup"><span data-stu-id="6700a-127">String</span></span>|<span data-ttu-id="6700a-128">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="6700a-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="6700a-129">Связи</span><span class="sxs-lookup"><span data-stu-id="6700a-129">Relationships</span></span>
<span data-ttu-id="6700a-130">Нет</span><span class="sxs-lookup"><span data-stu-id="6700a-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6700a-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6700a-131">JSON Representation</span></span>
<span data-ttu-id="6700a-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6700a-132">Here is a JSON representation of the resource.</span></span>
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






