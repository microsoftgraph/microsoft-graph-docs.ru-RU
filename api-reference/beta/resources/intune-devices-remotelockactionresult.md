---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bda264b7ad029988cf1a9ec0bbe7aa160f613da8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524944"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="c072f-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="c072f-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="c072f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c072f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c072f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c072f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c072f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c072f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c072f-107">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="c072f-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="c072f-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c072f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c072f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c072f-109">Properties</span></span>
|<span data-ttu-id="c072f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c072f-110">Property</span></span>|<span data-ttu-id="c072f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c072f-111">Type</span></span>|<span data-ttu-id="c072f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c072f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c072f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c072f-113">actionName</span></span>|<span data-ttu-id="c072f-114">String</span><span class="sxs-lookup"><span data-stu-id="c072f-114">String</span></span>|<span data-ttu-id="c072f-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c072f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c072f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c072f-116">actionState</span></span>|[<span data-ttu-id="c072f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c072f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c072f-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c072f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c072f-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c072f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c072f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c072f-120">startDateTime</span></span>|<span data-ttu-id="c072f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c072f-121">DateTimeOffset</span></span>|<span data-ttu-id="c072f-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c072f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c072f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c072f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c072f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c072f-124">DateTimeOffset</span></span>|<span data-ttu-id="c072f-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c072f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c072f-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="c072f-126">unlockPin</span></span>|<span data-ttu-id="c072f-127">String</span><span class="sxs-lookup"><span data-stu-id="c072f-127">String</span></span>|<span data-ttu-id="c072f-128">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="c072f-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="c072f-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c072f-129">Relationships</span></span>
<span data-ttu-id="c072f-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c072f-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c072f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c072f-131">JSON Representation</span></span>
<span data-ttu-id="c072f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c072f-132">Here is a JSON representation of the resource.</span></span>
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



