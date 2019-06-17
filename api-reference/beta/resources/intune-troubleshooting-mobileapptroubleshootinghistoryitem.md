---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7158855510df58b56fc63b467ec721250ca502d3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983584"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="e878d-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="e878d-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="e878d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e878d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e878d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e878d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e878d-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e878d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="e878d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e878d-107">Properties</span></span>
|<span data-ttu-id="e878d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e878d-108">Property</span></span>|<span data-ttu-id="e878d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e878d-109">Type</span></span>|<span data-ttu-id="e878d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e878d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e878d-111">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="e878d-111">occurrenceDateTime</span></span>|<span data-ttu-id="e878d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e878d-112">DateTimeOffset</span></span>|<span data-ttu-id="e878d-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="e878d-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e878d-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="e878d-114">Relationships</span></span>
<span data-ttu-id="e878d-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e878d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e878d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e878d-116">JSON Representation</span></span>
<span data-ttu-id="e878d-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e878d-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingHistoryItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingHistoryItem",
  "occurrenceDateTime": "String (timestamp)"
}
```





