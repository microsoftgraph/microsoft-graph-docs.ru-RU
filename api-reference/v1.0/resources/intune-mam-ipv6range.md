---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c747f86592394d6e9efc93bba2775872010b254
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356431"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="fbd35-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="fbd35-103">iPv6Range resource type</span></span>

> <span data-ttu-id="fbd35-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fbd35-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbd35-105">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="fbd35-105">IPv6 Range definition.</span></span>


<span data-ttu-id="fbd35-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fbd35-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbd35-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fbd35-107">Properties</span></span>
|<span data-ttu-id="fbd35-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fbd35-108">Property</span></span>|<span data-ttu-id="fbd35-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fbd35-109">Type</span></span>|<span data-ttu-id="fbd35-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fbd35-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbd35-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="fbd35-111">lowerAddress</span></span>|<span data-ttu-id="fbd35-112">String</span><span class="sxs-lookup"><span data-stu-id="fbd35-112">String</span></span>|<span data-ttu-id="fbd35-113">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="fbd35-113">Lower address</span></span>|
|<span data-ttu-id="fbd35-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="fbd35-114">upperAddress</span></span>|<span data-ttu-id="fbd35-115">String</span><span class="sxs-lookup"><span data-stu-id="fbd35-115">String</span></span>|<span data-ttu-id="fbd35-116">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="fbd35-116">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbd35-117">Связи</span><span class="sxs-lookup"><span data-stu-id="fbd35-117">Relationships</span></span>
<span data-ttu-id="fbd35-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fbd35-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbd35-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fbd35-119">JSON Representation</span></span>
<span data-ttu-id="fbd35-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fbd35-120">Here is a JSON representation of the resource.</span></span>
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




