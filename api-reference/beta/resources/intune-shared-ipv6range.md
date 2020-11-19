---
title: Тип ресурса iPv6Range
description: Определение диапазона IPv6.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 383d75ceafd1946d317cc3ee146f39a0433accd0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255835"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="8e8c6-103">Тип ресурса iPv6Range</span><span class="sxs-lookup"><span data-stu-id="8e8c6-103">iPv6Range resource type</span></span>

<span data-ttu-id="8e8c6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e8c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e8c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e8c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e8c6-107">Определение диапазона IPv6.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-107">IPv6 Range definition.</span></span>


<span data-ttu-id="8e8c6-108">Наследуется от ресурса [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="8e8c6-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e8c6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8e8c6-109">Properties</span></span>
|<span data-ttu-id="8e8c6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e8c6-110">Property</span></span>|<span data-ttu-id="8e8c6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8e8c6-111">Type</span></span>|<span data-ttu-id="8e8c6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8e8c6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e8c6-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="8e8c6-113">lowerAddress</span></span>|<span data-ttu-id="8e8c6-114">String</span><span class="sxs-lookup"><span data-stu-id="8e8c6-114">String</span></span>|<span data-ttu-id="8e8c6-115">Адрес нижнего уровня.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-115">Lower address.</span></span>|
|<span data-ttu-id="8e8c6-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="8e8c6-116">upperAddress</span></span>|<span data-ttu-id="8e8c6-117">String</span><span class="sxs-lookup"><span data-stu-id="8e8c6-117">String</span></span>|<span data-ttu-id="8e8c6-118">Верхний адрес.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-118">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e8c6-119">Связи</span><span class="sxs-lookup"><span data-stu-id="8e8c6-119">Relationships</span></span>
<span data-ttu-id="8e8c6-120">Нет</span><span class="sxs-lookup"><span data-stu-id="8e8c6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e8c6-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8e8c6-121">JSON Representation</span></span>
<span data-ttu-id="8e8c6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e8c6-122">Here is a JSON representation of the resource.</span></span>
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




