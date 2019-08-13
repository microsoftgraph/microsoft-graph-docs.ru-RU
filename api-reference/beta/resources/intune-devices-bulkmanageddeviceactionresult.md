---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1f260b032078bdcd60000ecbde315a91cfcf492
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337596"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="8b496-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="8b496-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="8b496-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b496-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b496-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b496-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b496-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="8b496-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8b496-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b496-107">Properties</span></span>
|<span data-ttu-id="8b496-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b496-108">Property</span></span>|<span data-ttu-id="8b496-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b496-109">Type</span></span>|<span data-ttu-id="8b496-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b496-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b496-111">сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="8b496-111">successfulDeviceIds</span></span>|<span data-ttu-id="8b496-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b496-112">String collection</span></span>|<span data-ttu-id="8b496-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="8b496-113">Successful devices</span></span>|
|<span data-ttu-id="8b496-114">фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="8b496-114">failedDeviceIds</span></span>|<span data-ttu-id="8b496-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b496-115">String collection</span></span>|<span data-ttu-id="8b496-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="8b496-116">Failed devices</span></span>|
|<span data-ttu-id="8b496-117">нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="8b496-117">notFoundDeviceIds</span></span>|<span data-ttu-id="8b496-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b496-118">String collection</span></span>|<span data-ttu-id="8b496-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="8b496-119">Not found devices</span></span>|
|<span data-ttu-id="8b496-120">нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="8b496-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="8b496-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b496-121">String collection</span></span>|<span data-ttu-id="8b496-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="8b496-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b496-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b496-123">Relationships</span></span>
<span data-ttu-id="8b496-124">Нет</span><span class="sxs-lookup"><span data-stu-id="8b496-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b496-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b496-125">JSON Representation</span></span>
<span data-ttu-id="8b496-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b496-126">Here is a JSON representation of the resource.</span></span>
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



