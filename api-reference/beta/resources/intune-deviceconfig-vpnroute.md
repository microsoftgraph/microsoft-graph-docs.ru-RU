---
title: Тип ресурса vpnRoute
description: Определение маршрута VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 628e2f384b06dece13da1595a4111a2d1022a673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423022"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="0b965-103">Тип ресурса vpnRoute</span><span class="sxs-lookup"><span data-stu-id="0b965-103">vpnRoute resource type</span></span>

> <span data-ttu-id="0b965-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0b965-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b965-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b965-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b965-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b965-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b965-107">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="0b965-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0b965-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b965-108">Properties</span></span>
|<span data-ttu-id="0b965-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b965-109">Property</span></span>|<span data-ttu-id="0b965-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0b965-110">Type</span></span>|<span data-ttu-id="0b965-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0b965-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b965-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="0b965-112">destinationPrefix</span></span>|<span data-ttu-id="0b965-113">String</span><span class="sxs-lookup"><span data-stu-id="0b965-113">String</span></span>|<span data-ttu-id="0b965-114">Префикс назначения (адрес IPv4/v6).</span><span class="sxs-lookup"><span data-stu-id="0b965-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="0b965-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="0b965-115">prefixSize</span></span>|<span data-ttu-id="0b965-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0b965-116">Int32</span></span>|<span data-ttu-id="0b965-117">Префикс размера.</span><span class="sxs-lookup"><span data-stu-id="0b965-117">Prefix size.</span></span> <span data-ttu-id="0b965-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="0b965-118">(1-32).</span></span> <span data-ttu-id="0b965-119">Допустимые значения 1 до 32</span><span class="sxs-lookup"><span data-stu-id="0b965-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b965-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="0b965-120">Relationships</span></span>
<span data-ttu-id="0b965-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0b965-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b965-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0b965-122">JSON Representation</span></span>
<span data-ttu-id="0b965-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b965-123">Here is a JSON representation of the resource.</span></span>
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




