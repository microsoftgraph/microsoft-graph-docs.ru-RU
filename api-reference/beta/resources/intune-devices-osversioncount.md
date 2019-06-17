---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b8987017012d4db0756fc3d8a78efe99319d68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963914"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="74602-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="74602-103">osVersionCount resource type</span></span>

> <span data-ttu-id="74602-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74602-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74602-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="74602-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74602-106">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="74602-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="74602-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="74602-107">Properties</span></span>
|<span data-ttu-id="74602-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="74602-108">Property</span></span>|<span data-ttu-id="74602-109">Тип</span><span class="sxs-lookup"><span data-stu-id="74602-109">Type</span></span>|<span data-ttu-id="74602-110">Описание</span><span class="sxs-lookup"><span data-stu-id="74602-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74602-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="74602-111">osVersion</span></span>|<span data-ttu-id="74602-112">String</span><span class="sxs-lookup"><span data-stu-id="74602-112">String</span></span>|<span data-ttu-id="74602-113">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="74602-113">OS version</span></span>|
|<span data-ttu-id="74602-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="74602-114">deviceCount</span></span>|<span data-ttu-id="74602-115">Int32</span><span class="sxs-lookup"><span data-stu-id="74602-115">Int32</span></span>|<span data-ttu-id="74602-116">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="74602-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="74602-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="74602-117">lastUpdateDateTime</span></span>|<span data-ttu-id="74602-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74602-118">DateTimeOffset</span></span>|<span data-ttu-id="74602-119">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="74602-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="74602-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="74602-120">Relationships</span></span>
<span data-ttu-id="74602-121">Нет</span><span class="sxs-lookup"><span data-stu-id="74602-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74602-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74602-122">JSON Representation</span></span>
<span data-ttu-id="74602-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74602-123">Here is a JSON representation of the resource.</span></span>
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





