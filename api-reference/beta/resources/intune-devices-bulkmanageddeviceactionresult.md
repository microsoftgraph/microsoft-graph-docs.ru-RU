---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae016986f8c3216156a4855f06aa77929e6acefc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299505"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="3f789-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="3f789-103">bulkManagedDeviceActionResult resource type</span></span>

<span data-ttu-id="3f789-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f789-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f789-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f789-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3f789-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3f789-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f789-108">Properties</span></span>
|<span data-ttu-id="3f789-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f789-109">Property</span></span>|<span data-ttu-id="3f789-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3f789-110">Type</span></span>|<span data-ttu-id="3f789-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3f789-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f789-112">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="3f789-112">successfulDeviceIds</span></span>|<span data-ttu-id="3f789-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f789-113">String collection</span></span>|<span data-ttu-id="3f789-114">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="3f789-114">Successful devices</span></span>|
|<span data-ttu-id="3f789-115">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="3f789-115">failedDeviceIds</span></span>|<span data-ttu-id="3f789-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f789-116">String collection</span></span>|<span data-ttu-id="3f789-117">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="3f789-117">Failed devices</span></span>|
|<span data-ttu-id="3f789-118">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="3f789-118">notFoundDeviceIds</span></span>|<span data-ttu-id="3f789-119">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f789-119">String collection</span></span>|<span data-ttu-id="3f789-120">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="3f789-120">Not found devices</span></span>|
|<span data-ttu-id="3f789-121">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="3f789-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="3f789-122">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="3f789-122">String collection</span></span>|<span data-ttu-id="3f789-123">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="3f789-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f789-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3f789-124">Relationships</span></span>
<span data-ttu-id="3f789-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3f789-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f789-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f789-126">JSON Representation</span></span>
<span data-ttu-id="3f789-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f789-127">Here is a JSON representation of the resource.</span></span>
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




