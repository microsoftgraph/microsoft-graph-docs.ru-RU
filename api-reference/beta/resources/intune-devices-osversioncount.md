---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1ea71a04a87972a1f7375af9458d0a25ab04b49
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725437"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="cf2c1-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="cf2c1-103">osVersionCount resource type</span></span>

<span data-ttu-id="cf2c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf2c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf2c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf2c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf2c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cf2c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf2c1-107">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="cf2c1-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="cf2c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cf2c1-108">Properties</span></span>
|<span data-ttu-id="cf2c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf2c1-109">Property</span></span>|<span data-ttu-id="cf2c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cf2c1-110">Type</span></span>|<span data-ttu-id="cf2c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cf2c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf2c1-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="cf2c1-112">osVersion</span></span>|<span data-ttu-id="cf2c1-113">String</span><span class="sxs-lookup"><span data-stu-id="cf2c1-113">String</span></span>|<span data-ttu-id="cf2c1-114">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="cf2c1-114">OS version</span></span>|
|<span data-ttu-id="cf2c1-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="cf2c1-115">deviceCount</span></span>|<span data-ttu-id="cf2c1-116">Int32</span><span class="sxs-lookup"><span data-stu-id="cf2c1-116">Int32</span></span>|<span data-ttu-id="cf2c1-117">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="cf2c1-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="cf2c1-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cf2c1-118">lastUpdateDateTime</span></span>|<span data-ttu-id="cf2c1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf2c1-119">DateTimeOffset</span></span>|<span data-ttu-id="cf2c1-120">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="cf2c1-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf2c1-121">Связи</span><span class="sxs-lookup"><span data-stu-id="cf2c1-121">Relationships</span></span>
<span data-ttu-id="cf2c1-122">Нет</span><span class="sxs-lookup"><span data-stu-id="cf2c1-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf2c1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cf2c1-123">JSON Representation</span></span>
<span data-ttu-id="cf2c1-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf2c1-124">Here is a JSON representation of the resource.</span></span>
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





