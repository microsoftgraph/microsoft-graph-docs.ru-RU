---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 07b7728677f639fefabd2954f74ff006ff76ef40
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356900"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="8f70c-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="8f70c-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="8f70c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f70c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f70c-105">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="8f70c-105">Reset passcode action result</span></span>


<span data-ttu-id="8f70c-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8f70c-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8f70c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f70c-107">Properties</span></span>
|<span data-ttu-id="8f70c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f70c-108">Property</span></span>|<span data-ttu-id="8f70c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8f70c-109">Type</span></span>|<span data-ttu-id="8f70c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f70c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f70c-111">actionName</span><span class="sxs-lookup"><span data-stu-id="8f70c-111">actionName</span></span>|<span data-ttu-id="8f70c-112">String</span><span class="sxs-lookup"><span data-stu-id="8f70c-112">String</span></span>|<span data-ttu-id="8f70c-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8f70c-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8f70c-114">actionState</span><span class="sxs-lookup"><span data-stu-id="8f70c-114">actionState</span></span>|[<span data-ttu-id="8f70c-115">actionState</span><span class="sxs-lookup"><span data-stu-id="8f70c-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="8f70c-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8f70c-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="8f70c-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="8f70c-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="8f70c-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8f70c-118">startDateTime</span></span>|<span data-ttu-id="8f70c-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f70c-119">DateTimeOffset</span></span>|<span data-ttu-id="8f70c-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="8f70c-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8f70c-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f70c-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="8f70c-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f70c-122">DateTimeOffset</span></span>|<span data-ttu-id="8f70c-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8f70c-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="8f70c-124">passcode</span><span class="sxs-lookup"><span data-stu-id="8f70c-124">passcode</span></span>|<span data-ttu-id="8f70c-125">String</span><span class="sxs-lookup"><span data-stu-id="8f70c-125">String</span></span>|<span data-ttu-id="8f70c-126">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="8f70c-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="8f70c-127">Связи</span><span class="sxs-lookup"><span data-stu-id="8f70c-127">Relationships</span></span>
<span data-ttu-id="8f70c-128">Нет</span><span class="sxs-lookup"><span data-stu-id="8f70c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f70c-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f70c-129">JSON Representation</span></span>
<span data-ttu-id="8f70c-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f70c-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```




