---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e3ad2761050ec3bf0a26a2da5e7faf83a8e5523
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752786"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="6d78b-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="6d78b-103">iPv4Range resource type</span></span>

<span data-ttu-id="6d78b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d78b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d78b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d78b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d78b-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="6d78b-106">IPv4 Range definition.</span></span>


<span data-ttu-id="6d78b-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6d78b-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6d78b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d78b-108">Properties</span></span>
|<span data-ttu-id="6d78b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d78b-109">Property</span></span>|<span data-ttu-id="6d78b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6d78b-110">Type</span></span>|<span data-ttu-id="6d78b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d78b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d78b-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="6d78b-112">lowerAddress</span></span>|<span data-ttu-id="6d78b-113">String</span><span class="sxs-lookup"><span data-stu-id="6d78b-113">String</span></span>|<span data-ttu-id="6d78b-114">Нижний адрес.</span><span class="sxs-lookup"><span data-stu-id="6d78b-114">Lower address.</span></span>|
|<span data-ttu-id="6d78b-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="6d78b-115">upperAddress</span></span>|<span data-ttu-id="6d78b-116">String</span><span class="sxs-lookup"><span data-stu-id="6d78b-116">String</span></span>|<span data-ttu-id="6d78b-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="6d78b-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d78b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d78b-118">Relationships</span></span>
<span data-ttu-id="6d78b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6d78b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d78b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d78b-120">JSON Representation</span></span>
<span data-ttu-id="6d78b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d78b-121">Here is a JSON representation of the resource.</span></span>
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




