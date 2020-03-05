---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 546d335fec5945703e790c6cf712f9c37d2394ab
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523312"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="31538-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="31538-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="31538-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31538-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31538-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31538-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31538-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31538-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31538-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="31538-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="31538-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="31538-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31538-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31538-109">Properties</span></span>
|<span data-ttu-id="31538-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31538-110">Property</span></span>|<span data-ttu-id="31538-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31538-111">Type</span></span>|<span data-ttu-id="31538-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31538-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31538-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="31538-113">occurrenceDateTime</span></span>|<span data-ttu-id="31538-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31538-114">DateTimeOffset</span></span>|<span data-ttu-id="31538-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="31538-115">Time when the history item occurred.</span></span> <span data-ttu-id="31538-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="31538-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="31538-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="31538-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="31538-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="31538-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="31538-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="31538-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="31538-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="31538-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="31538-121">actionType</span><span class="sxs-lookup"><span data-stu-id="31538-121">actionType</span></span>|<span data-ttu-id="31538-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="31538-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="31538-123">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="31538-123">Action type for Intune Application.</span></span> <span data-ttu-id="31538-124">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="31538-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="31538-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="31538-125">runState</span></span>|[<span data-ttu-id="31538-126">рунстате</span><span class="sxs-lookup"><span data-stu-id="31538-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="31538-127">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="31538-127">Status of the item.</span></span> <span data-ttu-id="31538-128">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="31538-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="31538-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="31538-129">errorCode</span></span>|<span data-ttu-id="31538-130">String</span><span class="sxs-lookup"><span data-stu-id="31538-130">String</span></span>|<span data-ttu-id="31538-131">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="31538-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31538-132">Связи</span><span class="sxs-lookup"><span data-stu-id="31538-132">Relationships</span></span>
<span data-ttu-id="31538-133">Нет</span><span class="sxs-lookup"><span data-stu-id="31538-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31538-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31538-134">JSON Representation</span></span>
<span data-ttu-id="31538-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31538-135">Here is a JSON representation of the resource.</span></span>
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



