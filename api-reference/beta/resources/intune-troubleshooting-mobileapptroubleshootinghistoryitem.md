---
title: Тип ресурса Мобилеапптраублешутингхисторитем
description: Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbc37488f478c47b0b097c4fd8a54b09273bc5c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160860"
---
# <a name="mobileapptroubleshootinghistoryitem-resource-type"></a><span data-ttu-id="ab937-103">Тип ресурса Мобилеапптраублешутингхисторитем</span><span class="sxs-lookup"><span data-stu-id="ab937-103">mobileAppTroubleshootingHistoryItem resource type</span></span>

> <span data-ttu-id="ab937-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab937-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab937-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ab937-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab937-106">Элемент History, содержащийся в соБытии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="ab937-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>

## <a name="properties"></a><span data-ttu-id="ab937-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab937-107">Properties</span></span>
|<span data-ttu-id="ab937-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab937-108">Property</span></span>|<span data-ttu-id="ab937-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ab937-109">Type</span></span>|<span data-ttu-id="ab937-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ab937-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab937-111">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="ab937-111">occurrenceDateTime</span></span>|<span data-ttu-id="ab937-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab937-112">DateTimeOffset</span></span>|<span data-ttu-id="ab937-113">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="ab937-113">Time when the history item occurred.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab937-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="ab937-114">Relationships</span></span>
<span data-ttu-id="ab937-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ab937-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab937-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab937-116">JSON Representation</span></span>
<span data-ttu-id="ab937-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ab937-117">Here is a JSON representation of the resource.</span></span>
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




