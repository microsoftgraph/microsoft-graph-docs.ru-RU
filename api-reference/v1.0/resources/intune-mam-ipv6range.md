---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b0e0b733ceea2585198a46e62d0f033b76748035
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439371"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="8459e-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="8459e-103">iPv6Range resource type</span></span>

<span data-ttu-id="8459e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8459e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8459e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8459e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8459e-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="8459e-106">IPv6 Range definition.</span></span>


<span data-ttu-id="8459e-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8459e-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8459e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8459e-108">Properties</span></span>
|<span data-ttu-id="8459e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8459e-109">Property</span></span>|<span data-ttu-id="8459e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8459e-110">Type</span></span>|<span data-ttu-id="8459e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8459e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8459e-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="8459e-112">lowerAddress</span></span>|<span data-ttu-id="8459e-113">String</span><span class="sxs-lookup"><span data-stu-id="8459e-113">String</span></span>|<span data-ttu-id="8459e-114">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="8459e-114">Lower address</span></span>|
|<span data-ttu-id="8459e-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="8459e-115">upperAddress</span></span>|<span data-ttu-id="8459e-116">String</span><span class="sxs-lookup"><span data-stu-id="8459e-116">String</span></span>|<span data-ttu-id="8459e-117">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="8459e-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="8459e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8459e-118">Relationships</span></span>
<span data-ttu-id="8459e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8459e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8459e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8459e-120">JSON Representation</span></span>
<span data-ttu-id="8459e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8459e-121">Here is a JSON representation of the resource.</span></span>
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







