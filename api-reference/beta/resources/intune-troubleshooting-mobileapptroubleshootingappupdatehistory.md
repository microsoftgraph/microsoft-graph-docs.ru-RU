---
title: Тип ресурса Мобилеапптраублешутингаппупдатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 72eedcfc1c3031a8c571d4f490a74def6a0fd9de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388239"
---
# <a name="mobileapptroubleshootingappupdatehistory-resource-type"></a><span data-ttu-id="3700a-103">Тип ресурса Мобилеапптраублешутингаппупдатехистори</span><span class="sxs-lookup"><span data-stu-id="3700a-103">mobileAppTroubleshootingAppUpdateHistory resource type</span></span>

<span data-ttu-id="3700a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3700a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3700a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3700a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3700a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3700a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3700a-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3700a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3700a-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3700a-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3700a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3700a-109">Properties</span></span>
|<span data-ttu-id="3700a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3700a-110">Property</span></span>|<span data-ttu-id="3700a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3700a-111">Type</span></span>|<span data-ttu-id="3700a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3700a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3700a-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="3700a-113">occurrenceDateTime</span></span>|<span data-ttu-id="3700a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3700a-114">DateTimeOffset</span></span>|<span data-ttu-id="3700a-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="3700a-115">Time when the history item occurred.</span></span> <span data-ttu-id="3700a-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3700a-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3700a-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="3700a-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3700a-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3700a-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3700a-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="3700a-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3700a-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3700a-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3700a-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3700a-121">Relationships</span></span>
<span data-ttu-id="3700a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3700a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3700a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3700a-123">JSON Representation</span></span>
<span data-ttu-id="3700a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3700a-124">Here is a JSON representation of the resource.</span></span>
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



