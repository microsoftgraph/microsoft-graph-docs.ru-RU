---
title: Тип ресурса Булкманажеддевицеактионресулт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a7b5e719e837dbd175fa634aea2082f5b0b142b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999992"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="09736-103">Тип ресурса Булкманажеддевицеактионресулт</span><span class="sxs-lookup"><span data-stu-id="09736-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="09736-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09736-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09736-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09736-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09736-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="09736-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="09736-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="09736-107">Properties</span></span>
|<span data-ttu-id="09736-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="09736-108">Property</span></span>|<span data-ttu-id="09736-109">Тип</span><span class="sxs-lookup"><span data-stu-id="09736-109">Type</span></span>|<span data-ttu-id="09736-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09736-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09736-111">Сукцессфулдевицеидс</span><span class="sxs-lookup"><span data-stu-id="09736-111">successfulDeviceIds</span></span>|<span data-ttu-id="09736-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09736-112">String collection</span></span>|<span data-ttu-id="09736-113">Успешное выполнение устройств</span><span class="sxs-lookup"><span data-stu-id="09736-113">Successful devices</span></span>|
|<span data-ttu-id="09736-114">Фаиледдевицеидс</span><span class="sxs-lookup"><span data-stu-id="09736-114">failedDeviceIds</span></span>|<span data-ttu-id="09736-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09736-115">String collection</span></span>|<span data-ttu-id="09736-116">Неисправные устройства</span><span class="sxs-lookup"><span data-stu-id="09736-116">Failed devices</span></span>|
|<span data-ttu-id="09736-117">Нотфаунддевицеидс</span><span class="sxs-lookup"><span data-stu-id="09736-117">notFoundDeviceIds</span></span>|<span data-ttu-id="09736-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09736-118">String collection</span></span>|<span data-ttu-id="09736-119">Устройства не найдены</span><span class="sxs-lookup"><span data-stu-id="09736-119">Not found devices</span></span>|
|<span data-ttu-id="09736-120">Нотсуппортеддевицеидс</span><span class="sxs-lookup"><span data-stu-id="09736-120">notSupportedDeviceIds</span></span>|<span data-ttu-id="09736-121">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="09736-121">String collection</span></span>|<span data-ttu-id="09736-122">Неподдерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="09736-122">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="09736-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="09736-123">Relationships</span></span>
<span data-ttu-id="09736-124">Нет</span><span class="sxs-lookup"><span data-stu-id="09736-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09736-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09736-125">JSON Representation</span></span>
<span data-ttu-id="09736-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09736-126">Here is a JSON representation of the resource.</span></span>
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





