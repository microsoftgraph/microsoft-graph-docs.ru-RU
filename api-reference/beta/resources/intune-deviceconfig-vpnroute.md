---
title: Тип ресурса Впнрауте
description: Определение маршрута VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54706d47267eef8fff6c465f24e4e9caa183ccc3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154301"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="0ecac-103">Тип ресурса Впнрауте</span><span class="sxs-lookup"><span data-stu-id="0ecac-103">vpnRoute resource type</span></span>

> <span data-ttu-id="0ecac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ecac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ecac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ecac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ecac-106">Определение маршрута VPN.</span><span class="sxs-lookup"><span data-stu-id="0ecac-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0ecac-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ecac-107">Properties</span></span>
|<span data-ttu-id="0ecac-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ecac-108">Property</span></span>|<span data-ttu-id="0ecac-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ecac-109">Type</span></span>|<span data-ttu-id="0ecac-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ecac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ecac-111">Дестинатионпрефикс</span><span class="sxs-lookup"><span data-stu-id="0ecac-111">destinationPrefix</span></span>|<span data-ttu-id="0ecac-112">String</span><span class="sxs-lookup"><span data-stu-id="0ecac-112">String</span></span>|<span data-ttu-id="0ecac-113">Префикс назначения (IPv4/V6-адрес).</span><span class="sxs-lookup"><span data-stu-id="0ecac-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="0ecac-114">Префикссизе</span><span class="sxs-lookup"><span data-stu-id="0ecac-114">prefixSize</span></span>|<span data-ttu-id="0ecac-115">Int32</span><span class="sxs-lookup"><span data-stu-id="0ecac-115">Int32</span></span>|<span data-ttu-id="0ecac-116">Размер префикса.</span><span class="sxs-lookup"><span data-stu-id="0ecac-116">Prefix size.</span></span> <span data-ttu-id="0ecac-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="0ecac-117">(1-32).</span></span> <span data-ttu-id="0ecac-118">Допустимые значения — от 1 до 32</span><span class="sxs-lookup"><span data-stu-id="0ecac-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ecac-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ecac-119">Relationships</span></span>
<span data-ttu-id="0ecac-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0ecac-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ecac-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ecac-121">JSON Representation</span></span>
<span data-ttu-id="0ecac-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ecac-122">Here is a JSON representation of the resource.</span></span>
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




