---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2a61c81bd0d4080cbf8ae706ae100a9fb1332f9a
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159061"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="f5b73-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="f5b73-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="f5b73-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5b73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5b73-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f5b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b73-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f5b73-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="f5b73-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5b73-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5b73-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5b73-108">Properties</span></span>
|<span data-ttu-id="f5b73-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5b73-109">Property</span></span>|<span data-ttu-id="f5b73-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f5b73-110">Type</span></span>|<span data-ttu-id="f5b73-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f5b73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b73-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="f5b73-112">occurrenceDateTime</span></span>|<span data-ttu-id="f5b73-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5b73-113">DateTimeOffset</span></span>|<span data-ttu-id="f5b73-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="f5b73-114">Time when the history item occurred.</span></span> <span data-ttu-id="f5b73-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5b73-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f5b73-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="f5b73-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f5b73-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f5b73-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f5b73-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="f5b73-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="f5b73-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f5b73-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f5b73-120">actionType</span><span class="sxs-lookup"><span data-stu-id="f5b73-120">actionType</span></span>|<span data-ttu-id="f5b73-121">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="f5b73-121">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="f5b73-122">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="f5b73-122">Action type for Intune Application.</span></span> <span data-ttu-id="f5b73-123">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="f5b73-123">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="f5b73-124">рунстате</span><span class="sxs-lookup"><span data-stu-id="f5b73-124">runState</span></span>|[<span data-ttu-id="f5b73-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="f5b73-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f5b73-126">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="f5b73-126">Status of the item.</span></span> <span data-ttu-id="f5b73-127">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f5b73-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="f5b73-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="f5b73-128">errorCode</span></span>|<span data-ttu-id="f5b73-129">String</span><span class="sxs-lookup"><span data-stu-id="f5b73-129">String</span></span>|<span data-ttu-id="f5b73-130">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="f5b73-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5b73-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="f5b73-131">Relationships</span></span>
<span data-ttu-id="f5b73-132">Нет</span><span class="sxs-lookup"><span data-stu-id="f5b73-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5b73-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5b73-133">JSON Representation</span></span>
<span data-ttu-id="f5b73-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5b73-134">Here is a JSON representation of the resource.</span></span>
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



