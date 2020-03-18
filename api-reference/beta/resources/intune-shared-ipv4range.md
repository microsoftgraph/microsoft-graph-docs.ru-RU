---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1bed3b43af7203a6c1ee081156708679337e94e0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769285"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f321b-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f321b-103">iPv4Range resource type</span></span>

> <span data-ttu-id="f321b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f321b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f321b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f321b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f321b-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="f321b-106">IPv4 Range definition.</span></span>


<span data-ttu-id="f321b-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f321b-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f321b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f321b-108">Properties</span></span>
|<span data-ttu-id="f321b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f321b-109">Property</span></span>|<span data-ttu-id="f321b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f321b-110">Type</span></span>|<span data-ttu-id="f321b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f321b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f321b-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f321b-112">lowerAddress</span></span>|<span data-ttu-id="f321b-113">String</span><span class="sxs-lookup"><span data-stu-id="f321b-113">String</span></span>|<span data-ttu-id="f321b-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="f321b-114">Lower address.</span></span>|
|<span data-ttu-id="f321b-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f321b-115">upperAddress</span></span>|<span data-ttu-id="f321b-116">String</span><span class="sxs-lookup"><span data-stu-id="f321b-116">String</span></span>|<span data-ttu-id="f321b-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="f321b-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f321b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f321b-118">Relationships</span></span>
<span data-ttu-id="f321b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f321b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f321b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f321b-120">JSON Representation</span></span>
<span data-ttu-id="f321b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f321b-121">Here is a JSON representation of the resource.</span></span>
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



