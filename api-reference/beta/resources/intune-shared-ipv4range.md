---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521c27396c483ba07cc39aec583dd3e610da267d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160517"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="85866-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="85866-103">iPv4Range resource type</span></span>

> <span data-ttu-id="85866-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85866-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85866-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85866-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85866-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="85866-106">IPv4 Range definition.</span></span>


<span data-ttu-id="85866-107">Наследуется от [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="85866-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85866-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="85866-108">Properties</span></span>
|<span data-ttu-id="85866-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="85866-109">Property</span></span>|<span data-ttu-id="85866-110">Тип</span><span class="sxs-lookup"><span data-stu-id="85866-110">Type</span></span>|<span data-ttu-id="85866-111">Описание</span><span class="sxs-lookup"><span data-stu-id="85866-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85866-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="85866-112">lowerAddress</span></span>|<span data-ttu-id="85866-113">String</span><span class="sxs-lookup"><span data-stu-id="85866-113">String</span></span>|<span data-ttu-id="85866-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="85866-114">Lower address.</span></span>|
|<span data-ttu-id="85866-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="85866-115">upperAddress</span></span>|<span data-ttu-id="85866-116">String</span><span class="sxs-lookup"><span data-stu-id="85866-116">String</span></span>|<span data-ttu-id="85866-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="85866-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85866-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="85866-118">Relationships</span></span>
<span data-ttu-id="85866-119">Нет</span><span class="sxs-lookup"><span data-stu-id="85866-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85866-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="85866-120">JSON Representation</span></span>
<span data-ttu-id="85866-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85866-121">Here is a JSON representation of the resource.</span></span>
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




