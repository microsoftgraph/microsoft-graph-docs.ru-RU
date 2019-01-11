---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 759f661464d2dd5cd6c12f6fbfe6b1bfcf549a70
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829661"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="84a57-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="84a57-103">iPv6Range resource type</span></span>

> <span data-ttu-id="84a57-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="84a57-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84a57-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84a57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84a57-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="84a57-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84a57-107">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="84a57-107">IP V6 range</span></span>

<span data-ttu-id="84a57-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="84a57-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84a57-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="84a57-109">Properties</span></span>
|<span data-ttu-id="84a57-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="84a57-110">Property</span></span>|<span data-ttu-id="84a57-111">Тип</span><span class="sxs-lookup"><span data-stu-id="84a57-111">Type</span></span>|<span data-ttu-id="84a57-112">Описание</span><span class="sxs-lookup"><span data-stu-id="84a57-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a57-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="84a57-113">lowerAddress</span></span>|<span data-ttu-id="84a57-114">Строка</span><span class="sxs-lookup"><span data-stu-id="84a57-114">String</span></span>|<span data-ttu-id="84a57-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="84a57-115">Lower IP Address</span></span>|
|<span data-ttu-id="84a57-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="84a57-116">upperAddress</span></span>|<span data-ttu-id="84a57-117">Строка</span><span class="sxs-lookup"><span data-stu-id="84a57-117">String</span></span>|<span data-ttu-id="84a57-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="84a57-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="84a57-119">Связи</span><span class="sxs-lookup"><span data-stu-id="84a57-119">Relationships</span></span>
<span data-ttu-id="84a57-120">Нет</span><span class="sxs-lookup"><span data-stu-id="84a57-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84a57-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84a57-121">JSON Representation</span></span>
<span data-ttu-id="84a57-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84a57-122">Here is a JSON representation of the resource.</span></span>
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



