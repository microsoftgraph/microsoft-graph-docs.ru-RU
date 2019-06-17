---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e86c630e87b3d809087ec0c83a16d97097e34a60
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34981477"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="e5d8e-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="e5d8e-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="e5d8e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5d8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5d8e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e5d8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5d8e-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5d8e-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="e5d8e-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5d8e-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5d8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5d8e-108">Properties</span></span>
|<span data-ttu-id="e5d8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5d8e-109">Property</span></span>|<span data-ttu-id="e5d8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e5d8e-110">Type</span></span>|<span data-ttu-id="e5d8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5d8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5d8e-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="e5d8e-112">occurrenceDateTime</span></span>|<span data-ttu-id="e5d8e-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5d8e-113">DateTimeOffset</span></span>|<span data-ttu-id="e5d8e-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="e5d8e-114">Time when the history item occurred.</span></span> <span data-ttu-id="e5d8e-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5d8e-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5d8e-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="e5d8e-116">Relationships</span></span>
<span data-ttu-id="e5d8e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e5d8e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5d8e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5d8e-118">JSON Representation</span></span>
<span data-ttu-id="e5d8e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5d8e-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)"
}
```





