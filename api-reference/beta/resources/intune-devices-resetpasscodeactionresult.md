---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5c022d2531bd1576ab7e336193d2f488f5f89f98
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407048"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="db2a6-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="db2a6-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="db2a6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db2a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="db2a6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db2a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db2a6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db2a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db2a6-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="db2a6-107">Reset passcode action result</span></span>


<span data-ttu-id="db2a6-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db2a6-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db2a6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="db2a6-109">Properties</span></span>
|<span data-ttu-id="db2a6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="db2a6-110">Property</span></span>|<span data-ttu-id="db2a6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="db2a6-111">Type</span></span>|<span data-ttu-id="db2a6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="db2a6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db2a6-113">actionName</span><span class="sxs-lookup"><span data-stu-id="db2a6-113">actionName</span></span>|<span data-ttu-id="db2a6-114">String</span><span class="sxs-lookup"><span data-stu-id="db2a6-114">String</span></span>|<span data-ttu-id="db2a6-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db2a6-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db2a6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="db2a6-116">actionState</span></span>|[<span data-ttu-id="db2a6-117">actionState</span><span class="sxs-lookup"><span data-stu-id="db2a6-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="db2a6-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="db2a6-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="db2a6-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="db2a6-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="db2a6-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="db2a6-120">startDateTime</span></span>|<span data-ttu-id="db2a6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db2a6-121">DateTimeOffset</span></span>|<span data-ttu-id="db2a6-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db2a6-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db2a6-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="db2a6-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="db2a6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db2a6-124">DateTimeOffset</span></span>|<span data-ttu-id="db2a6-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="db2a6-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="db2a6-126">passcode</span><span class="sxs-lookup"><span data-stu-id="db2a6-126">passcode</span></span>|<span data-ttu-id="db2a6-127">String</span><span class="sxs-lookup"><span data-stu-id="db2a6-127">String</span></span>|<span data-ttu-id="db2a6-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="db2a6-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="db2a6-129">Связи</span><span class="sxs-lookup"><span data-stu-id="db2a6-129">Relationships</span></span>
<span data-ttu-id="db2a6-130">Нет</span><span class="sxs-lookup"><span data-stu-id="db2a6-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db2a6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db2a6-131">JSON Representation</span></span>
<span data-ttu-id="db2a6-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db2a6-132">Here is a JSON representation of the resource.</span></span>
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




