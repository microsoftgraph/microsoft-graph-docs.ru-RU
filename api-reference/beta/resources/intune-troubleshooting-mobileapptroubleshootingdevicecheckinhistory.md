---
title: Тип ресурса Мобилеапптраублешутингдевицечеккинхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd1bf9b738fce16b813a03ae56c4a6abbb47cec4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523291"
---
# <a name="mobileapptroubleshootingdevicecheckinhistory-resource-type"></a><span data-ttu-id="c0f78-103">Тип ресурса Мобилеапптраублешутингдевицечеккинхистори</span><span class="sxs-lookup"><span data-stu-id="c0f78-103">mobileAppTroubleshootingDeviceCheckinHistory resource type</span></span>

<span data-ttu-id="c0f78-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c0f78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0f78-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0f78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0f78-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0f78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0f78-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c0f78-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c0f78-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0f78-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0f78-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0f78-109">Properties</span></span>
|<span data-ttu-id="c0f78-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0f78-110">Property</span></span>|<span data-ttu-id="c0f78-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c0f78-111">Type</span></span>|<span data-ttu-id="c0f78-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c0f78-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0f78-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="c0f78-113">occurrenceDateTime</span></span>|<span data-ttu-id="c0f78-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c0f78-114">DateTimeOffset</span></span>|<span data-ttu-id="c0f78-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="c0f78-115">Time when the history item occurred.</span></span> <span data-ttu-id="c0f78-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0f78-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c0f78-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="c0f78-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="c0f78-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="c0f78-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="c0f78-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="c0f78-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="c0f78-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c0f78-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0f78-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c0f78-121">Relationships</span></span>
<span data-ttu-id="c0f78-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c0f78-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0f78-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0f78-123">JSON Representation</span></span>
<span data-ttu-id="c0f78-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0f78-124">Here is a JSON representation of the resource.</span></span>
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



