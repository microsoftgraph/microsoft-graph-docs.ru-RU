---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e1c4e19212e5f4e54abf90cd22942160d0f1ce24
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611876"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="7c1a2-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="7c1a2-103">remoteLockActionResult resource type</span></span>

<span data-ttu-id="7c1a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c1a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c1a2-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c1a2-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c1a2-107">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="7c1a2-107">Lock action result with a pin to unlock</span></span>


<span data-ttu-id="7c1a2-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7c1a2-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c1a2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c1a2-109">Properties</span></span>
|<span data-ttu-id="7c1a2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c1a2-110">Property</span></span>|<span data-ttu-id="7c1a2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7c1a2-111">Type</span></span>|<span data-ttu-id="7c1a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7c1a2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c1a2-113">actionName</span><span class="sxs-lookup"><span data-stu-id="7c1a2-113">actionName</span></span>|<span data-ttu-id="7c1a2-114">String</span><span class="sxs-lookup"><span data-stu-id="7c1a2-114">String</span></span>|<span data-ttu-id="7c1a2-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7c1a2-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7c1a2-116">actionState</span><span class="sxs-lookup"><span data-stu-id="7c1a2-116">actionState</span></span>|[<span data-ttu-id="7c1a2-117">actionState</span><span class="sxs-lookup"><span data-stu-id="7c1a2-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7c1a2-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7c1a2-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7c1a2-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7c1a2-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7c1a2-120">startDateTime</span></span>|<span data-ttu-id="7c1a2-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c1a2-121">DateTimeOffset</span></span>|<span data-ttu-id="7c1a2-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7c1a2-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7c1a2-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c1a2-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="7c1a2-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c1a2-124">DateTimeOffset</span></span>|<span data-ttu-id="7c1a2-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7c1a2-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7c1a2-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="7c1a2-126">unlockPin</span></span>|<span data-ttu-id="7c1a2-127">String</span><span class="sxs-lookup"><span data-stu-id="7c1a2-127">String</span></span>|<span data-ttu-id="7c1a2-128">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="7c1a2-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c1a2-129">Связи</span><span class="sxs-lookup"><span data-stu-id="7c1a2-129">Relationships</span></span>
<span data-ttu-id="7c1a2-130">Нет</span><span class="sxs-lookup"><span data-stu-id="7c1a2-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c1a2-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c1a2-131">JSON Representation</span></span>
<span data-ttu-id="7c1a2-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c1a2-132">Here is a JSON representation of the resource.</span></span>
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




