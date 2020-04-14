---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b727be90c5fab9966b4a81179c8c9fa65279e0a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443865"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="a0405-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="a0405-103">osVersionCount resource type</span></span>

<span data-ttu-id="a0405-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0405-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0405-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a0405-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0405-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a0405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0405-107">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="a0405-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="a0405-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0405-108">Properties</span></span>
|<span data-ttu-id="a0405-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0405-109">Property</span></span>|<span data-ttu-id="a0405-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a0405-110">Type</span></span>|<span data-ttu-id="a0405-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a0405-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0405-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="a0405-112">osVersion</span></span>|<span data-ttu-id="a0405-113">String</span><span class="sxs-lookup"><span data-stu-id="a0405-113">String</span></span>|<span data-ttu-id="a0405-114">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="a0405-114">OS version</span></span>|
|<span data-ttu-id="a0405-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a0405-115">deviceCount</span></span>|<span data-ttu-id="a0405-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a0405-116">Int32</span></span>|<span data-ttu-id="a0405-117">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="a0405-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="a0405-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a0405-118">lastUpdateDateTime</span></span>|<span data-ttu-id="a0405-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0405-119">DateTimeOffset</span></span>|<span data-ttu-id="a0405-120">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="a0405-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0405-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a0405-121">Relationships</span></span>
<span data-ttu-id="a0405-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a0405-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0405-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0405-123">JSON Representation</span></span>
<span data-ttu-id="a0405-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0405-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```



