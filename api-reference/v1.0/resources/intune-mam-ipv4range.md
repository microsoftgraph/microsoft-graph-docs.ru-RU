---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 14cb0d88013b13f57b186f5388d5ac89f60db043
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465526"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="d56a7-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="d56a7-103">iPv4Range resource type</span></span>

> <span data-ttu-id="d56a7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d56a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d56a7-105">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="d56a7-105">IPv4 Range definition.</span></span>


<span data-ttu-id="d56a7-106">Наследуется от ресурса [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="d56a7-106">Inherits from [ipRange](../resources/intune-mam-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d56a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d56a7-107">Properties</span></span>
|<span data-ttu-id="d56a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d56a7-108">Property</span></span>|<span data-ttu-id="d56a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d56a7-109">Type</span></span>|<span data-ttu-id="d56a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d56a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d56a7-111">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="d56a7-111">lowerAddress</span></span>|<span data-ttu-id="d56a7-112">String</span><span class="sxs-lookup"><span data-stu-id="d56a7-112">String</span></span>|<span data-ttu-id="d56a7-113">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="d56a7-113">Lower address.</span></span>|
|<span data-ttu-id="d56a7-114">upperAddress</span><span class="sxs-lookup"><span data-stu-id="d56a7-114">upperAddress</span></span>|<span data-ttu-id="d56a7-115">String</span><span class="sxs-lookup"><span data-stu-id="d56a7-115">String</span></span>|<span data-ttu-id="d56a7-116">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="d56a7-116">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d56a7-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d56a7-117">Relationships</span></span>
<span data-ttu-id="d56a7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d56a7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d56a7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d56a7-119">JSON Representation</span></span>
<span data-ttu-id="d56a7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d56a7-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



