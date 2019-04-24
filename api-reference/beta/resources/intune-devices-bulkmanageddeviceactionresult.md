---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0978367465fde92f9874e338a0de84da2a20403
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467353"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="adf11-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="adf11-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="adf11-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="adf11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="adf11-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="adf11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adf11-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="adf11-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="adf11-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="adf11-107">Properties</span></span>
|<span data-ttu-id="adf11-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="adf11-108">Property</span></span>|<span data-ttu-id="adf11-109">Тип</span><span class="sxs-lookup"><span data-stu-id="adf11-109">Type</span></span>|<span data-ttu-id="adf11-110">Описание</span><span class="sxs-lookup"><span data-stu-id="adf11-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adf11-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="adf11-111">successfulDeviceIds</span></span>|<span data-ttu-id="adf11-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="adf11-112">String collection</span></span>|<span data-ttu-id="adf11-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="adf11-113">Successful devices</span></span>|
|<span data-ttu-id="adf11-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="adf11-114">failedDeviceIds</span></span>|<span data-ttu-id="adf11-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="adf11-115">String collection</span></span>|<span data-ttu-id="adf11-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="adf11-116">Failed devices</span></span>|
|<span data-ttu-id="adf11-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="adf11-117">notFoundDeviceIds</span></span>|<span data-ttu-id="adf11-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="adf11-118">String collection</span></span>|<span data-ttu-id="adf11-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="adf11-119">Not found devices</span></span>|
|<span data-ttu-id="adf11-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="adf11-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="adf11-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="adf11-121">String collection</span></span>|<span data-ttu-id="adf11-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="adf11-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="adf11-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="adf11-123">Relationships</span></span>
<span data-ttu-id="adf11-124">Нет</span><span class="sxs-lookup"><span data-stu-id="adf11-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="adf11-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="adf11-125">JSON Representation</span></span>
<span data-ttu-id="adf11-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adf11-126">Here is a JSON representation of the resource.</span></span>
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





