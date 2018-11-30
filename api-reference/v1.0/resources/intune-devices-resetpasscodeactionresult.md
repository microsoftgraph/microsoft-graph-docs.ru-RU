---
title: Тип ресурса resetPasscodeActionResult
description: Результат сброса секретного кода
ms.openlocfilehash: 6b951a75b93b4e625fb61110ba909632c051b0f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025858"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="08911-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="08911-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="08911-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08911-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08911-105">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="08911-105">Reset passcode action result</span></span>

<span data-ttu-id="08911-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08911-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08911-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="08911-107">Properties</span></span>
|<span data-ttu-id="08911-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="08911-108">Property</span></span>|<span data-ttu-id="08911-109">Тип</span><span class="sxs-lookup"><span data-stu-id="08911-109">Type</span></span>|<span data-ttu-id="08911-110">Описание</span><span class="sxs-lookup"><span data-stu-id="08911-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08911-111">actionName</span><span class="sxs-lookup"><span data-stu-id="08911-111">actionName</span></span>|<span data-ttu-id="08911-112">String</span><span class="sxs-lookup"><span data-stu-id="08911-112">String</span></span>|<span data-ttu-id="08911-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08911-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08911-114">actionState</span><span class="sxs-lookup"><span data-stu-id="08911-114">actionState</span></span>|[<span data-ttu-id="08911-115">actionState</span><span class="sxs-lookup"><span data-stu-id="08911-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="08911-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="08911-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="08911-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="08911-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="08911-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="08911-118">startDateTime</span></span>|<span data-ttu-id="08911-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08911-119">DateTimeOffset</span></span>|<span data-ttu-id="08911-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08911-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08911-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="08911-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="08911-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08911-122">DateTimeOffset</span></span>|<span data-ttu-id="08911-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08911-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08911-124">passcode</span><span class="sxs-lookup"><span data-stu-id="08911-124">passcode</span></span>|<span data-ttu-id="08911-125">String</span><span class="sxs-lookup"><span data-stu-id="08911-125">String</span></span>|<span data-ttu-id="08911-126">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="08911-126">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="08911-127">Связи</span><span class="sxs-lookup"><span data-stu-id="08911-127">Relationships</span></span>
<span data-ttu-id="08911-128">Нет</span><span class="sxs-lookup"><span data-stu-id="08911-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08911-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08911-129">JSON Representation</span></span>
<span data-ttu-id="08911-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08911-130">Here is a JSON representation of the resource.</span></span>
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



