---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
ms.openlocfilehash: ac2834ea68e1ce4aa7e28f7b421ff4e3d031f8fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082546"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="45bb2-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="45bb2-103">iPv6Range resource type</span></span>

> <span data-ttu-id="45bb2-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45bb2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45bb2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45bb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45bb2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="45bb2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45bb2-107">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="45bb2-107">IP V6 range</span></span>

<span data-ttu-id="45bb2-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="45bb2-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45bb2-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="45bb2-109">Properties</span></span>
|<span data-ttu-id="45bb2-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="45bb2-110">Property</span></span>|<span data-ttu-id="45bb2-111">Тип</span><span class="sxs-lookup"><span data-stu-id="45bb2-111">Type</span></span>|<span data-ttu-id="45bb2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="45bb2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45bb2-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="45bb2-113">lowerAddress</span></span>|<span data-ttu-id="45bb2-114">String</span><span class="sxs-lookup"><span data-stu-id="45bb2-114">String</span></span>|<span data-ttu-id="45bb2-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="45bb2-115">Lower IP Address</span></span>|
|<span data-ttu-id="45bb2-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="45bb2-116">upperAddress</span></span>|<span data-ttu-id="45bb2-117">String</span><span class="sxs-lookup"><span data-stu-id="45bb2-117">String</span></span>|<span data-ttu-id="45bb2-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="45bb2-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="45bb2-119">Связи</span><span class="sxs-lookup"><span data-stu-id="45bb2-119">Relationships</span></span>
<span data-ttu-id="45bb2-120">Нет</span><span class="sxs-lookup"><span data-stu-id="45bb2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45bb2-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45bb2-121">JSON Representation</span></span>
<span data-ttu-id="45bb2-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45bb2-122">Here is a JSON representation of the resource.</span></span>
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



