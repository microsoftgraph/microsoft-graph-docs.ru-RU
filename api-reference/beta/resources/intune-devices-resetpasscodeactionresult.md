---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e7ff89fb85192a873595cb362c3e6031b834a7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524937"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="fdc7d-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="fdc7d-103">resetPasscodeActionResult resource type</span></span>

<span data-ttu-id="fdc7d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fdc7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fdc7d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fdc7d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc7d-107">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="fdc7d-107">Reset passcode action result</span></span>


<span data-ttu-id="fdc7d-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fdc7d-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fdc7d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fdc7d-109">Properties</span></span>
|<span data-ttu-id="fdc7d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdc7d-110">Property</span></span>|<span data-ttu-id="fdc7d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fdc7d-111">Type</span></span>|<span data-ttu-id="fdc7d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fdc7d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc7d-113">actionName</span><span class="sxs-lookup"><span data-stu-id="fdc7d-113">actionName</span></span>|<span data-ttu-id="fdc7d-114">String</span><span class="sxs-lookup"><span data-stu-id="fdc7d-114">String</span></span>|<span data-ttu-id="fdc7d-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fdc7d-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fdc7d-116">actionState</span><span class="sxs-lookup"><span data-stu-id="fdc7d-116">actionState</span></span>|[<span data-ttu-id="fdc7d-117">actionState</span><span class="sxs-lookup"><span data-stu-id="fdc7d-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="fdc7d-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fdc7d-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="fdc7d-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="fdc7d-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc7d-120">startDateTime</span></span>|<span data-ttu-id="fdc7d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc7d-121">DateTimeOffset</span></span>|<span data-ttu-id="fdc7d-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="fdc7d-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fdc7d-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fdc7d-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="fdc7d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fdc7d-124">DateTimeOffset</span></span>|<span data-ttu-id="fdc7d-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="fdc7d-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="fdc7d-126">passcode</span><span class="sxs-lookup"><span data-stu-id="fdc7d-126">passcode</span></span>|<span data-ttu-id="fdc7d-127">String</span><span class="sxs-lookup"><span data-stu-id="fdc7d-127">String</span></span>|<span data-ttu-id="fdc7d-128">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="fdc7d-128">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="fdc7d-129">Связи</span><span class="sxs-lookup"><span data-stu-id="fdc7d-129">Relationships</span></span>
<span data-ttu-id="fdc7d-130">Нет</span><span class="sxs-lookup"><span data-stu-id="fdc7d-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdc7d-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fdc7d-131">JSON Representation</span></span>
<span data-ttu-id="fdc7d-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdc7d-132">Here is a JSON representation of the resource.</span></span>
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



