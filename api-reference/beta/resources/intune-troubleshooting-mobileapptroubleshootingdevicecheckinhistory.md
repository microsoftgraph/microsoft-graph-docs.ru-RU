---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9fbad683f193ffc6bce00fc29aa694422d2f494
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939814"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="34ffb-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="34ffb-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="34ffb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34ffb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34ffb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34ffb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ffb-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="34ffb-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="34ffb-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="34ffb-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34ffb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="34ffb-108">Properties</span></span>
|<span data-ttu-id="34ffb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="34ffb-109">Property</span></span>|<span data-ttu-id="34ffb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="34ffb-110">Type</span></span>|<span data-ttu-id="34ffb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="34ffb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ffb-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="34ffb-112">occurrenceDateTime</span></span>|<span data-ttu-id="34ffb-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ffb-113">DateTimeOffset</span></span>|<span data-ttu-id="34ffb-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="34ffb-114">Time when the history item occurred.</span></span> <span data-ttu-id="34ffb-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="34ffb-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="34ffb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="34ffb-116">Relationships</span></span>
<span data-ttu-id="34ffb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="34ffb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34ffb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34ffb-118">JSON Representation</span></span>
<span data-ttu-id="34ffb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34ffb-119">Here is a JSON representation of the resource.</span></span>
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




