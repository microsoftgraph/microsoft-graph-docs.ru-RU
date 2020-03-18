---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf5dff72f8df369fa48c71ff58bf6e4925cc16e8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769166"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="a8820-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="a8820-103">iPv6Range resource type</span></span>

> <span data-ttu-id="a8820-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8820-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8820-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a8820-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8820-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="a8820-106">IPv6 Range definition.</span></span>


<span data-ttu-id="a8820-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a8820-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8820-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8820-108">Properties</span></span>
|<span data-ttu-id="a8820-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8820-109">Property</span></span>|<span data-ttu-id="a8820-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a8820-110">Type</span></span>|<span data-ttu-id="a8820-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8820-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8820-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a8820-112">lowerAddress</span></span>|<span data-ttu-id="a8820-113">String</span><span class="sxs-lookup"><span data-stu-id="a8820-113">String</span></span>|<span data-ttu-id="a8820-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="a8820-114">Lower address.</span></span>|
|<span data-ttu-id="a8820-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a8820-115">upperAddress</span></span>|<span data-ttu-id="a8820-116">String</span><span class="sxs-lookup"><span data-stu-id="a8820-116">String</span></span>|<span data-ttu-id="a8820-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="a8820-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8820-118">Связи</span><span class="sxs-lookup"><span data-stu-id="a8820-118">Relationships</span></span>
<span data-ttu-id="a8820-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a8820-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8820-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8820-120">JSON Representation</span></span>
<span data-ttu-id="a8820-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8820-121">Here is a JSON representation of the resource.</span></span>
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



