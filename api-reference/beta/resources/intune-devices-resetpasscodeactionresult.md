---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 90a99b0ad365004365d65ffd7b428e540bcc00a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949915"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="dc363-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="dc363-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="dc363-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dc363-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc363-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc363-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc363-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dc363-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc363-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="dc363-107">Reset passcode action result</span></span>

<span data-ttu-id="dc363-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dc363-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc363-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="dc363-109">Properties</span></span>
|<span data-ttu-id="dc363-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="dc363-110">Property</span></span>|<span data-ttu-id="dc363-111">Тип</span><span class="sxs-lookup"><span data-stu-id="dc363-111">Type</span></span>|<span data-ttu-id="dc363-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dc363-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc363-113">actionName</span><span class="sxs-lookup"><span data-stu-id="dc363-113">actionName</span></span>|<span data-ttu-id="dc363-114">String</span><span class="sxs-lookup"><span data-stu-id="dc363-114">String</span></span>|<span data-ttu-id="dc363-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dc363-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dc363-116">actionState</span><span class="sxs-lookup"><span data-stu-id="dc363-116">actionState</span></span>|[<span data-ttu-id="dc363-117">actionState</span><span class="sxs-lookup"><span data-stu-id="dc363-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="dc363-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="dc363-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="dc363-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="dc363-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dc363-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dc363-120">startDateTime</span></span>|<span data-ttu-id="dc363-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc363-121">DateTimeOffset</span></span>|<span data-ttu-id="dc363-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dc363-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dc363-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc363-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="dc363-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc363-124">DateTimeOffset</span></span>|<span data-ttu-id="dc363-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="dc363-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="dc363-126">passcode</span><span class="sxs-lookup"><span data-stu-id="dc363-126">passcode</span></span>|<span data-ttu-id="dc363-127">String</span><span class="sxs-lookup"><span data-stu-id="dc363-127">String</span></span>|<span data-ttu-id="dc363-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="dc363-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="dc363-129">Связи</span><span class="sxs-lookup"><span data-stu-id="dc363-129">Relationships</span></span>
<span data-ttu-id="dc363-130">Нет</span><span class="sxs-lookup"><span data-stu-id="dc363-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc363-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dc363-131">JSON Representation</span></span>
<span data-ttu-id="dc363-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dc363-132">Here is a JSON representation of the resource.</span></span>
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





