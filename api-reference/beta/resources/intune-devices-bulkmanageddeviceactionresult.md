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
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="0e412-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="0e412-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="0e412-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e412-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e412-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e412-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e412-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0e412-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e412-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0e412-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0e412-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e412-108">Properties</span></span>
|<span data-ttu-id="0e412-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e412-109">Property</span></span>|<span data-ttu-id="0e412-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0e412-110">Type</span></span>|<span data-ttu-id="0e412-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e412-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e412-112">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="0e412-112">successfulDeviceIds</span></span>|<span data-ttu-id="0e412-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0e412-113">String collection</span></span>|<span data-ttu-id="0e412-114">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="0e412-114">Successful devices</span></span>|
|<span data-ttu-id="0e412-115">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="0e412-115">failedDeviceIds</span></span>|<span data-ttu-id="0e412-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0e412-116">String collection</span></span>|<span data-ttu-id="0e412-117">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="0e412-117">Failed devices</span></span>|
|<span data-ttu-id="0e412-118">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="0e412-118">notFoundDeviceIds</span></span>|<span data-ttu-id="0e412-119">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0e412-119">String collection</span></span>|<span data-ttu-id="0e412-120">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="0e412-120">Not found devices</span></span>|
|<span data-ttu-id="0e412-121">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="0e412-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="0e412-122">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="0e412-122">String collection</span></span>|<span data-ttu-id="0e412-123">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="0e412-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e412-124">Связи</span><span class="sxs-lookup"><span data-stu-id="0e412-124">Relationships</span></span>
<span data-ttu-id="0e412-125">Нет</span><span class="sxs-lookup"><span data-stu-id="0e412-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e412-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e412-126">JSON Representation</span></span>
<span data-ttu-id="0e412-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e412-127">Here is a JSON representation of the resource.</span></span>
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



