---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
author: tfitzmac
ms.openlocfilehash: eae240d185a6cf0dc2fc7d0d83194dc9f3f6f00d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314772"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="96ec0-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="96ec0-103">iPv4Range resource type</span></span>

> <span data-ttu-id="96ec0-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="96ec0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96ec0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="96ec0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96ec0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="96ec0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96ec0-107">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="96ec0-107">IP V4 range</span></span>

<span data-ttu-id="96ec0-108">Наследуется от [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="96ec0-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96ec0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="96ec0-109">Properties</span></span>
|<span data-ttu-id="96ec0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="96ec0-110">Property</span></span>|<span data-ttu-id="96ec0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="96ec0-111">Type</span></span>|<span data-ttu-id="96ec0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="96ec0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ec0-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="96ec0-113">lowerAddress</span></span>|<span data-ttu-id="96ec0-114">Строка</span><span class="sxs-lookup"><span data-stu-id="96ec0-114">String</span></span>|<span data-ttu-id="96ec0-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="96ec0-115">Lower IP Address</span></span>|
|<span data-ttu-id="96ec0-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="96ec0-116">upperAddress</span></span>|<span data-ttu-id="96ec0-117">Строка</span><span class="sxs-lookup"><span data-stu-id="96ec0-117">String</span></span>|<span data-ttu-id="96ec0-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="96ec0-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="96ec0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="96ec0-119">Relationships</span></span>
<span data-ttu-id="96ec0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="96ec0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96ec0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="96ec0-121">JSON Representation</span></span>
<span data-ttu-id="96ec0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="96ec0-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



