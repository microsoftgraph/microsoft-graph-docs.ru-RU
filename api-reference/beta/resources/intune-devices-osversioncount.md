---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6408ee1cef68ade4ccb1c8b90f91ca99a5b75bf4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230900"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="163e8-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="163e8-103">osVersionCount resource type</span></span>

<span data-ttu-id="163e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="163e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="163e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="163e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="163e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="163e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163e8-107">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="163e8-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="163e8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="163e8-108">Properties</span></span>
|<span data-ttu-id="163e8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="163e8-109">Property</span></span>|<span data-ttu-id="163e8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="163e8-110">Type</span></span>|<span data-ttu-id="163e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="163e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163e8-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="163e8-112">osVersion</span></span>|<span data-ttu-id="163e8-113">String</span><span class="sxs-lookup"><span data-stu-id="163e8-113">String</span></span>|<span data-ttu-id="163e8-114">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="163e8-114">OS version</span></span>|
|<span data-ttu-id="163e8-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="163e8-115">deviceCount</span></span>|<span data-ttu-id="163e8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="163e8-116">Int32</span></span>|<span data-ttu-id="163e8-117">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="163e8-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="163e8-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="163e8-118">lastUpdateDateTime</span></span>|<span data-ttu-id="163e8-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163e8-119">DateTimeOffset</span></span>|<span data-ttu-id="163e8-120">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="163e8-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="163e8-121">Связи</span><span class="sxs-lookup"><span data-stu-id="163e8-121">Relationships</span></span>
<span data-ttu-id="163e8-122">Нет</span><span class="sxs-lookup"><span data-stu-id="163e8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="163e8-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="163e8-123">JSON Representation</span></span>
<span data-ttu-id="163e8-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="163e8-124">Here is a JSON representation of the resource.</span></span>
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




