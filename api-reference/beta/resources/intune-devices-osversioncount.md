---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4654f49d6d58d07dbb349edf38d4336da82a4aeb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783923"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="8f53e-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="8f53e-103">osVersionCount resource type</span></span>

> <span data-ttu-id="8f53e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f53e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f53e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f53e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f53e-106">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="8f53e-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="8f53e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f53e-107">Properties</span></span>
|<span data-ttu-id="8f53e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f53e-108">Property</span></span>|<span data-ttu-id="8f53e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8f53e-109">Type</span></span>|<span data-ttu-id="8f53e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8f53e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f53e-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="8f53e-111">osVersion</span></span>|<span data-ttu-id="8f53e-112">String</span><span class="sxs-lookup"><span data-stu-id="8f53e-112">String</span></span>|<span data-ttu-id="8f53e-113">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="8f53e-113">OS version</span></span>|
|<span data-ttu-id="8f53e-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="8f53e-114">deviceCount</span></span>|<span data-ttu-id="8f53e-115">Int32</span><span class="sxs-lookup"><span data-stu-id="8f53e-115">Int32</span></span>|<span data-ttu-id="8f53e-116">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="8f53e-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="8f53e-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="8f53e-117">lastUpdateDateTime</span></span>|<span data-ttu-id="8f53e-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f53e-118">DateTimeOffset</span></span>|<span data-ttu-id="8f53e-119">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="8f53e-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f53e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="8f53e-120">Relationships</span></span>
<span data-ttu-id="8f53e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8f53e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f53e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f53e-122">JSON Representation</span></span>
<span data-ttu-id="8f53e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f53e-123">Here is a JSON representation of the resource.</span></span>
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



