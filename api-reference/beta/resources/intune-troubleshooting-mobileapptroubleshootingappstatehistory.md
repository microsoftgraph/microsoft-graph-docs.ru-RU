---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71a5786bb5c2a89d6a4397e999155a31cc0f9369
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42729103"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="6006d-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="6006d-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="6006d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6006d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6006d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6006d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6006d-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="6006d-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="6006d-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6006d-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6006d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6006d-108">Properties</span></span>
|<span data-ttu-id="6006d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6006d-109">Property</span></span>|<span data-ttu-id="6006d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6006d-110">Type</span></span>|<span data-ttu-id="6006d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6006d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6006d-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="6006d-112">occurrenceDateTime</span></span>|<span data-ttu-id="6006d-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6006d-113">DateTimeOffset</span></span>|<span data-ttu-id="6006d-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="6006d-114">Time when the history item occurred.</span></span> <span data-ttu-id="6006d-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6006d-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6006d-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="6006d-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="6006d-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6006d-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="6006d-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="6006d-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="6006d-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="6006d-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="6006d-120">actionType</span><span class="sxs-lookup"><span data-stu-id="6006d-120">actionType</span></span>|<span data-ttu-id="6006d-121">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="6006d-121">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="6006d-122">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="6006d-122">Action type for Intune Application.</span></span> <span data-ttu-id="6006d-123">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="6006d-123">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="6006d-124">рунстате</span><span class="sxs-lookup"><span data-stu-id="6006d-124">runState</span></span>|[<span data-ttu-id="6006d-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="6006d-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="6006d-126">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="6006d-126">Status of the item.</span></span> <span data-ttu-id="6006d-127">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="6006d-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="6006d-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="6006d-128">errorCode</span></span>|<span data-ttu-id="6006d-129">String</span><span class="sxs-lookup"><span data-stu-id="6006d-129">String</span></span>|<span data-ttu-id="6006d-130">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="6006d-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6006d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="6006d-131">Relationships</span></span>
<span data-ttu-id="6006d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="6006d-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6006d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6006d-133">JSON Representation</span></span>
<span data-ttu-id="6006d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6006d-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
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
  },
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```



