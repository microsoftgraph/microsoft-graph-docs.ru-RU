---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911842"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="98c93-103">Тип ресурса osVersionCount</span><span class="sxs-lookup"><span data-stu-id="98c93-103">osVersionCount resource type</span></span>

> <span data-ttu-id="98c93-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98c93-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98c93-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98c93-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98c93-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98c93-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98c93-107">Количество устройств с вредоносных программ для каждой версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="98c93-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="98c93-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="98c93-108">Properties</span></span>
|<span data-ttu-id="98c93-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="98c93-109">Property</span></span>|<span data-ttu-id="98c93-110">Тип</span><span class="sxs-lookup"><span data-stu-id="98c93-110">Type</span></span>|<span data-ttu-id="98c93-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98c93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98c93-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="98c93-112">osVersion</span></span>|<span data-ttu-id="98c93-113">String</span><span class="sxs-lookup"><span data-stu-id="98c93-113">String</span></span>|<span data-ttu-id="98c93-114">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="98c93-114">OS version</span></span>|
|<span data-ttu-id="98c93-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="98c93-115">deviceCount</span></span>|<span data-ttu-id="98c93-116">Int32</span><span class="sxs-lookup"><span data-stu-id="98c93-116">Int32</span></span>|<span data-ttu-id="98c93-117">Количество устройств с вредоносных программ для версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="98c93-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="98c93-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="98c93-118">lastUpdateDateTime</span></span>|<span data-ttu-id="98c93-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98c93-119">DateTimeOffset</span></span>|<span data-ttu-id="98c93-120">Метка времени последнего обновления для счетчик устройства в формате UTC</span><span class="sxs-lookup"><span data-stu-id="98c93-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="98c93-121">Связи</span><span class="sxs-lookup"><span data-stu-id="98c93-121">Relationships</span></span>
<span data-ttu-id="98c93-122">Нет</span><span class="sxs-lookup"><span data-stu-id="98c93-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98c93-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98c93-123">JSON Representation</span></span>
<span data-ttu-id="98c93-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98c93-124">Here is a JSON representation of the resource.</span></span>
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





