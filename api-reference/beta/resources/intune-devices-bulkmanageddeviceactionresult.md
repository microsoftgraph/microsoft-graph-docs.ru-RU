---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8190071f5ed6e239c2452bc53d802125b71339f5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983367"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="40441-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="40441-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="40441-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40441-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40441-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40441-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40441-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="40441-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="40441-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40441-107">Properties</span></span>
|<span data-ttu-id="40441-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40441-108">Property</span></span>|<span data-ttu-id="40441-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40441-109">Type</span></span>|<span data-ttu-id="40441-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40441-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40441-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="40441-111">successfulDeviceIds</span></span>|<span data-ttu-id="40441-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40441-112">String collection</span></span>|<span data-ttu-id="40441-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="40441-113">Successful devices</span></span>|
|<span data-ttu-id="40441-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="40441-114">failedDeviceIds</span></span>|<span data-ttu-id="40441-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40441-115">String collection</span></span>|<span data-ttu-id="40441-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="40441-116">Failed devices</span></span>|
|<span data-ttu-id="40441-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="40441-117">notFoundDeviceIds</span></span>|<span data-ttu-id="40441-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40441-118">String collection</span></span>|<span data-ttu-id="40441-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="40441-119">Not found devices</span></span>|
|<span data-ttu-id="40441-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="40441-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="40441-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="40441-121">String collection</span></span>|<span data-ttu-id="40441-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="40441-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="40441-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="40441-123">Relationships</span></span>
<span data-ttu-id="40441-124">Нет</span><span class="sxs-lookup"><span data-stu-id="40441-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40441-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40441-125">JSON Representation</span></span>
<span data-ttu-id="40441-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40441-126">Here is a JSON representation of the resource.</span></span>
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





