---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c066e87066a766fdef40fc75caa8818a973de4f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943048"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="aff9f-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="aff9f-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="aff9f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aff9f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aff9f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aff9f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aff9f-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="aff9f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="aff9f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="aff9f-107">Properties</span></span>
|<span data-ttu-id="aff9f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="aff9f-108">Property</span></span>|<span data-ttu-id="aff9f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="aff9f-109">Type</span></span>|<span data-ttu-id="aff9f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="aff9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aff9f-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="aff9f-111">successfulDeviceIds</span></span>|<span data-ttu-id="aff9f-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aff9f-112">String collection</span></span>|<span data-ttu-id="aff9f-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="aff9f-113">Successful devices</span></span>|
|<span data-ttu-id="aff9f-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="aff9f-114">failedDeviceIds</span></span>|<span data-ttu-id="aff9f-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aff9f-115">String collection</span></span>|<span data-ttu-id="aff9f-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="aff9f-116">Failed devices</span></span>|
|<span data-ttu-id="aff9f-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="aff9f-117">notFoundDeviceIds</span></span>|<span data-ttu-id="aff9f-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aff9f-118">String collection</span></span>|<span data-ttu-id="aff9f-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="aff9f-119">Not found devices</span></span>|
|<span data-ttu-id="aff9f-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="aff9f-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="aff9f-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="aff9f-121">String collection</span></span>|<span data-ttu-id="aff9f-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="aff9f-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="aff9f-123">Связи</span><span class="sxs-lookup"><span data-stu-id="aff9f-123">Relationships</span></span>
<span data-ttu-id="aff9f-124">Нет</span><span class="sxs-lookup"><span data-stu-id="aff9f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aff9f-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aff9f-125">JSON Representation</span></span>
<span data-ttu-id="aff9f-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aff9f-126">Here is a JSON representation of the resource.</span></span>
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




