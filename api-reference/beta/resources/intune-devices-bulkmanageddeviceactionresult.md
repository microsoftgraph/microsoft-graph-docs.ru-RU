---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 199fe08b4eaf339f17fdb67bb6dbcc0243fd90f9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168336"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="21ba4-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="21ba4-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="21ba4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21ba4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21ba4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21ba4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21ba4-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="21ba4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="21ba4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="21ba4-107">Properties</span></span>
|<span data-ttu-id="21ba4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="21ba4-108">Property</span></span>|<span data-ttu-id="21ba4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="21ba4-109">Type</span></span>|<span data-ttu-id="21ba4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="21ba4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ba4-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="21ba4-111">successfulDeviceIds</span></span>|<span data-ttu-id="21ba4-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21ba4-112">String collection</span></span>|<span data-ttu-id="21ba4-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="21ba4-113">Successful devices</span></span>|
|<span data-ttu-id="21ba4-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="21ba4-114">failedDeviceIds</span></span>|<span data-ttu-id="21ba4-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21ba4-115">String collection</span></span>|<span data-ttu-id="21ba4-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="21ba4-116">Failed devices</span></span>|
|<span data-ttu-id="21ba4-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="21ba4-117">notFoundDeviceIds</span></span>|<span data-ttu-id="21ba4-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21ba4-118">String collection</span></span>|<span data-ttu-id="21ba4-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="21ba4-119">Not found devices</span></span>|
|<span data-ttu-id="21ba4-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="21ba4-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="21ba4-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="21ba4-121">String collection</span></span>|<span data-ttu-id="21ba4-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="21ba4-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="21ba4-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="21ba4-123">Relationships</span></span>
<span data-ttu-id="21ba4-124">Нет</span><span class="sxs-lookup"><span data-stu-id="21ba4-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21ba4-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21ba4-125">JSON Representation</span></span>
<span data-ttu-id="21ba4-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21ba4-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```




