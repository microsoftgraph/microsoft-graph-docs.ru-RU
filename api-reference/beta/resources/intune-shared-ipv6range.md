---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: rolyon
localization_priority: Normal
doc_type: resourcePageType
ms.prod: Intune
ms.openlocfilehash: 1f2b46cea71d097955ca9e78cc74f6f0cddd1002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967379"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="b763f-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="b763f-103">iPv6Range resource type</span></span>

> <span data-ttu-id="b763f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b763f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b763f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b763f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b763f-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="b763f-106">IPv6 Range definition.</span></span>


<span data-ttu-id="b763f-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b763f-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b763f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b763f-108">Properties</span></span>
|<span data-ttu-id="b763f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b763f-109">Property</span></span>|<span data-ttu-id="b763f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b763f-110">Type</span></span>|<span data-ttu-id="b763f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b763f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b763f-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b763f-112">lowerAddress</span></span>|<span data-ttu-id="b763f-113">String</span><span class="sxs-lookup"><span data-stu-id="b763f-113">String</span></span>|<span data-ttu-id="b763f-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="b763f-114">Lower address.</span></span>|
|<span data-ttu-id="b763f-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b763f-115">upperAddress</span></span>|<span data-ttu-id="b763f-116">String</span><span class="sxs-lookup"><span data-stu-id="b763f-116">String</span></span>|<span data-ttu-id="b763f-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="b763f-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b763f-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b763f-118">Relationships</span></span>
<span data-ttu-id="b763f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b763f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b763f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b763f-120">JSON Representation</span></span>
<span data-ttu-id="b763f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b763f-121">Here is a JSON representation of the resource.</span></span>
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





