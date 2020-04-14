---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77037ad6e8635a9e83da6fb727b30406e77304b4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473584"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="e6549-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="e6549-103">iPv6Range resource type</span></span>

<span data-ttu-id="e6549-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6549-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6549-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6549-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6549-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e6549-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6549-107">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="e6549-107">IPv6 Range definition.</span></span>


<span data-ttu-id="e6549-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="e6549-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6549-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6549-109">Properties</span></span>
|<span data-ttu-id="e6549-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6549-110">Property</span></span>|<span data-ttu-id="e6549-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e6549-111">Type</span></span>|<span data-ttu-id="e6549-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e6549-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6549-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="e6549-113">lowerAddress</span></span>|<span data-ttu-id="e6549-114">String</span><span class="sxs-lookup"><span data-stu-id="e6549-114">String</span></span>|<span data-ttu-id="e6549-115">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="e6549-115">Lower address.</span></span>|
|<span data-ttu-id="e6549-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="e6549-116">upperAddress</span></span>|<span data-ttu-id="e6549-117">String</span><span class="sxs-lookup"><span data-stu-id="e6549-117">String</span></span>|<span data-ttu-id="e6549-118">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="e6549-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6549-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="e6549-119">Relationships</span></span>
<span data-ttu-id="e6549-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e6549-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6549-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6549-121">JSON Representation</span></span>
<span data-ttu-id="e6549-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6549-122">Here is a JSON representation of the resource.</span></span>
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



