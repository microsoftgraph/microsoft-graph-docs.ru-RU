---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 18f9c87e497edef167a69eff67a2dba3571e2d67
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785128"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="af79d-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="af79d-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="af79d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af79d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af79d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af79d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af79d-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="af79d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="af79d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af79d-107">Properties</span></span>
|<span data-ttu-id="af79d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af79d-108">Property</span></span>|<span data-ttu-id="af79d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af79d-109">Type</span></span>|<span data-ttu-id="af79d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af79d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af79d-111">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="af79d-111">successfulDeviceIds</span></span>|<span data-ttu-id="af79d-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af79d-112">String collection</span></span>|<span data-ttu-id="af79d-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="af79d-113">Successful devices</span></span>|
|<span data-ttu-id="af79d-114">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="af79d-114">failedDeviceIds</span></span>|<span data-ttu-id="af79d-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af79d-115">String collection</span></span>|<span data-ttu-id="af79d-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="af79d-116">Failed devices</span></span>|
|<span data-ttu-id="af79d-117">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="af79d-117">notFoundDeviceIds</span></span>|<span data-ttu-id="af79d-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af79d-118">String collection</span></span>|<span data-ttu-id="af79d-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="af79d-119">Not found devices</span></span>|
|<span data-ttu-id="af79d-120">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="af79d-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="af79d-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="af79d-121">String collection</span></span>|<span data-ttu-id="af79d-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="af79d-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="af79d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="af79d-123">Relationships</span></span>
<span data-ttu-id="af79d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="af79d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af79d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af79d-125">JSON Representation</span></span>
<span data-ttu-id="af79d-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af79d-126">Here is a JSON representation of the resource.</span></span>
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



