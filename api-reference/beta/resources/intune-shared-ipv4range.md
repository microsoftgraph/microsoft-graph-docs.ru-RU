---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8f63731a88c1e18843cd8b2dbfc90740ca0a40fa
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347985"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="09377-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="09377-103">iPv4Range resource type</span></span>

> <span data-ttu-id="09377-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="09377-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09377-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="09377-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09377-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="09377-106">IPv4 Range definition.</span></span>


<span data-ttu-id="09377-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="09377-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09377-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="09377-108">Properties</span></span>
|<span data-ttu-id="09377-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="09377-109">Property</span></span>|<span data-ttu-id="09377-110">Тип</span><span class="sxs-lookup"><span data-stu-id="09377-110">Type</span></span>|<span data-ttu-id="09377-111">Описание</span><span class="sxs-lookup"><span data-stu-id="09377-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09377-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="09377-112">lowerAddress</span></span>|<span data-ttu-id="09377-113">String</span><span class="sxs-lookup"><span data-stu-id="09377-113">String</span></span>|<span data-ttu-id="09377-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="09377-114">Lower address.</span></span>|
|<span data-ttu-id="09377-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="09377-115">upperAddress</span></span>|<span data-ttu-id="09377-116">String</span><span class="sxs-lookup"><span data-stu-id="09377-116">String</span></span>|<span data-ttu-id="09377-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="09377-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09377-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="09377-118">Relationships</span></span>
<span data-ttu-id="09377-119">Нет</span><span class="sxs-lookup"><span data-stu-id="09377-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09377-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09377-120">JSON Representation</span></span>
<span data-ttu-id="09377-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09377-121">Here is a JSON representation of the resource.</span></span>
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



