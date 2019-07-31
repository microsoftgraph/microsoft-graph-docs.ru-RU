---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 433b4068606b795cb4bb5ceb7654df3eae068b25
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010226"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="9bc88-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="9bc88-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="9bc88-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9bc88-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9bc88-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9bc88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bc88-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="9bc88-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="9bc88-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9bc88-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9bc88-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9bc88-108">Properties</span></span>
|<span data-ttu-id="9bc88-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9bc88-109">Property</span></span>|<span data-ttu-id="9bc88-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9bc88-110">Type</span></span>|<span data-ttu-id="9bc88-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9bc88-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bc88-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="9bc88-112">occurrenceDateTime</span></span>|<span data-ttu-id="9bc88-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9bc88-113">DateTimeOffset</span></span>|<span data-ttu-id="9bc88-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="9bc88-114">Time when the history item occurred.</span></span> <span data-ttu-id="9bc88-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="9bc88-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bc88-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="9bc88-116">Relationships</span></span>
<span data-ttu-id="9bc88-117">Нет</span><span class="sxs-lookup"><span data-stu-id="9bc88-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bc88-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9bc88-118">JSON Representation</span></span>
<span data-ttu-id="9bc88-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9bc88-119">Here is a JSON representation of the resource.</span></span>
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





