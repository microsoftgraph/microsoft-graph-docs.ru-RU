---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af7daab0b92e1753438cf8b77d129127ee7572ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764441"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="dfb73-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="dfb73-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

> <span data-ttu-id="dfb73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfb73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfb73-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfb73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfb73-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="dfb73-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="dfb73-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfb73-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfb73-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfb73-108">Properties</span></span>
|<span data-ttu-id="dfb73-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfb73-109">Property</span></span>|<span data-ttu-id="dfb73-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dfb73-110">Type</span></span>|<span data-ttu-id="dfb73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dfb73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb73-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="dfb73-112">occurrenceDateTime</span></span>|<span data-ttu-id="dfb73-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfb73-113">DateTimeOffset</span></span>|<span data-ttu-id="dfb73-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="dfb73-114">Time when the history item occurred.</span></span> <span data-ttu-id="dfb73-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfb73-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="dfb73-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="dfb73-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="dfb73-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="dfb73-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="dfb73-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="dfb73-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="dfb73-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="dfb73-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb73-120">Связи</span><span class="sxs-lookup"><span data-stu-id="dfb73-120">Relationships</span></span>
<span data-ttu-id="dfb73-121">Нет</span><span class="sxs-lookup"><span data-stu-id="dfb73-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb73-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfb73-122">JSON Representation</span></span>
<span data-ttu-id="dfb73-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfb73-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingDeviceCheckinHistory",
  "occurrenceDateTime": "String (timestamp)",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  }
}
```



