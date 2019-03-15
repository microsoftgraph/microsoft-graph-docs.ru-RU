---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b54782b1851ea800b548f02b34f60da3a3236a3
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571538"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="b474e-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="b474e-103">iPv6Range resource type</span></span>

> <span data-ttu-id="b474e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b474e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b474e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b474e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b474e-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="b474e-106">IPv6 Range definition.</span></span>


<span data-ttu-id="b474e-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b474e-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b474e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b474e-108">Properties</span></span>
|<span data-ttu-id="b474e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b474e-109">Property</span></span>|<span data-ttu-id="b474e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b474e-110">Type</span></span>|<span data-ttu-id="b474e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b474e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b474e-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="b474e-112">lowerAddress</span></span>|<span data-ttu-id="b474e-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b474e-113">String</span></span>|<span data-ttu-id="b474e-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="b474e-114">Lower address.</span></span>|
|<span data-ttu-id="b474e-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="b474e-115">upperAddress</span></span>|<span data-ttu-id="b474e-116">String</span><span class="sxs-lookup"><span data-stu-id="b474e-116">String</span></span>|<span data-ttu-id="b474e-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="b474e-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b474e-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b474e-118">Relationships</span></span>
<span data-ttu-id="b474e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b474e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b474e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b474e-120">JSON Representation</span></span>
<span data-ttu-id="b474e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b474e-121">Here is a JSON representation of the resource.</span></span>
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




