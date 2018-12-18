---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
author: tfitzmac
ms.openlocfilehash: 3dd5479776cf5f497ab6f26e893a78c73fa6ad86
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316669"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="1aca8-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="1aca8-103">iPv4Range resource type</span></span>

> <span data-ttu-id="1aca8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1aca8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aca8-105">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="1aca8-105">IP V4 range</span></span>

<span data-ttu-id="1aca8-106">Наследуется от [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="1aca8-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1aca8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1aca8-107">Properties</span></span>
|<span data-ttu-id="1aca8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1aca8-108">Property</span></span>|<span data-ttu-id="1aca8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1aca8-109">Type</span></span>|<span data-ttu-id="1aca8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1aca8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aca8-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="1aca8-111">lowerAddress</span></span>|<span data-ttu-id="1aca8-112">Строка</span><span class="sxs-lookup"><span data-stu-id="1aca8-112">String</span></span>|<span data-ttu-id="1aca8-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="1aca8-113">Lower IP Address</span></span>|
|<span data-ttu-id="1aca8-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="1aca8-114">upperAddress</span></span>|<span data-ttu-id="1aca8-115">Строка</span><span class="sxs-lookup"><span data-stu-id="1aca8-115">String</span></span>|<span data-ttu-id="1aca8-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="1aca8-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aca8-117">Связи</span><span class="sxs-lookup"><span data-stu-id="1aca8-117">Relationships</span></span>
<span data-ttu-id="1aca8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1aca8-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1aca8-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1aca8-119">JSON Representation</span></span>
<span data-ttu-id="1aca8-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1aca8-120">Here is a JSON representation of the resource.</span></span>
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



