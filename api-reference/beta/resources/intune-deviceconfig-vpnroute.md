---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e0d5b07aa04d7e47459923b1b33d3d32008dcc1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787329"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="9a4c2-103">Тип ресурса Впнрауте</span><span class="sxs-lookup"><span data-stu-id="9a4c2-103">vpnRoute resource type</span></span>

> <span data-ttu-id="9a4c2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a4c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a4c2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a4c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a4c2-106">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="9a4c2-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="9a4c2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a4c2-107">Properties</span></span>
|<span data-ttu-id="9a4c2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a4c2-108">Property</span></span>|<span data-ttu-id="9a4c2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9a4c2-109">Type</span></span>|<span data-ttu-id="9a4c2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9a4c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a4c2-111">дестинатионпрефикс</span><span class="sxs-lookup"><span data-stu-id="9a4c2-111">destinationPrefix</span></span>|<span data-ttu-id="9a4c2-112">String</span><span class="sxs-lookup"><span data-stu-id="9a4c2-112">String</span></span>|<span data-ttu-id="9a4c2-113">Префикс назначения (IPv4/V6-адрес).</span><span class="sxs-lookup"><span data-stu-id="9a4c2-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="9a4c2-114">префикссизе</span><span class="sxs-lookup"><span data-stu-id="9a4c2-114">prefixSize</span></span>|<span data-ttu-id="9a4c2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9a4c2-115">Int32</span></span>|<span data-ttu-id="9a4c2-116">Размер префикса.</span><span class="sxs-lookup"><span data-stu-id="9a4c2-116">Prefix size.</span></span> <span data-ttu-id="9a4c2-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="9a4c2-117">(1-32).</span></span> <span data-ttu-id="9a4c2-118">Допустимые значения — от 1 до 32</span><span class="sxs-lookup"><span data-stu-id="9a4c2-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a4c2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="9a4c2-119">Relationships</span></span>
<span data-ttu-id="9a4c2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="9a4c2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a4c2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9a4c2-121">JSON Representation</span></span>
<span data-ttu-id="9a4c2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a4c2-122">Here is a JSON representation of the resource.</span></span>
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



