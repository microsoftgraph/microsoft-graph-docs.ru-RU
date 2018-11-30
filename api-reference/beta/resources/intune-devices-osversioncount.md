---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
ms.openlocfilehash: 7892761bd0dc20f09ab2deb47549aeb157e25644
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080900"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="77f14-103">Тип ресурса osVersionCount</span><span class="sxs-lookup"><span data-stu-id="77f14-103">osVersionCount resource type</span></span>

> <span data-ttu-id="77f14-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="77f14-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77f14-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77f14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77f14-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="77f14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77f14-107">Количество устройств с вредоносных программ для каждой версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="77f14-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="77f14-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="77f14-108">Properties</span></span>
|<span data-ttu-id="77f14-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="77f14-109">Property</span></span>|<span data-ttu-id="77f14-110">Тип</span><span class="sxs-lookup"><span data-stu-id="77f14-110">Type</span></span>|<span data-ttu-id="77f14-111">Description</span><span class="sxs-lookup"><span data-stu-id="77f14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f14-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="77f14-112">osVersion</span></span>|<span data-ttu-id="77f14-113">String</span><span class="sxs-lookup"><span data-stu-id="77f14-113">String</span></span>|<span data-ttu-id="77f14-114">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="77f14-114">OS version</span></span>|
|<span data-ttu-id="77f14-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="77f14-115">deviceCount</span></span>|<span data-ttu-id="77f14-116">Int32</span><span class="sxs-lookup"><span data-stu-id="77f14-116">Int32</span></span>|<span data-ttu-id="77f14-117">Количество устройств с вредоносных программ для версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="77f14-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="77f14-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="77f14-118">lastUpdateDateTime</span></span>|<span data-ttu-id="77f14-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f14-119">DateTimeOffset</span></span>|<span data-ttu-id="77f14-120">Метка времени последнего обновления для счетчик устройства в формате UTC</span><span class="sxs-lookup"><span data-stu-id="77f14-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f14-121">Связи</span><span class="sxs-lookup"><span data-stu-id="77f14-121">Relationships</span></span>
<span data-ttu-id="77f14-122">Нет</span><span class="sxs-lookup"><span data-stu-id="77f14-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="77f14-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77f14-123">JSON Representation</span></span>
<span data-ttu-id="77f14-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77f14-124">Here is a JSON representation of the resource.</span></span>
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





