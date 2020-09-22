---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a7bdde3831a3634dce25e562ea1d1a332c18fac2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984427"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="d068f-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="d068f-103">iPv6Range resource type</span></span>

<span data-ttu-id="d068f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d068f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d068f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d068f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d068f-106">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="d068f-106">IPv6 Range definition.</span></span>


<span data-ttu-id="d068f-107">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="d068f-107">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d068f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d068f-108">Properties</span></span>
|<span data-ttu-id="d068f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d068f-109">Property</span></span>|<span data-ttu-id="d068f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d068f-110">Type</span></span>|<span data-ttu-id="d068f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d068f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d068f-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="d068f-112">lowerAddress</span></span>|<span data-ttu-id="d068f-113">String</span><span class="sxs-lookup"><span data-stu-id="d068f-113">String</span></span>|<span data-ttu-id="d068f-114">Понижение адреса</span><span class="sxs-lookup"><span data-stu-id="d068f-114">Lower address</span></span>|
|<span data-ttu-id="d068f-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="d068f-115">upperAddress</span></span>|<span data-ttu-id="d068f-116">String</span><span class="sxs-lookup"><span data-stu-id="d068f-116">String</span></span>|<span data-ttu-id="d068f-117">Верхний адрес</span><span class="sxs-lookup"><span data-stu-id="d068f-117">Upper address</span></span>|

## <a name="relationships"></a><span data-ttu-id="d068f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d068f-118">Relationships</span></span>
<span data-ttu-id="d068f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d068f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d068f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d068f-120">JSON Representation</span></span>
<span data-ttu-id="d068f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d068f-121">Here is a JSON representation of the resource.</span></span>
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









