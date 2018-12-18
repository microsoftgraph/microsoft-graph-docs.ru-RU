---
title: Тип ресурса vpnRoute
description: Определение маршрута VPN.
author: tfitzmac
ms.openlocfilehash: 64d755c4f21b47e928c64348a2f1d6dad1f7206a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322024"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="8e9eb-103">Тип ресурса vpnRoute</span><span class="sxs-lookup"><span data-stu-id="8e9eb-103">vpnRoute resource type</span></span>

> <span data-ttu-id="8e9eb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e9eb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e9eb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e9eb-107">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-107">VPN Route definition.</span></span>
## <a name="properties"></a><span data-ttu-id="8e9eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e9eb-108">Properties</span></span>
|<span data-ttu-id="8e9eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e9eb-109">Property</span></span>|<span data-ttu-id="8e9eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8e9eb-110">Type</span></span>|<span data-ttu-id="8e9eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e9eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9eb-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="8e9eb-112">destinationPrefix</span></span>|<span data-ttu-id="8e9eb-113">String.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-113">String</span></span>|<span data-ttu-id="8e9eb-114">Префикс назначения (адрес IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="8e9eb-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="8e9eb-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="8e9eb-115">prefixSize</span></span>|<span data-ttu-id="8e9eb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9eb-116">Int32</span></span>|<span data-ttu-id="8e9eb-117">Префикс размера.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-117">Prefix size.</span></span> <span data-ttu-id="8e9eb-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="8e9eb-118">(1-32).</span></span> <span data-ttu-id="8e9eb-119">Допустимые значения 1 до 32</span><span class="sxs-lookup"><span data-stu-id="8e9eb-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e9eb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="8e9eb-120">Relationships</span></span>
<span data-ttu-id="8e9eb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="8e9eb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e9eb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e9eb-122">JSON Representation</span></span>
<span data-ttu-id="8e9eb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e9eb-123">Here is a JSON representation of the resource.</span></span>
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





