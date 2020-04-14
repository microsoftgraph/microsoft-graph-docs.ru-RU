---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 198e22884adf355dfaf05a1ab516e2d6d22f0510
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385276"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="2e91a-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="2e91a-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="2e91a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e91a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e91a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e91a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e91a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e91a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e91a-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="2e91a-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="2e91a-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2e91a-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e91a-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e91a-109">Properties</span></span>
|<span data-ttu-id="2e91a-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e91a-110">Property</span></span>|<span data-ttu-id="2e91a-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2e91a-111">Type</span></span>|<span data-ttu-id="2e91a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2e91a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e91a-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="2e91a-113">occurrenceDateTime</span></span>|<span data-ttu-id="2e91a-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e91a-114">DateTimeOffset</span></span>|<span data-ttu-id="2e91a-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="2e91a-115">Time when the history item occurred.</span></span> <span data-ttu-id="2e91a-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2e91a-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="2e91a-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="2e91a-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="2e91a-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="2e91a-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="2e91a-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="2e91a-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="2e91a-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="2e91a-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="2e91a-121">actionType</span><span class="sxs-lookup"><span data-stu-id="2e91a-121">actionType</span></span>|<span data-ttu-id="2e91a-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="2e91a-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="2e91a-123">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="2e91a-123">Action type for Intune Application.</span></span> <span data-ttu-id="2e91a-124">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="2e91a-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="2e91a-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="2e91a-125">runState</span></span>|[<span data-ttu-id="2e91a-126">рунстате</span><span class="sxs-lookup"><span data-stu-id="2e91a-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="2e91a-127">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="2e91a-127">Status of the item.</span></span> <span data-ttu-id="2e91a-128">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="2e91a-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="2e91a-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="2e91a-129">errorCode</span></span>|<span data-ttu-id="2e91a-130">String</span><span class="sxs-lookup"><span data-stu-id="2e91a-130">String</span></span>|<span data-ttu-id="2e91a-131">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="2e91a-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e91a-132">Связи</span><span class="sxs-lookup"><span data-stu-id="2e91a-132">Relationships</span></span>
<span data-ttu-id="2e91a-133">Нет</span><span class="sxs-lookup"><span data-stu-id="2e91a-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e91a-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e91a-134">JSON Representation</span></span>
<span data-ttu-id="2e91a-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e91a-135">Here is a JSON representation of the resource.</span></span>
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



