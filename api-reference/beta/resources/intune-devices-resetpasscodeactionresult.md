---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
author: tfitzmac
ms.openlocfilehash: 24d7a6f259f456c742c4317763dd9cefe8d185a9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301114"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="fcf1f-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="fcf1f-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="fcf1f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fcf1f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf1f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcf1f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcf1f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fcf1f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcf1f-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="fcf1f-107">Reset passcode action result</span></span>

<span data-ttu-id="fcf1f-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fcf1f-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fcf1f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fcf1f-109">Properties</span></span>
|<span data-ttu-id="fcf1f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fcf1f-110">Property</span></span>|<span data-ttu-id="fcf1f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fcf1f-111">Type</span></span>|<span data-ttu-id="fcf1f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fcf1f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf1f-113">actionName</span><span class="sxs-lookup"><span data-stu-id="fcf1f-113">actionName</span></span>|<span data-ttu-id="fcf1f-114">String</span><span class="sxs-lookup"><span data-stu-id="fcf1f-114">String</span></span>|<span data-ttu-id="fcf1f-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fcf1f-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fcf1f-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fcf1f-116">actionState</span></span>|[<span data-ttu-id="fcf1f-117">actionState</span><span class="sxs-lookup"><span data-stu-id="fcf1f-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fcf1f-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fcf1f-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fcf1f-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fcf1f-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fcf1f-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf1f-120">startDateTime</span></span>|<span data-ttu-id="fcf1f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf1f-121">DateTimeOffset</span></span>|<span data-ttu-id="fcf1f-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fcf1f-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fcf1f-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf1f-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="fcf1f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf1f-124">DateTimeOffset</span></span>|<span data-ttu-id="fcf1f-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fcf1f-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fcf1f-126">passcode</span><span class="sxs-lookup"><span data-stu-id="fcf1f-126">passcode</span></span>|<span data-ttu-id="fcf1f-127">String</span><span class="sxs-lookup"><span data-stu-id="fcf1f-127">String</span></span>|<span data-ttu-id="fcf1f-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="fcf1f-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="fcf1f-129">Связи</span><span class="sxs-lookup"><span data-stu-id="fcf1f-129">Relationships</span></span>
<span data-ttu-id="fcf1f-130">Нет</span><span class="sxs-lookup"><span data-stu-id="fcf1f-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fcf1f-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fcf1f-131">JSON Representation</span></span>
<span data-ttu-id="fcf1f-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fcf1f-132">Here is a JSON representation of the resource.</span></span>
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





