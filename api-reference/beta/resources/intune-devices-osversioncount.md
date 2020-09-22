---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2243c5c9897e108701b1729832562b781d63ec51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081148"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="5f1e4-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="5f1e4-103">osVersionCount resource type</span></span>

<span data-ttu-id="5f1e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f1e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f1e4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f1e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f1e4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f1e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f1e4-107">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="5f1e4-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="5f1e4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f1e4-108">Properties</span></span>
|<span data-ttu-id="5f1e4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f1e4-109">Property</span></span>|<span data-ttu-id="5f1e4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5f1e4-110">Type</span></span>|<span data-ttu-id="5f1e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f1e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1e4-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="5f1e4-112">osVersion</span></span>|<span data-ttu-id="5f1e4-113">String</span><span class="sxs-lookup"><span data-stu-id="5f1e4-113">String</span></span>|<span data-ttu-id="5f1e4-114">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="5f1e4-114">OS version</span></span>|
|<span data-ttu-id="5f1e4-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5f1e4-115">deviceCount</span></span>|<span data-ttu-id="5f1e4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5f1e4-116">Int32</span></span>|<span data-ttu-id="5f1e4-117">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="5f1e4-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="5f1e4-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5f1e4-118">lastUpdateDateTime</span></span>|<span data-ttu-id="5f1e4-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f1e4-119">DateTimeOffset</span></span>|<span data-ttu-id="5f1e4-120">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="5f1e4-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f1e4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="5f1e4-121">Relationships</span></span>
<span data-ttu-id="5f1e4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="5f1e4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f1e4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f1e4-123">JSON Representation</span></span>
<span data-ttu-id="5f1e4-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f1e4-124">Here is a JSON representation of the resource.</span></span>
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






