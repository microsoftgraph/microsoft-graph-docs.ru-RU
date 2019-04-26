---
title: Тип ресурса iPv4Range
description: Определение диапазона IPv4.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c896eb6f9a35992d7370cf29124d8072c171eb30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550597"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="5f2fc-103">Тип ресурса iPv4Range</span><span class="sxs-lookup"><span data-stu-id="5f2fc-103">iPv4Range resource type</span></span>

> <span data-ttu-id="5f2fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f2fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f2fc-106">Определение диапазона IPv4.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-106">IPv4 Range definition.</span></span>


<span data-ttu-id="5f2fc-107">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="5f2fc-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5f2fc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f2fc-108">Properties</span></span>
|<span data-ttu-id="5f2fc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f2fc-109">Property</span></span>|<span data-ttu-id="5f2fc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5f2fc-110">Type</span></span>|<span data-ttu-id="5f2fc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5f2fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f2fc-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="5f2fc-112">lowerAddress</span></span>|<span data-ttu-id="5f2fc-113">String</span><span class="sxs-lookup"><span data-stu-id="5f2fc-113">String</span></span>|<span data-ttu-id="5f2fc-114">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-114">Lower address.</span></span>|
|<span data-ttu-id="5f2fc-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="5f2fc-115">upperAddress</span></span>|<span data-ttu-id="5f2fc-116">String</span><span class="sxs-lookup"><span data-stu-id="5f2fc-116">String</span></span>|<span data-ttu-id="5f2fc-117">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f2fc-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="5f2fc-118">Relationships</span></span>
<span data-ttu-id="5f2fc-119">Нет</span><span class="sxs-lookup"><span data-stu-id="5f2fc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f2fc-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f2fc-120">JSON Representation</span></span>
<span data-ttu-id="5f2fc-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f2fc-121">Here is a JSON representation of the resource.</span></span>
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





