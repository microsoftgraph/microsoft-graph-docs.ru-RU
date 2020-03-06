---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 545de5eb3a2d2bb53fe40f1c23c03014c2391562
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533198"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f5848-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f5848-103">iPv4Range resource type</span></span>

<span data-ttu-id="f5848-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5848-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5848-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5848-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5848-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="f5848-106">IPv4 Range definition.</span></span>


<span data-ttu-id="f5848-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f5848-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5848-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5848-108">Properties</span></span>
|<span data-ttu-id="f5848-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5848-109">Property</span></span>|<span data-ttu-id="f5848-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5848-110">Type</span></span>|<span data-ttu-id="f5848-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5848-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5848-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f5848-112">lowerAddress</span></span>|<span data-ttu-id="f5848-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f5848-113">String</span></span>|<span data-ttu-id="f5848-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="f5848-114">Lower address.</span></span>|
|<span data-ttu-id="f5848-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f5848-115">upperAddress</span></span>|<span data-ttu-id="f5848-116">String</span><span class="sxs-lookup"><span data-stu-id="f5848-116">String</span></span>|<span data-ttu-id="f5848-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="f5848-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5848-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f5848-118">Relationships</span></span>
<span data-ttu-id="f5848-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f5848-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5848-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5848-120">JSON Representation</span></span>
<span data-ttu-id="f5848-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5848-121">Here is a JSON representation of the resource.</span></span>
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




