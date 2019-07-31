---
title: Тип ресурса resetPasscodeActionResult
description: Результат действия "Сброс секретного кода"
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 883818d7061f070f01f3e3c9fdfee9e15f322829
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968262"
---
# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="14937-103">Тип ресурса resetPasscodeActionResult</span><span class="sxs-lookup"><span data-stu-id="14937-103">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="14937-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14937-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14937-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="14937-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14937-106">Результат сброса секретного кода</span><span class="sxs-lookup"><span data-stu-id="14937-106">Reset passcode action result</span></span>


<span data-ttu-id="14937-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="14937-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="14937-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="14937-108">Properties</span></span>
|<span data-ttu-id="14937-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="14937-109">Property</span></span>|<span data-ttu-id="14937-110">Тип</span><span class="sxs-lookup"><span data-stu-id="14937-110">Type</span></span>|<span data-ttu-id="14937-111">Описание</span><span class="sxs-lookup"><span data-stu-id="14937-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14937-112">actionName</span><span class="sxs-lookup"><span data-stu-id="14937-112">actionName</span></span>|<span data-ttu-id="14937-113">String</span><span class="sxs-lookup"><span data-stu-id="14937-113">String</span></span>|<span data-ttu-id="14937-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="14937-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="14937-115">actionState</span><span class="sxs-lookup"><span data-stu-id="14937-115">actionState</span></span>|[<span data-ttu-id="14937-116">actionState</span><span class="sxs-lookup"><span data-stu-id="14937-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="14937-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="14937-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="14937-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="14937-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="14937-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="14937-119">startDateTime</span></span>|<span data-ttu-id="14937-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14937-120">DateTimeOffset</span></span>|<span data-ttu-id="14937-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="14937-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="14937-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="14937-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="14937-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14937-123">DateTimeOffset</span></span>|<span data-ttu-id="14937-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="14937-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="14937-125">passcode</span><span class="sxs-lookup"><span data-stu-id="14937-125">passcode</span></span>|<span data-ttu-id="14937-126">String</span><span class="sxs-lookup"><span data-stu-id="14937-126">String</span></span>|<span data-ttu-id="14937-127">Новый секретный код для устройства</span><span class="sxs-lookup"><span data-stu-id="14937-127">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="14937-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="14937-128">Relationships</span></span>
<span data-ttu-id="14937-129">Нет</span><span class="sxs-lookup"><span data-stu-id="14937-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14937-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14937-130">JSON Representation</span></span>
<span data-ttu-id="14937-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14937-131">Here is a JSON representation of the resource.</span></span>
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





