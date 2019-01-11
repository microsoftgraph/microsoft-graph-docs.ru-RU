---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 593fc2287e888b38eadd3c588aaeeb51b31ea78f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816263"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f6e1b-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f6e1b-103">iPv4Range resource type</span></span>

> <span data-ttu-id="f6e1b-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f6e1b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6e1b-105">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="f6e1b-105">IP V4 range</span></span>

<span data-ttu-id="f6e1b-106">Наследуется от [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f6e1b-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f6e1b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f6e1b-107">Properties</span></span>
|<span data-ttu-id="f6e1b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f6e1b-108">Property</span></span>|<span data-ttu-id="f6e1b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f6e1b-109">Type</span></span>|<span data-ttu-id="f6e1b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f6e1b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6e1b-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f6e1b-111">lowerAddress</span></span>|<span data-ttu-id="f6e1b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f6e1b-112">String</span></span>|<span data-ttu-id="f6e1b-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f6e1b-113">Lower IP Address</span></span>|
|<span data-ttu-id="f6e1b-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f6e1b-114">upperAddress</span></span>|<span data-ttu-id="f6e1b-115">Строка</span><span class="sxs-lookup"><span data-stu-id="f6e1b-115">String</span></span>|<span data-ttu-id="f6e1b-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f6e1b-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6e1b-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f6e1b-117">Relationships</span></span>
<span data-ttu-id="f6e1b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f6e1b-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f6e1b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f6e1b-119">JSON Representation</span></span>
<span data-ttu-id="f6e1b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f6e1b-120">Here is a JSON representation of the resource.</span></span>
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



