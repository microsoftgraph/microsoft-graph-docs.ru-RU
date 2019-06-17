---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89b07a6f58bcd8ce5159c5bec07d01d2beea9fdd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987539"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="3f2b2-103">Тип ресурса Впнрауте</span><span class="sxs-lookup"><span data-stu-id="3f2b2-103">vpnRoute resource type</span></span>

> <span data-ttu-id="3f2b2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f2b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f2b2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f2b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f2b2-106">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="3f2b2-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3f2b2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f2b2-107">Properties</span></span>
|<span data-ttu-id="3f2b2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f2b2-108">Property</span></span>|<span data-ttu-id="3f2b2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3f2b2-109">Type</span></span>|<span data-ttu-id="3f2b2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f2b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f2b2-111">Дестинатионпрефикс</span><span class="sxs-lookup"><span data-stu-id="3f2b2-111">destinationPrefix</span></span>|<span data-ttu-id="3f2b2-112">String</span><span class="sxs-lookup"><span data-stu-id="3f2b2-112">String</span></span>|<span data-ttu-id="3f2b2-113">Префикс назначения (IPv4/V6-адрес).</span><span class="sxs-lookup"><span data-stu-id="3f2b2-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="3f2b2-114">Префикссизе</span><span class="sxs-lookup"><span data-stu-id="3f2b2-114">prefixSize</span></span>|<span data-ttu-id="3f2b2-115">Int32</span><span class="sxs-lookup"><span data-stu-id="3f2b2-115">Int32</span></span>|<span data-ttu-id="3f2b2-116">Размер префикса.</span><span class="sxs-lookup"><span data-stu-id="3f2b2-116">Prefix size.</span></span> <span data-ttu-id="3f2b2-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="3f2b2-117">(1-32).</span></span> <span data-ttu-id="3f2b2-118">Допустимые значения — от 1 до 32</span><span class="sxs-lookup"><span data-stu-id="3f2b2-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f2b2-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f2b2-119">Relationships</span></span>
<span data-ttu-id="3f2b2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="3f2b2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f2b2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f2b2-121">JSON Representation</span></span>
<span data-ttu-id="3f2b2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f2b2-122">Here is a JSON representation of the resource.</span></span>
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





