---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2c30d85a83bb604a5c0ccb6563d6315a183f6497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971482"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="6fd8e-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="6fd8e-103">iPv6Range resource type</span></span>

> <span data-ttu-id="6fd8e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6fd8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6fd8e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fd8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6fd8e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6fd8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fd8e-107">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="6fd8e-107">IP V6 range</span></span>

<span data-ttu-id="6fd8e-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6fd8e-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6fd8e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fd8e-109">Properties</span></span>
|<span data-ttu-id="6fd8e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fd8e-110">Property</span></span>|<span data-ttu-id="6fd8e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="6fd8e-111">Type</span></span>|<span data-ttu-id="6fd8e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd8e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fd8e-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="6fd8e-113">lowerAddress</span></span>|<span data-ttu-id="6fd8e-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6fd8e-114">String</span></span>|<span data-ttu-id="6fd8e-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="6fd8e-115">Lower IP Address</span></span>|
|<span data-ttu-id="6fd8e-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="6fd8e-116">upperAddress</span></span>|<span data-ttu-id="6fd8e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="6fd8e-117">String</span></span>|<span data-ttu-id="6fd8e-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="6fd8e-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fd8e-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6fd8e-119">Relationships</span></span>
<span data-ttu-id="6fd8e-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6fd8e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6fd8e-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fd8e-121">JSON Representation</span></span>
<span data-ttu-id="6fd8e-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fd8e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



