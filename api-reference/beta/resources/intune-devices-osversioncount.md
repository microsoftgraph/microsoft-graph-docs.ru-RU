---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864150"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="1a006-103">Тип ресурса osVersionCount</span><span class="sxs-lookup"><span data-stu-id="1a006-103">osVersionCount resource type</span></span>

> <span data-ttu-id="1a006-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1a006-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a006-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1a006-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a006-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1a006-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a006-107">Количество устройств с вредоносных программ для каждой версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="1a006-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="1a006-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a006-108">Properties</span></span>
|<span data-ttu-id="1a006-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a006-109">Property</span></span>|<span data-ttu-id="1a006-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1a006-110">Type</span></span>|<span data-ttu-id="1a006-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1a006-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a006-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="1a006-112">osVersion</span></span>|<span data-ttu-id="1a006-113">String</span><span class="sxs-lookup"><span data-stu-id="1a006-113">String</span></span>|<span data-ttu-id="1a006-114">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="1a006-114">OS version</span></span>|
|<span data-ttu-id="1a006-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1a006-115">deviceCount</span></span>|<span data-ttu-id="1a006-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1a006-116">Int32</span></span>|<span data-ttu-id="1a006-117">Количество устройств с вредоносных программ для версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="1a006-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="1a006-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1a006-118">lastUpdateDateTime</span></span>|<span data-ttu-id="1a006-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a006-119">DateTimeOffset</span></span>|<span data-ttu-id="1a006-120">Метка времени последнего обновления для счетчик устройства в формате UTC</span><span class="sxs-lookup"><span data-stu-id="1a006-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a006-121">Связи</span><span class="sxs-lookup"><span data-stu-id="1a006-121">Relationships</span></span>
<span data-ttu-id="1a006-122">Нет</span><span class="sxs-lookup"><span data-stu-id="1a006-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1a006-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1a006-123">JSON Representation</span></span>
<span data-ttu-id="1a006-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a006-124">Here is a JSON representation of the resource.</span></span>
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





