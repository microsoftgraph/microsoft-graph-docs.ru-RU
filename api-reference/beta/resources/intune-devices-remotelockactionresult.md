---
title: Тип ресурса remoteLockActionResult
description: Результат блокирования с ПИН-кодом разблокировки
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0ed8931153c70cea877e8db82ed794301664cbd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937777"
---
# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="c606b-103">Тип ресурса remoteLockActionResult</span><span class="sxs-lookup"><span data-stu-id="c606b-103">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="c606b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c606b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c606b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c606b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c606b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c606b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c606b-107">Результат блокирования с ПИН-кодом разблокировки</span><span class="sxs-lookup"><span data-stu-id="c606b-107">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="c606b-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c606b-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c606b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c606b-109">Properties</span></span>
|<span data-ttu-id="c606b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c606b-110">Property</span></span>|<span data-ttu-id="c606b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c606b-111">Type</span></span>|<span data-ttu-id="c606b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c606b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c606b-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c606b-113">actionName</span></span>|<span data-ttu-id="c606b-114">String</span><span class="sxs-lookup"><span data-stu-id="c606b-114">String</span></span>|<span data-ttu-id="c606b-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c606b-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c606b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c606b-116">actionState</span></span>|[<span data-ttu-id="c606b-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c606b-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c606b-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c606b-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c606b-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c606b-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c606b-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c606b-120">startDateTime</span></span>|<span data-ttu-id="c606b-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c606b-121">DateTimeOffset</span></span>|<span data-ttu-id="c606b-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c606b-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c606b-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c606b-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c606b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c606b-124">DateTimeOffset</span></span>|<span data-ttu-id="c606b-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c606b-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c606b-126">unlockPin</span><span class="sxs-lookup"><span data-stu-id="c606b-126">unlockPin</span></span>|<span data-ttu-id="c606b-127">String</span><span class="sxs-lookup"><span data-stu-id="c606b-127">String</span></span>|<span data-ttu-id="c606b-128">ПИН-код для разблокировки клиента</span><span class="sxs-lookup"><span data-stu-id="c606b-128">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="c606b-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c606b-129">Relationships</span></span>
<span data-ttu-id="c606b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c606b-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c606b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c606b-131">JSON Representation</span></span>
<span data-ttu-id="c606b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c606b-132">Here is a JSON representation of the resource.</span></span>
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





