---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
ms.openlocfilehash: c2f17529b589fc2d7837f6a8f539ff64d5d82dd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028423"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="4b0de-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="4b0de-103">iPv6Range resource type</span></span>

> <span data-ttu-id="4b0de-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4b0de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b0de-105">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="4b0de-105">IP V6 range</span></span>

<span data-ttu-id="4b0de-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="4b0de-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b0de-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b0de-107">Properties</span></span>
|<span data-ttu-id="4b0de-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b0de-108">Property</span></span>|<span data-ttu-id="4b0de-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4b0de-109">Type</span></span>|<span data-ttu-id="4b0de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b0de-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="4b0de-111">lowerAddress</span></span>|<span data-ttu-id="4b0de-112">String</span><span class="sxs-lookup"><span data-stu-id="4b0de-112">String</span></span>|<span data-ttu-id="4b0de-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="4b0de-113">Lower IP Address</span></span>|
|<span data-ttu-id="4b0de-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="4b0de-114">upperAddress</span></span>|<span data-ttu-id="4b0de-115">String</span><span class="sxs-lookup"><span data-stu-id="4b0de-115">String</span></span>|<span data-ttu-id="4b0de-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="4b0de-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b0de-117">Связи</span><span class="sxs-lookup"><span data-stu-id="4b0de-117">Relationships</span></span>
<span data-ttu-id="4b0de-118">Нет</span><span class="sxs-lookup"><span data-stu-id="4b0de-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b0de-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b0de-119">JSON Representation</span></span>
<span data-ttu-id="4b0de-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b0de-120">Here is a JSON representation of the resource.</span></span>
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



