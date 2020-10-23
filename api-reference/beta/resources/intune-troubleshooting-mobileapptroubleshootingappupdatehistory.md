---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 46c4c52d0449e599a314b0e562680a6c36c040fc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732448"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="4ef54-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="4ef54-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="4ef54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ef54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ef54-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ef54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef54-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4ef54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef54-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4ef54-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4ef54-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ef54-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ef54-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ef54-109">Properties</span></span>
|<span data-ttu-id="4ef54-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ef54-110">Property</span></span>|<span data-ttu-id="4ef54-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4ef54-111">Type</span></span>|<span data-ttu-id="4ef54-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4ef54-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef54-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="4ef54-113">occurrenceDateTime</span></span>|<span data-ttu-id="4ef54-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ef54-114">DateTimeOffset</span></span>|<span data-ttu-id="4ef54-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="4ef54-115">Time when the history item occurred.</span></span> <span data-ttu-id="4ef54-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ef54-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4ef54-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="4ef54-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="4ef54-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="4ef54-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="4ef54-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="4ef54-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="4ef54-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ef54-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ef54-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4ef54-121">Relationships</span></span>
<span data-ttu-id="4ef54-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4ef54-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ef54-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ef54-123">JSON Representation</span></span>
<span data-ttu-id="4ef54-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ef54-124">Here is a JSON representation of the resource.</span></span>
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





