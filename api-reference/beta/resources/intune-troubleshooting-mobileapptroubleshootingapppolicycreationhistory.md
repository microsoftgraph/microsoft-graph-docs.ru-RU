---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a322c09c5c9dc4acce593846238e95c49d0fde6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764462"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="88df9-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="88df9-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="88df9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88df9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88df9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="88df9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88df9-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="88df9-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="88df9-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="88df9-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88df9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88df9-108">Properties</span></span>
|<span data-ttu-id="88df9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88df9-109">Property</span></span>|<span data-ttu-id="88df9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88df9-110">Type</span></span>|<span data-ttu-id="88df9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88df9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88df9-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="88df9-112">occurrenceDateTime</span></span>|<span data-ttu-id="88df9-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88df9-113">DateTimeOffset</span></span>|<span data-ttu-id="88df9-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="88df9-114">Time when the history item occurred.</span></span> <span data-ttu-id="88df9-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="88df9-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="88df9-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="88df9-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="88df9-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="88df9-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="88df9-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="88df9-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="88df9-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="88df9-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="88df9-120">рунстате</span><span class="sxs-lookup"><span data-stu-id="88df9-120">runState</span></span>|[<span data-ttu-id="88df9-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="88df9-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="88df9-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="88df9-122">Status of the item.</span></span> <span data-ttu-id="88df9-123">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="88df9-123">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="88df9-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="88df9-124">errorCode</span></span>|<span data-ttu-id="88df9-125">String</span><span class="sxs-lookup"><span data-stu-id="88df9-125">String</span></span>|<span data-ttu-id="88df9-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="88df9-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88df9-127">Связи</span><span class="sxs-lookup"><span data-stu-id="88df9-127">Relationships</span></span>
<span data-ttu-id="88df9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="88df9-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88df9-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88df9-129">JSON Representation</span></span>
<span data-ttu-id="88df9-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88df9-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
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
  "runState": "String",
  "errorCode": "String"
}
```



