---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d8b82955c7c600997468204c46783001bf171038
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468542"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="a207e-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="a207e-103">iPv4Range resource type</span></span>

<span data-ttu-id="a207e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a207e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a207e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a207e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a207e-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="a207e-106">IPv4 Range definition.</span></span>


<span data-ttu-id="a207e-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="a207e-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a207e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a207e-108">Properties</span></span>
|<span data-ttu-id="a207e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a207e-109">Property</span></span>|<span data-ttu-id="a207e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a207e-110">Type</span></span>|<span data-ttu-id="a207e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a207e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a207e-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="a207e-112">lowerAddress</span></span>|<span data-ttu-id="a207e-113">String</span><span class="sxs-lookup"><span data-stu-id="a207e-113">String</span></span>|<span data-ttu-id="a207e-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="a207e-114">Lower address.</span></span>|
|<span data-ttu-id="a207e-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="a207e-115">upperAddress</span></span>|<span data-ttu-id="a207e-116">String</span><span class="sxs-lookup"><span data-stu-id="a207e-116">String</span></span>|<span data-ttu-id="a207e-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="a207e-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a207e-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a207e-118">Relationships</span></span>
<span data-ttu-id="a207e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a207e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a207e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a207e-120">JSON Representation</span></span>
<span data-ttu-id="a207e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a207e-121">Here is a JSON representation of the resource.</span></span>
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







