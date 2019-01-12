---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 115c89b6ae90a292e08e7b0374e1c3b529e2df19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926864"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="ea4ec-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="ea4ec-103">iPv6Range resource type</span></span>

> <span data-ttu-id="ea4ec-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea4ec-105">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="ea4ec-105">IP V6 range</span></span>

<span data-ttu-id="ea4ec-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ec-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea4ec-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea4ec-107">Properties</span></span>
|<span data-ttu-id="ea4ec-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea4ec-108">Property</span></span>|<span data-ttu-id="ea4ec-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ea4ec-109">Type</span></span>|<span data-ttu-id="ea4ec-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ea4ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4ec-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="ea4ec-111">lowerAddress</span></span>|<span data-ttu-id="ea4ec-112">Строка</span><span class="sxs-lookup"><span data-stu-id="ea4ec-112">String</span></span>|<span data-ttu-id="ea4ec-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ea4ec-113">Lower IP Address</span></span>|
|<span data-ttu-id="ea4ec-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="ea4ec-114">upperAddress</span></span>|<span data-ttu-id="ea4ec-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ea4ec-115">String</span></span>|<span data-ttu-id="ea4ec-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="ea4ec-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea4ec-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ea4ec-117">Relationships</span></span>
<span data-ttu-id="ea4ec-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ea4ec-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea4ec-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea4ec-119">JSON Representation</span></span>
<span data-ttu-id="ea4ec-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-120">Here is a JSON representation of the resource.</span></span>
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



