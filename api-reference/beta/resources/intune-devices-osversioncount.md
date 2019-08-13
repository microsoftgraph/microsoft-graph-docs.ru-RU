---
title: Тип ресурса Осверсионкаунт
description: Количество устройств с вредоносной программой для каждой версии ОС
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9302a9604c10db0f462eac1de2caab42a933588
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372533"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="689b4-103">Тип ресурса Осверсионкаунт</span><span class="sxs-lookup"><span data-stu-id="689b4-103">osVersionCount resource type</span></span>

> <span data-ttu-id="689b4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="689b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689b4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="689b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689b4-106">Количество устройств с вредоносной программой для каждой версии ОС</span><span class="sxs-lookup"><span data-stu-id="689b4-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="689b4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="689b4-107">Properties</span></span>
|<span data-ttu-id="689b4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="689b4-108">Property</span></span>|<span data-ttu-id="689b4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="689b4-109">Type</span></span>|<span data-ttu-id="689b4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="689b4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689b4-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="689b4-111">osVersion</span></span>|<span data-ttu-id="689b4-112">String</span><span class="sxs-lookup"><span data-stu-id="689b4-112">String</span></span>|<span data-ttu-id="689b4-113">Версия ОС</span><span class="sxs-lookup"><span data-stu-id="689b4-113">OS version</span></span>|
|<span data-ttu-id="689b4-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="689b4-114">deviceCount</span></span>|<span data-ttu-id="689b4-115">Int32</span><span class="sxs-lookup"><span data-stu-id="689b4-115">Int32</span></span>|<span data-ttu-id="689b4-116">Количество устройств с вредоносной программой для версии ОС</span><span class="sxs-lookup"><span data-stu-id="689b4-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="689b4-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="689b4-117">lastUpdateDateTime</span></span>|<span data-ttu-id="689b4-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="689b4-118">DateTimeOffset</span></span>|<span data-ttu-id="689b4-119">Метка времени последнего обновления числа устройств в формате UTC</span><span class="sxs-lookup"><span data-stu-id="689b4-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="689b4-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="689b4-120">Relationships</span></span>
<span data-ttu-id="689b4-121">Нет</span><span class="sxs-lookup"><span data-stu-id="689b4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="689b4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="689b4-122">JSON Representation</span></span>
<span data-ttu-id="689b4-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="689b4-123">Here is a JSON representation of the resource.</span></span>
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



