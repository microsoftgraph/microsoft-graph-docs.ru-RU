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
# <a name="ipv6range-resource-type"></a><span data-ttu-id="62a7a-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="62a7a-103">iPv6Range resource type</span></span>

<span data-ttu-id="62a7a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62a7a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="62a7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a7a-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="62a7a-106">IPv6 Range definition.</span></span>


<span data-ttu-id="62a7a-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="62a7a-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62a7a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="62a7a-108">Properties</span></span>
|<span data-ttu-id="62a7a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="62a7a-109">Property</span></span>|<span data-ttu-id="62a7a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="62a7a-110">Type</span></span>|<span data-ttu-id="62a7a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="62a7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a7a-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="62a7a-112">lowerAddress</span></span>|<span data-ttu-id="62a7a-113">String</span><span class="sxs-lookup"><span data-stu-id="62a7a-113">String</span></span>|<span data-ttu-id="62a7a-114">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="62a7a-114">Lower address</span></span>|
|<span data-ttu-id="62a7a-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="62a7a-115">upperAddress</span></span>|<span data-ttu-id="62a7a-116">String</span><span class="sxs-lookup"><span data-stu-id="62a7a-116">String</span></span>|<span data-ttu-id="62a7a-117">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="62a7a-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="62a7a-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="62a7a-118">Relationships</span></span>
<span data-ttu-id="62a7a-119">Нет</span><span class="sxs-lookup"><span data-stu-id="62a7a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62a7a-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62a7a-120">JSON Representation</span></span>
<span data-ttu-id="62a7a-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62a7a-121">Here is a JSON representation of the resource.</span></span>
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







