---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ead49e3c73dc65ebbc139fc7d1fd37743fe98be3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844711"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="4b7b6-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="4b7b6-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="4b7b6-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b7b6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b7b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b7b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b7b6-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b7b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b7b6-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="4b7b6-107">Reset passcode action result</span></span>

<span data-ttu-id="4b7b6-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4b7b6-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b7b6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b7b6-109">Properties</span></span>
|<span data-ttu-id="4b7b6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b7b6-110">Property</span></span>|<span data-ttu-id="4b7b6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4b7b6-111">Type</span></span>|<span data-ttu-id="4b7b6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4b7b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b7b6-113">actionName</span><span class="sxs-lookup"><span data-stu-id="4b7b6-113">actionName</span></span>|<span data-ttu-id="4b7b6-114">String</span><span class="sxs-lookup"><span data-stu-id="4b7b6-114">String</span></span>|<span data-ttu-id="4b7b6-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4b7b6-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4b7b6-116">actionState</span><span class="sxs-lookup"><span data-stu-id="4b7b6-116">actionState</span></span>|[<span data-ttu-id="4b7b6-117">actionState</span><span class="sxs-lookup"><span data-stu-id="4b7b6-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4b7b6-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="4b7b6-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="4b7b6-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4b7b6-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="4b7b6-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7b6-120">startDateTime</span></span>|<span data-ttu-id="4b7b6-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b7b6-121">DateTimeOffset</span></span>|<span data-ttu-id="4b7b6-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4b7b6-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4b7b6-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b7b6-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="4b7b6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b7b6-124">DateTimeOffset</span></span>|<span data-ttu-id="4b7b6-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="4b7b6-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="4b7b6-126">passcode</span><span class="sxs-lookup"><span data-stu-id="4b7b6-126">passcode</span></span>|<span data-ttu-id="4b7b6-127">String</span><span class="sxs-lookup"><span data-stu-id="4b7b6-127">String</span></span>|<span data-ttu-id="4b7b6-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="4b7b6-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="4b7b6-129">Связи</span><span class="sxs-lookup"><span data-stu-id="4b7b6-129">Relationships</span></span>
<span data-ttu-id="4b7b6-130">Нет</span><span class="sxs-lookup"><span data-stu-id="4b7b6-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b7b6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b7b6-131">JSON Representation</span></span>
<span data-ttu-id="4b7b6-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b7b6-132">Here is a JSON representation of the resource.</span></span>
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





