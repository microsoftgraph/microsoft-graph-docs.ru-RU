---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a65489c02840960a48bb3795cada7be54abcbcca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010436"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="d9f8b-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="d9f8b-103">iPv4Range resource type</span></span>

> <span data-ttu-id="d9f8b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9f8b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9f8b-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-106">IPv4 Range definition.</span></span>


<span data-ttu-id="d9f8b-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="d9f8b-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d9f8b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d9f8b-108">Properties</span></span>
|<span data-ttu-id="d9f8b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d9f8b-109">Property</span></span>|<span data-ttu-id="d9f8b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d9f8b-110">Type</span></span>|<span data-ttu-id="d9f8b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d9f8b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9f8b-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="d9f8b-112">lowerAddress</span></span>|<span data-ttu-id="d9f8b-113">String</span><span class="sxs-lookup"><span data-stu-id="d9f8b-113">String</span></span>|<span data-ttu-id="d9f8b-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-114">Lower address.</span></span>|
|<span data-ttu-id="d9f8b-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="d9f8b-115">upperAddress</span></span>|<span data-ttu-id="d9f8b-116">String</span><span class="sxs-lookup"><span data-stu-id="d9f8b-116">String</span></span>|<span data-ttu-id="d9f8b-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9f8b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="d9f8b-118">Relationships</span></span>
<span data-ttu-id="d9f8b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d9f8b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9f8b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d9f8b-120">JSON Representation</span></span>
<span data-ttu-id="d9f8b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d9f8b-121">Here is a JSON representation of the resource.</span></span>
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





