---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0978367465fde92f9874e338a0de84da2a20403
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31770937"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="d50f5-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="d50f5-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="d50f5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d50f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d50f5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d50f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d50f5-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="d50f5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d50f5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d50f5-107">Properties</span></span>
|<span data-ttu-id="d50f5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d50f5-108">Property</span></span>|<span data-ttu-id="d50f5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d50f5-109">Type</span></span>|<span data-ttu-id="d50f5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d50f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50f5-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="d50f5-111">successfulDeviceIds</span></span>|<span data-ttu-id="d50f5-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50f5-112">String collection</span></span>|<span data-ttu-id="d50f5-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="d50f5-113">Successful devices</span></span>|
|<span data-ttu-id="d50f5-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="d50f5-114">failedDeviceIds</span></span>|<span data-ttu-id="d50f5-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50f5-115">String collection</span></span>|<span data-ttu-id="d50f5-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="d50f5-116">Failed devices</span></span>|
|<span data-ttu-id="d50f5-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="d50f5-117">notFoundDeviceIds</span></span>|<span data-ttu-id="d50f5-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50f5-118">String collection</span></span>|<span data-ttu-id="d50f5-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="d50f5-119">Not found devices</span></span>|
|<span data-ttu-id="d50f5-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="d50f5-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="d50f5-121">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d50f5-121">String collection</span></span>|<span data-ttu-id="d50f5-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="d50f5-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50f5-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="d50f5-123">Relationships</span></span>
<span data-ttu-id="d50f5-124">Нет</span><span class="sxs-lookup"><span data-stu-id="d50f5-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d50f5-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d50f5-125">JSON Representation</span></span>
<span data-ttu-id="d50f5-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d50f5-126">Here is a JSON representation of the resource.</span></span>
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





