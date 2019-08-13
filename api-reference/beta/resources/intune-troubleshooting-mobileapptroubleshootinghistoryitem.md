---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b75ba857cce7798ee68fecaefe65b5251a80317
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371945"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="1f551-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="1f551-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="1f551-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f551-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f551-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f551-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f551-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="1f551-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="1f551-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f551-107">Properties</span></span>
|<span data-ttu-id="1f551-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f551-108">Property</span></span>|<span data-ttu-id="1f551-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f551-109">Type</span></span>|<span data-ttu-id="1f551-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f551-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f551-111">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="1f551-111">occurrenceDateTime</span></span>|<span data-ttu-id="1f551-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f551-112">DateTimeOffset</span></span>|<span data-ttu-id="1f551-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="1f551-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f551-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="1f551-114">Relationships</span></span>
<span data-ttu-id="1f551-115">Нет</span><span class="sxs-lookup"><span data-stu-id="1f551-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f551-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f551-116">JSON Representation</span></span>
<span data-ttu-id="1f551-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f551-117">Here is a JSON representation of the resource.</span></span>
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



