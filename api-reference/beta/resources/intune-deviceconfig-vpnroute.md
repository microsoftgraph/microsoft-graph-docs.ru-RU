---
title: Тип ресурса vpnRoute
description: Определение маршрута VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43924b76a76060ac6576657d172757a503204a82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927592"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="0a89e-103">Тип ресурса vpnRoute</span><span class="sxs-lookup"><span data-stu-id="0a89e-103">vpnRoute resource type</span></span>

> <span data-ttu-id="0a89e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a89e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a89e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a89e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a89e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0a89e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a89e-107">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="0a89e-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="0a89e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a89e-108">Properties</span></span>
|<span data-ttu-id="0a89e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a89e-109">Property</span></span>|<span data-ttu-id="0a89e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a89e-110">Type</span></span>|<span data-ttu-id="0a89e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a89e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a89e-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="0a89e-112">destinationPrefix</span></span>|<span data-ttu-id="0a89e-113">String</span><span class="sxs-lookup"><span data-stu-id="0a89e-113">String</span></span>|<span data-ttu-id="0a89e-114">Префикс назначения (адрес IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="0a89e-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="0a89e-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="0a89e-115">prefixSize</span></span>|<span data-ttu-id="0a89e-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0a89e-116">Int32</span></span>|<span data-ttu-id="0a89e-117">Префикс размера.</span><span class="sxs-lookup"><span data-stu-id="0a89e-117">Prefix size.</span></span> <span data-ttu-id="0a89e-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="0a89e-118">(1-32).</span></span> <span data-ttu-id="0a89e-119">Допустимые значения 1 до 32</span><span class="sxs-lookup"><span data-stu-id="0a89e-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a89e-120">Связи</span><span class="sxs-lookup"><span data-stu-id="0a89e-120">Relationships</span></span>
<span data-ttu-id="0a89e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0a89e-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a89e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a89e-122">JSON Representation</span></span>
<span data-ttu-id="0a89e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a89e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```





