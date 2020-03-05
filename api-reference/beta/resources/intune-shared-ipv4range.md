---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a4583b84f3bc2859763c0672f1ea833efeda9378
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523648"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="135de-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="135de-103">iPv4Range resource type</span></span>

<span data-ttu-id="135de-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="135de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="135de-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="135de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="135de-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="135de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="135de-107">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="135de-107">IPv4 Range definition.</span></span>


<span data-ttu-id="135de-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="135de-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="135de-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="135de-109">Properties</span></span>
|<span data-ttu-id="135de-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="135de-110">Property</span></span>|<span data-ttu-id="135de-111">Тип</span><span class="sxs-lookup"><span data-stu-id="135de-111">Type</span></span>|<span data-ttu-id="135de-112">Описание</span><span class="sxs-lookup"><span data-stu-id="135de-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="135de-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="135de-113">lowerAddress</span></span>|<span data-ttu-id="135de-114">String</span><span class="sxs-lookup"><span data-stu-id="135de-114">String</span></span>|<span data-ttu-id="135de-115">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="135de-115">Lower address.</span></span>|
|<span data-ttu-id="135de-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="135de-116">upperAddress</span></span>|<span data-ttu-id="135de-117">String</span><span class="sxs-lookup"><span data-stu-id="135de-117">String</span></span>|<span data-ttu-id="135de-118">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="135de-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="135de-119">Связи</span><span class="sxs-lookup"><span data-stu-id="135de-119">Relationships</span></span>
<span data-ttu-id="135de-120">Нет</span><span class="sxs-lookup"><span data-stu-id="135de-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="135de-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="135de-121">JSON Representation</span></span>
<span data-ttu-id="135de-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="135de-122">Here is a JSON representation of the resource.</span></span>
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



