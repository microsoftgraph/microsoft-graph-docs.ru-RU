---
title: Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс
description: Тип параметров идентификатора группы
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d54a98bef3b9c0e0517b426332b8d3223e904c8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30177856"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="64735-103">Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс</span><span class="sxs-lookup"><span data-stu-id="64735-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="64735-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64735-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64735-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64735-106">Тип параметров идентификатора группы</span><span class="sxs-lookup"><span data-stu-id="64735-106">Group id options type</span></span>


<span data-ttu-id="64735-107">НаСледуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="64735-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64735-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="64735-108">Properties</span></span>
|<span data-ttu-id="64735-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="64735-109">Property</span></span>|<span data-ttu-id="64735-110">Тип</span><span class="sxs-lookup"><span data-stu-id="64735-110">Type</span></span>|<span data-ttu-id="64735-111">Описание</span><span class="sxs-lookup"><span data-stu-id="64735-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64735-112">Граупидсаурцеоптион</span><span class="sxs-lookup"><span data-stu-id="64735-112">groupIdSourceOption</span></span>|[<span data-ttu-id="64735-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="64735-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="64735-114">Установите эту политику, чтобы ограничить выбор однорангового узла определенным источником.</span><span class="sxs-lookup"><span data-stu-id="64735-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="64735-115">Возможные значения: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="64735-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64735-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="64735-116">Relationships</span></span>
<span data-ttu-id="64735-117">Нет</span><span class="sxs-lookup"><span data-stu-id="64735-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64735-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64735-118">JSON Representation</span></span>
<span data-ttu-id="64735-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64735-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSourceOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdSourceOptions",
  "groupIdSourceOption": "String"
}
```




