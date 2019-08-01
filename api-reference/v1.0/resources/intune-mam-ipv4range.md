---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40845b43a50391613e23bf1c4885c382385b4f5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038139"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="c7320-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="c7320-103">iPv4Range resource type</span></span>

> <span data-ttu-id="c7320-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7320-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7320-105">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="c7320-105">IPv4 Range definition.</span></span>


<span data-ttu-id="c7320-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="c7320-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7320-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7320-107">Properties</span></span>
|<span data-ttu-id="c7320-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7320-108">Property</span></span>|<span data-ttu-id="c7320-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c7320-109">Type</span></span>|<span data-ttu-id="c7320-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c7320-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7320-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="c7320-111">lowerAddress</span></span>|<span data-ttu-id="c7320-112">String</span><span class="sxs-lookup"><span data-stu-id="c7320-112">String</span></span>|<span data-ttu-id="c7320-113">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="c7320-113">Lower address.</span></span>|
|<span data-ttu-id="c7320-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="c7320-114">upperAddress</span></span>|<span data-ttu-id="c7320-115">String</span><span class="sxs-lookup"><span data-stu-id="c7320-115">String</span></span>|<span data-ttu-id="c7320-116">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="c7320-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7320-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="c7320-117">Relationships</span></span>
<span data-ttu-id="c7320-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c7320-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7320-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7320-119">JSON Representation</span></span>
<span data-ttu-id="c7320-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7320-120">Here is a JSON representation of the resource.</span></span>
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



