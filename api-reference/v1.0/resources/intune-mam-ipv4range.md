---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c260796259ce6084add7eadb48192ea50c209c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931932"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="ff2c9-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="ff2c9-103">iPv4Range resource type</span></span>

> <span data-ttu-id="ff2c9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff2c9-105">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="ff2c9-105">IP V4 range</span></span>

<span data-ttu-id="ff2c9-106">Наследуется от [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ff2c9-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff2c9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff2c9-107">Properties</span></span>
|<span data-ttu-id="ff2c9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff2c9-108">Property</span></span>|<span data-ttu-id="ff2c9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2c9-109">Type</span></span>|<span data-ttu-id="ff2c9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2c9-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ff2c9-111">lowerAddress</span></span>|<span data-ttu-id="ff2c9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ff2c9-112">String</span></span>|<span data-ttu-id="ff2c9-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ff2c9-113">Lower IP Address</span></span>|
|<span data-ttu-id="ff2c9-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ff2c9-114">upperAddress</span></span>|<span data-ttu-id="ff2c9-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ff2c9-115">String</span></span>|<span data-ttu-id="ff2c9-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ff2c9-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2c9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ff2c9-117">Relationships</span></span>
<span data-ttu-id="ff2c9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ff2c9-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ff2c9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff2c9-119">JSON Representation</span></span>
<span data-ttu-id="ff2c9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff2c9-120">Here is a JSON representation of the resource.</span></span>
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



