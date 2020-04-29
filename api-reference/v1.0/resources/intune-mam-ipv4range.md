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
# <a name="ipv4range-resource-type"></a><span data-ttu-id="01635-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="01635-103">iPv4Range resource type</span></span>

<span data-ttu-id="01635-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01635-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01635-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="01635-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01635-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="01635-106">IPv4 Range definition.</span></span>


<span data-ttu-id="01635-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="01635-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="01635-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="01635-108">Properties</span></span>
|<span data-ttu-id="01635-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="01635-109">Property</span></span>|<span data-ttu-id="01635-110">Тип</span><span class="sxs-lookup"><span data-stu-id="01635-110">Type</span></span>|<span data-ttu-id="01635-111">Описание</span><span class="sxs-lookup"><span data-stu-id="01635-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01635-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="01635-112">lowerAddress</span></span>|<span data-ttu-id="01635-113">String</span><span class="sxs-lookup"><span data-stu-id="01635-113">String</span></span>|<span data-ttu-id="01635-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="01635-114">Lower address.</span></span>|
|<span data-ttu-id="01635-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="01635-115">upperAddress</span></span>|<span data-ttu-id="01635-116">String</span><span class="sxs-lookup"><span data-stu-id="01635-116">String</span></span>|<span data-ttu-id="01635-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="01635-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01635-118">Связи</span><span class="sxs-lookup"><span data-stu-id="01635-118">Relationships</span></span>
<span data-ttu-id="01635-119">Нет</span><span class="sxs-lookup"><span data-stu-id="01635-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01635-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="01635-120">JSON Representation</span></span>
<span data-ttu-id="01635-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="01635-121">Here is a JSON representation of the resource.</span></span>
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







