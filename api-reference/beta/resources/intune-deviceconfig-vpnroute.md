---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00f5d1eb3f05d11833e687d002e1d698a366fd61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367612"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="1021f-103">Тип ресурса Впнрауте</span><span class="sxs-lookup"><span data-stu-id="1021f-103">vpnRoute resource type</span></span>

> <span data-ttu-id="1021f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1021f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1021f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1021f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1021f-106">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="1021f-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1021f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1021f-107">Properties</span></span>
|<span data-ttu-id="1021f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1021f-108">Property</span></span>|<span data-ttu-id="1021f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1021f-109">Type</span></span>|<span data-ttu-id="1021f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1021f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1021f-111">дестинатионпрефикс</span><span class="sxs-lookup"><span data-stu-id="1021f-111">destinationPrefix</span></span>|<span data-ttu-id="1021f-112">String</span><span class="sxs-lookup"><span data-stu-id="1021f-112">String</span></span>|<span data-ttu-id="1021f-113">Префикс назначения (IPv4/V6-адрес).</span><span class="sxs-lookup"><span data-stu-id="1021f-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="1021f-114">префикссизе</span><span class="sxs-lookup"><span data-stu-id="1021f-114">prefixSize</span></span>|<span data-ttu-id="1021f-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1021f-115">Int32</span></span>|<span data-ttu-id="1021f-116">Размер префикса.</span><span class="sxs-lookup"><span data-stu-id="1021f-116">Prefix size.</span></span> <span data-ttu-id="1021f-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="1021f-117">(1-32).</span></span> <span data-ttu-id="1021f-118">Допустимые значения — от 1 до 32</span><span class="sxs-lookup"><span data-stu-id="1021f-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="1021f-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="1021f-119">Relationships</span></span>
<span data-ttu-id="1021f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="1021f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1021f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1021f-121">JSON Representation</span></span>
<span data-ttu-id="1021f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1021f-122">Here is a JSON representation of the resource.</span></span>
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



