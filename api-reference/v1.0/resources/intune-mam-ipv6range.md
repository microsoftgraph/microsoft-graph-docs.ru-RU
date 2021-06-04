---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 965260f0aece2dab826dddd0816877be47de154e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754513"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="a350d-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="a350d-103">iPv6Range resource type</span></span>

<span data-ttu-id="a350d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a350d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a350d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a350d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a350d-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="a350d-106">IPv6 Range definition.</span></span>


<span data-ttu-id="a350d-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a350d-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a350d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a350d-108">Properties</span></span>
|<span data-ttu-id="a350d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a350d-109">Property</span></span>|<span data-ttu-id="a350d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a350d-110">Type</span></span>|<span data-ttu-id="a350d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a350d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a350d-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a350d-112">lowerAddress</span></span>|<span data-ttu-id="a350d-113">String</span><span class="sxs-lookup"><span data-stu-id="a350d-113">String</span></span>|<span data-ttu-id="a350d-114">Нижний адрес.</span><span class="sxs-lookup"><span data-stu-id="a350d-114">Lower address.</span></span>|
|<span data-ttu-id="a350d-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a350d-115">upperAddress</span></span>|<span data-ttu-id="a350d-116">String</span><span class="sxs-lookup"><span data-stu-id="a350d-116">String</span></span>|<span data-ttu-id="a350d-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="a350d-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a350d-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a350d-118">Relationships</span></span>
<span data-ttu-id="a350d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a350d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a350d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a350d-120">JSON Representation</span></span>
<span data-ttu-id="a350d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a350d-121">Here is a JSON representation of the resource.</span></span>
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




