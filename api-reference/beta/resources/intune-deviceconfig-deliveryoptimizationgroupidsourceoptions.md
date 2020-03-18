---
title: Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс
description: Тип параметров идентификатора группы
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 052b2e658af7e2eaabb1700b64da3687dd9cc91a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793410"
---
# <a name="deliveryoptimizationgroupidsourceoptions-resource-type"></a><span data-ttu-id="59f4c-103">Тип ресурса Деливерйоптимизатионграупидсаурцеоптионс</span><span class="sxs-lookup"><span data-stu-id="59f4c-103">deliveryOptimizationGroupIdSourceOptions resource type</span></span>

> <span data-ttu-id="59f4c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59f4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="59f4c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="59f4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59f4c-106">Тип параметров идентификатора группы</span><span class="sxs-lookup"><span data-stu-id="59f4c-106">Group id options type</span></span>


<span data-ttu-id="59f4c-107">Наследуется от [деливерйоптимизатионграупидсаурце](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="59f4c-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59f4c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="59f4c-108">Properties</span></span>
|<span data-ttu-id="59f4c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="59f4c-109">Property</span></span>|<span data-ttu-id="59f4c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="59f4c-110">Type</span></span>|<span data-ttu-id="59f4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="59f4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59f4c-112">граупидсаурцеоптион</span><span class="sxs-lookup"><span data-stu-id="59f4c-112">groupIdSourceOption</span></span>|[<span data-ttu-id="59f4c-113">deliveryOptimizationGroupIdOptionsType</span><span class="sxs-lookup"><span data-stu-id="59f4c-113">deliveryOptimizationGroupIdOptionsType</span></span>](../resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype.md)|<span data-ttu-id="59f4c-114">Установите эту политику, чтобы ограничить выбор однорангового узла определенным источником.</span><span class="sxs-lookup"><span data-stu-id="59f4c-114">Set this policy to restrict peer selection to a specific source.</span></span> <span data-ttu-id="59f4c-115">Возможные значения: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span><span class="sxs-lookup"><span data-stu-id="59f4c-115">Possible values are: `notConfigured`, `adSite`, `authenticatedDomainSid`, `dhcpUserOption`, `dnsSuffix`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59f4c-116">Связи</span><span class="sxs-lookup"><span data-stu-id="59f4c-116">Relationships</span></span>
<span data-ttu-id="59f4c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="59f4c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="59f4c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59f4c-118">JSON Representation</span></span>
<span data-ttu-id="59f4c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59f4c-119">Here is a JSON representation of the resource.</span></span>
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



