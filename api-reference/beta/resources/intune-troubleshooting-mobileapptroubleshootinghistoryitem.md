---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0136d8e4627875cf3b49e2c1f876bfb7454ea165
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010219"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="fc96e-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="fc96e-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="fc96e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc96e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc96e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc96e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc96e-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="fc96e-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="fc96e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc96e-107">Properties</span></span>
|<span data-ttu-id="fc96e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc96e-108">Property</span></span>|<span data-ttu-id="fc96e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fc96e-109">Type</span></span>|<span data-ttu-id="fc96e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc96e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc96e-111">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="fc96e-111">occurrenceDateTime</span></span>|<span data-ttu-id="fc96e-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc96e-112">DateTimeOffset</span></span>|<span data-ttu-id="fc96e-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="fc96e-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc96e-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="fc96e-114">Relationships</span></span>
<span data-ttu-id="fc96e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="fc96e-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc96e-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc96e-116">JSON Representation</span></span>
<span data-ttu-id="fc96e-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc96e-117">Here is a JSON representation of the resource.</span></span>
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





