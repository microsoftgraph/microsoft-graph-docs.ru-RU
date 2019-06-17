---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 24ee76f226e54e2f04da2f3cf4ebf47e6e4fa537
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995982"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="fd7bd-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="fd7bd-103">iPv6Range resource type</span></span>

> <span data-ttu-id="fd7bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fd7bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fd7bd-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-106">IPv6 Range definition.</span></span>


<span data-ttu-id="fd7bd-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fd7bd-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fd7bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd7bd-108">Properties</span></span>
|<span data-ttu-id="fd7bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd7bd-109">Property</span></span>|<span data-ttu-id="fd7bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fd7bd-110">Type</span></span>|<span data-ttu-id="fd7bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fd7bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd7bd-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="fd7bd-112">lowerAddress</span></span>|<span data-ttu-id="fd7bd-113">String</span><span class="sxs-lookup"><span data-stu-id="fd7bd-113">String</span></span>|<span data-ttu-id="fd7bd-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-114">Lower address.</span></span>|
|<span data-ttu-id="fd7bd-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="fd7bd-115">upperAddress</span></span>|<span data-ttu-id="fd7bd-116">String</span><span class="sxs-lookup"><span data-stu-id="fd7bd-116">String</span></span>|<span data-ttu-id="fd7bd-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fd7bd-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="fd7bd-118">Relationships</span></span>
<span data-ttu-id="fd7bd-119">Нет</span><span class="sxs-lookup"><span data-stu-id="fd7bd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd7bd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fd7bd-120">JSON Representation</span></span>
<span data-ttu-id="fd7bd-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd7bd-121">Here is a JSON representation of the resource.</span></span>
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





