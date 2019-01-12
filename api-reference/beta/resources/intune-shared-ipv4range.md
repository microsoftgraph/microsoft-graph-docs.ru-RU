---
title: Тип ресурса iPv4Range
description: Диапазон IPv4-адресов
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 57bcaabfc5155e6b6733de2dc228dd240515281b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980183"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="f8b96-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="f8b96-103">iPv4Range resource type</span></span>

> <span data-ttu-id="f8b96-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8b96-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b96-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8b96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b96-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8b96-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b96-107">Диапазон IPv4-адресов</span><span class="sxs-lookup"><span data-stu-id="f8b96-107">IP V4 range</span></span>

<span data-ttu-id="f8b96-108">Наследуется от [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f8b96-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f8b96-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8b96-109">Properties</span></span>
|<span data-ttu-id="f8b96-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8b96-110">Property</span></span>|<span data-ttu-id="f8b96-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f8b96-111">Type</span></span>|<span data-ttu-id="f8b96-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f8b96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b96-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f8b96-113">lowerAddress</span></span>|<span data-ttu-id="f8b96-114">Строка</span><span class="sxs-lookup"><span data-stu-id="f8b96-114">String</span></span>|<span data-ttu-id="f8b96-115">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f8b96-115">Lower IP Address</span></span>|
|<span data-ttu-id="f8b96-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f8b96-116">upperAddress</span></span>|<span data-ttu-id="f8b96-117">Строка</span><span class="sxs-lookup"><span data-stu-id="f8b96-117">String</span></span>|<span data-ttu-id="f8b96-118">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f8b96-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8b96-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f8b96-119">Relationships</span></span>
<span data-ttu-id="f8b96-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f8b96-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8b96-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8b96-121">JSON Representation</span></span>
<span data-ttu-id="f8b96-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8b96-122">Here is a JSON representation of the resource.</span></span>
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



