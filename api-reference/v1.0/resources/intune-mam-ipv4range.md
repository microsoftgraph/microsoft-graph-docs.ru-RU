---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7fc8ef3ecc436580c14150df472971144b5197d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356452"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="dab9f-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="dab9f-103">iPv4Range resource type</span></span>

> <span data-ttu-id="dab9f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dab9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dab9f-105">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="dab9f-105">IPv4 Range definition.</span></span>


<span data-ttu-id="dab9f-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="dab9f-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dab9f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dab9f-107">Properties</span></span>
|<span data-ttu-id="dab9f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dab9f-108">Property</span></span>|<span data-ttu-id="dab9f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dab9f-109">Type</span></span>|<span data-ttu-id="dab9f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dab9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dab9f-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="dab9f-111">lowerAddress</span></span>|<span data-ttu-id="dab9f-112">String</span><span class="sxs-lookup"><span data-stu-id="dab9f-112">String</span></span>|<span data-ttu-id="dab9f-113">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="dab9f-113">Lower address.</span></span>|
|<span data-ttu-id="dab9f-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="dab9f-114">upperAddress</span></span>|<span data-ttu-id="dab9f-115">String</span><span class="sxs-lookup"><span data-stu-id="dab9f-115">String</span></span>|<span data-ttu-id="dab9f-116">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="dab9f-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dab9f-117">Связи</span><span class="sxs-lookup"><span data-stu-id="dab9f-117">Relationships</span></span>
<span data-ttu-id="dab9f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="dab9f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dab9f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dab9f-119">JSON Representation</span></span>
<span data-ttu-id="dab9f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dab9f-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```




