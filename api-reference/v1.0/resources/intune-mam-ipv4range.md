---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
ms.openlocfilehash: 8b59101e1fcdb5ab88d9c24a0359f8abb1687818
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027238"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="56225-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="56225-103">iPv4Range resource type</span></span>

> <span data-ttu-id="56225-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="56225-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56225-105">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="56225-105">IP V4 range</span></span>

<span data-ttu-id="56225-106">Наследуется от [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="56225-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56225-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="56225-107">Properties</span></span>
|<span data-ttu-id="56225-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="56225-108">Property</span></span>|<span data-ttu-id="56225-109">Тип</span><span class="sxs-lookup"><span data-stu-id="56225-109">Type</span></span>|<span data-ttu-id="56225-110">Описание</span><span class="sxs-lookup"><span data-stu-id="56225-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56225-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="56225-111">lowerAddress</span></span>|<span data-ttu-id="56225-112">String</span><span class="sxs-lookup"><span data-stu-id="56225-112">String</span></span>|<span data-ttu-id="56225-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="56225-113">Lower IP Address</span></span>|
|<span data-ttu-id="56225-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="56225-114">upperAddress</span></span>|<span data-ttu-id="56225-115">String</span><span class="sxs-lookup"><span data-stu-id="56225-115">String</span></span>|<span data-ttu-id="56225-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="56225-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="56225-117">Связи</span><span class="sxs-lookup"><span data-stu-id="56225-117">Relationships</span></span>
<span data-ttu-id="56225-118">Нет</span><span class="sxs-lookup"><span data-stu-id="56225-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56225-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56225-119">JSON Representation</span></span>
<span data-ttu-id="56225-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56225-120">Here is a JSON representation of the resource.</span></span>
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



