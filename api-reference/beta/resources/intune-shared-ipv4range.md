---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6a732ad11980b22b08d4684a8706e244e78a08a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938869"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="d75df-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="d75df-103">iPv4Range resource type</span></span>

> <span data-ttu-id="d75df-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d75df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d75df-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d75df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d75df-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="d75df-106">IPv4 Range definition.</span></span>


<span data-ttu-id="d75df-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="d75df-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d75df-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d75df-108">Properties</span></span>
|<span data-ttu-id="d75df-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d75df-109">Property</span></span>|<span data-ttu-id="d75df-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d75df-110">Type</span></span>|<span data-ttu-id="d75df-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d75df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d75df-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="d75df-112">lowerAddress</span></span>|<span data-ttu-id="d75df-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d75df-113">String</span></span>|<span data-ttu-id="d75df-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="d75df-114">Lower address.</span></span>|
|<span data-ttu-id="d75df-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="d75df-115">upperAddress</span></span>|<span data-ttu-id="d75df-116">String</span><span class="sxs-lookup"><span data-stu-id="d75df-116">String</span></span>|<span data-ttu-id="d75df-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="d75df-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d75df-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d75df-118">Relationships</span></span>
<span data-ttu-id="d75df-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d75df-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d75df-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d75df-120">JSON Representation</span></span>
<span data-ttu-id="d75df-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d75df-121">Here is a JSON representation of the resource.</span></span>
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




