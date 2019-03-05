---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f171a8ebb28d15e78a30bf542c37a163f0d097f0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258991"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="2027f-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="2027f-103">iPv6Range resource type</span></span>

> <span data-ttu-id="2027f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2027f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2027f-105">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="2027f-105">IPv6 Range definition.</span></span>


<span data-ttu-id="2027f-106">Наследуется от [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="2027f-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2027f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2027f-107">Properties</span></span>
|<span data-ttu-id="2027f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2027f-108">Property</span></span>|<span data-ttu-id="2027f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2027f-109">Type</span></span>|<span data-ttu-id="2027f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2027f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2027f-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="2027f-111">lowerAddress</span></span>|<span data-ttu-id="2027f-112">String</span><span class="sxs-lookup"><span data-stu-id="2027f-112">String</span></span>|<span data-ttu-id="2027f-113">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="2027f-113">Lower address</span></span>|
|<span data-ttu-id="2027f-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="2027f-114">upperAddress</span></span>|<span data-ttu-id="2027f-115">String</span><span class="sxs-lookup"><span data-stu-id="2027f-115">String</span></span>|<span data-ttu-id="2027f-116">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="2027f-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="2027f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="2027f-117">Relationships</span></span>
<span data-ttu-id="2027f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="2027f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2027f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2027f-119">JSON Representation</span></span>
<span data-ttu-id="2027f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2027f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



