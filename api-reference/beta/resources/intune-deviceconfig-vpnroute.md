---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d978b80c79d0cb9f876410e1d2a86723ec55437
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279488"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="86bb9-103">Тип ресурса Впнрауте</span><span class="sxs-lookup"><span data-stu-id="86bb9-103">vpnRoute resource type</span></span>

<span data-ttu-id="86bb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86bb9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86bb9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86bb9-107">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="86bb9-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="86bb9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="86bb9-108">Properties</span></span>
|<span data-ttu-id="86bb9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="86bb9-109">Property</span></span>|<span data-ttu-id="86bb9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="86bb9-110">Type</span></span>|<span data-ttu-id="86bb9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="86bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86bb9-112">дестинатионпрефикс</span><span class="sxs-lookup"><span data-stu-id="86bb9-112">destinationPrefix</span></span>|<span data-ttu-id="86bb9-113">String</span><span class="sxs-lookup"><span data-stu-id="86bb9-113">String</span></span>|<span data-ttu-id="86bb9-114">Префикс назначения (IPv4/V6-адрес).</span><span class="sxs-lookup"><span data-stu-id="86bb9-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="86bb9-115">префикссизе</span><span class="sxs-lookup"><span data-stu-id="86bb9-115">prefixSize</span></span>|<span data-ttu-id="86bb9-116">Int32</span><span class="sxs-lookup"><span data-stu-id="86bb9-116">Int32</span></span>|<span data-ttu-id="86bb9-117">Размер префикса.</span><span class="sxs-lookup"><span data-stu-id="86bb9-117">Prefix size.</span></span> <span data-ttu-id="86bb9-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="86bb9-118">(1-32).</span></span> <span data-ttu-id="86bb9-119">Допустимые значения — от 1 до 32</span><span class="sxs-lookup"><span data-stu-id="86bb9-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="86bb9-120">Связи</span><span class="sxs-lookup"><span data-stu-id="86bb9-120">Relationships</span></span>
<span data-ttu-id="86bb9-121">Нет</span><span class="sxs-lookup"><span data-stu-id="86bb9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86bb9-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="86bb9-122">JSON Representation</span></span>
<span data-ttu-id="86bb9-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86bb9-123">Here is a JSON representation of the resource.</span></span>
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




