---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b661577af3bcd1282a007555c25eb60b121ce539
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465190"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="91911-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="91911-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="91911-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91911-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91911-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91911-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91911-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91911-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91911-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="91911-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="91911-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91911-108">Properties</span></span>
|<span data-ttu-id="91911-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91911-109">Property</span></span>|<span data-ttu-id="91911-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91911-110">Type</span></span>|<span data-ttu-id="91911-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91911-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91911-112">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="91911-112">successfulDeviceIds</span></span>|<span data-ttu-id="91911-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91911-113">String collection</span></span>|<span data-ttu-id="91911-114">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="91911-114">Successful devices</span></span>|
|<span data-ttu-id="91911-115">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="91911-115">failedDeviceIds</span></span>|<span data-ttu-id="91911-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91911-116">String collection</span></span>|<span data-ttu-id="91911-117">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="91911-117">Failed devices</span></span>|
|<span data-ttu-id="91911-118">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="91911-118">notFoundDeviceIds</span></span>|<span data-ttu-id="91911-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91911-119">String collection</span></span>|<span data-ttu-id="91911-120">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="91911-120">Not found devices</span></span>|
|<span data-ttu-id="91911-121">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="91911-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="91911-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91911-122">String collection</span></span>|<span data-ttu-id="91911-123">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="91911-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="91911-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="91911-124">Relationships</span></span>
<span data-ttu-id="91911-125">Нет</span><span class="sxs-lookup"><span data-stu-id="91911-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91911-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91911-126">JSON Representation</span></span>
<span data-ttu-id="91911-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91911-127">Here is a JSON representation of the resource.</span></span>
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



