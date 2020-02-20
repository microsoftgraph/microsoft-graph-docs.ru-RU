---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0d83f07cfa71c84cb0db99b7ea6e26822177f8f
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159082"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="560b7-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="560b7-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="560b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="560b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="560b7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="560b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="560b7-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="560b7-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="560b7-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="560b7-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="560b7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="560b7-108">Properties</span></span>
|<span data-ttu-id="560b7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="560b7-109">Property</span></span>|<span data-ttu-id="560b7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="560b7-110">Type</span></span>|<span data-ttu-id="560b7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="560b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="560b7-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="560b7-112">occurrenceDateTime</span></span>|<span data-ttu-id="560b7-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="560b7-113">DateTimeOffset</span></span>|<span data-ttu-id="560b7-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="560b7-114">Time when the history item occurred.</span></span> <span data-ttu-id="560b7-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="560b7-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="560b7-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="560b7-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="560b7-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="560b7-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="560b7-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="560b7-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="560b7-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="560b7-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="560b7-120">рунстате</span><span class="sxs-lookup"><span data-stu-id="560b7-120">runState</span></span>|[<span data-ttu-id="560b7-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="560b7-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="560b7-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="560b7-122">Status of the item.</span></span> <span data-ttu-id="560b7-123">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="560b7-123">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="560b7-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="560b7-124">errorCode</span></span>|<span data-ttu-id="560b7-125">String</span><span class="sxs-lookup"><span data-stu-id="560b7-125">String</span></span>|<span data-ttu-id="560b7-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="560b7-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="560b7-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="560b7-127">Relationships</span></span>
<span data-ttu-id="560b7-128">Нет</span><span class="sxs-lookup"><span data-stu-id="560b7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="560b7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="560b7-129">JSON Representation</span></span>
<span data-ttu-id="560b7-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="560b7-130">Here is a JSON representation of the resource.</span></span>
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



