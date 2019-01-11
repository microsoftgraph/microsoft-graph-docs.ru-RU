---
title: Тип ресурса iPv6Range
description: Диапазон IPv6-адресов
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 84d925cc7885dab4b3e87dbd62060894e741f52c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845748"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="f272e-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="f272e-103">iPv6Range resource type</span></span>

> <span data-ttu-id="f272e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f272e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f272e-105">Диапазон IPv6-адресов</span><span class="sxs-lookup"><span data-stu-id="f272e-105">IP V6 range</span></span>

<span data-ttu-id="f272e-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="f272e-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f272e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f272e-107">Properties</span></span>
|<span data-ttu-id="f272e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f272e-108">Property</span></span>|<span data-ttu-id="f272e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f272e-109">Type</span></span>|<span data-ttu-id="f272e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f272e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f272e-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="f272e-111">lowerAddress</span></span>|<span data-ttu-id="f272e-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f272e-112">String</span></span>|<span data-ttu-id="f272e-113">Нижний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f272e-113">Lower IP Address</span></span>|
|<span data-ttu-id="f272e-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="f272e-114">upperAddress</span></span>|<span data-ttu-id="f272e-115">Строка</span><span class="sxs-lookup"><span data-stu-id="f272e-115">String</span></span>|<span data-ttu-id="f272e-116">Верхний IP-адрес</span><span class="sxs-lookup"><span data-stu-id="f272e-116">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="f272e-117">Связи</span><span class="sxs-lookup"><span data-stu-id="f272e-117">Relationships</span></span>
<span data-ttu-id="f272e-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f272e-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f272e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f272e-119">JSON Representation</span></span>
<span data-ttu-id="f272e-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f272e-120">Here is a JSON representation of the resource.</span></span>
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



