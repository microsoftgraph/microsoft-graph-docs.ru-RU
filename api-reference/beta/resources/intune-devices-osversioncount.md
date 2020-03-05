---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4a75ac62e0744b621300fc5474cfefe0823cab8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524958"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="e7589-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="e7589-103">osVersionCount resource type</span></span>

<span data-ttu-id="e7589-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e7589-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7589-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e7589-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7589-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e7589-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7589-107">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="e7589-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="e7589-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7589-108">Properties</span></span>
|<span data-ttu-id="e7589-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7589-109">Property</span></span>|<span data-ttu-id="e7589-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e7589-110">Type</span></span>|<span data-ttu-id="e7589-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e7589-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7589-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="e7589-112">osVersion</span></span>|<span data-ttu-id="e7589-113">String</span><span class="sxs-lookup"><span data-stu-id="e7589-113">String</span></span>|<span data-ttu-id="e7589-114">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="e7589-114">OS version</span></span>|
|<span data-ttu-id="e7589-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e7589-115">deviceCount</span></span>|<span data-ttu-id="e7589-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e7589-116">Int32</span></span>|<span data-ttu-id="e7589-117">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="e7589-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="e7589-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e7589-118">lastUpdateDateTime</span></span>|<span data-ttu-id="e7589-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7589-119">DateTimeOffset</span></span>|<span data-ttu-id="e7589-120">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="e7589-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7589-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e7589-121">Relationships</span></span>
<span data-ttu-id="e7589-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e7589-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7589-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e7589-123">JSON Representation</span></span>
<span data-ttu-id="e7589-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7589-124">Here is a JSON representation of the resource.</span></span>
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



