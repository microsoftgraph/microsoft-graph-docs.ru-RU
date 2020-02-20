---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0ba8969dbd74da45f9d5f89fd07524cd1f025a46
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163733"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="da554-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="da554-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

> <span data-ttu-id="da554-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da554-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da554-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="da554-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da554-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="da554-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="da554-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="da554-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da554-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="da554-108">Properties</span></span>
|<span data-ttu-id="da554-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="da554-109">Property</span></span>|<span data-ttu-id="da554-110">Тип</span><span class="sxs-lookup"><span data-stu-id="da554-110">Type</span></span>|<span data-ttu-id="da554-111">Описание</span><span class="sxs-lookup"><span data-stu-id="da554-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da554-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="da554-112">occurrenceDateTime</span></span>|<span data-ttu-id="da554-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da554-113">DateTimeOffset</span></span>|<span data-ttu-id="da554-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="da554-114">Time when the history item occurred.</span></span> <span data-ttu-id="da554-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="da554-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="da554-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="da554-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="da554-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="da554-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="da554-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="da554-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="da554-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="da554-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="da554-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="da554-120">Relationships</span></span>
<span data-ttu-id="da554-121">Нет</span><span class="sxs-lookup"><span data-stu-id="da554-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da554-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da554-122">JSON Representation</span></span>
<span data-ttu-id="da554-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da554-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppUpdateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppUpdateHistory",
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



