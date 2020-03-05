---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 330972424697aed731cd3f1a646505c51cd3f52c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528701"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="c63b8-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="c63b8-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="c63b8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c63b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c63b8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c63b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c63b8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c63b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c63b8-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c63b8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c63b8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c63b8-108">Properties</span></span>
|<span data-ttu-id="c63b8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c63b8-109">Property</span></span>|<span data-ttu-id="c63b8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c63b8-110">Type</span></span>|<span data-ttu-id="c63b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c63b8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c63b8-112">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="c63b8-112">successfulDeviceIds</span></span>|<span data-ttu-id="c63b8-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c63b8-113">String collection</span></span>|<span data-ttu-id="c63b8-114">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="c63b8-114">Successful devices</span></span>|
|<span data-ttu-id="c63b8-115">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="c63b8-115">failedDeviceIds</span></span>|<span data-ttu-id="c63b8-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c63b8-116">String collection</span></span>|<span data-ttu-id="c63b8-117">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="c63b8-117">Failed devices</span></span>|
|<span data-ttu-id="c63b8-118">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="c63b8-118">notFoundDeviceIds</span></span>|<span data-ttu-id="c63b8-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c63b8-119">String collection</span></span>|<span data-ttu-id="c63b8-120">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="c63b8-120">Not found devices</span></span>|
|<span data-ttu-id="c63b8-121">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="c63b8-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="c63b8-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c63b8-122">String collection</span></span>|<span data-ttu-id="c63b8-123">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="c63b8-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="c63b8-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c63b8-124">Relationships</span></span>
<span data-ttu-id="c63b8-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c63b8-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c63b8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c63b8-126">JSON Representation</span></span>
<span data-ttu-id="c63b8-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c63b8-127">Here is a JSON representation of the resource.</span></span>
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



