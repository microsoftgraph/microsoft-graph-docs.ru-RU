---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 858beb604d8f677142685f85f41c05ecaa6dc2ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003537"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="f0b80-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="f0b80-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

<span data-ttu-id="f0b80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0b80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0b80-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0b80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0b80-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0b80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0b80-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="f0b80-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="f0b80-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0b80-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0b80-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f0b80-109">Properties</span></span>
|<span data-ttu-id="f0b80-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0b80-110">Property</span></span>|<span data-ttu-id="f0b80-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f0b80-111">Type</span></span>|<span data-ttu-id="f0b80-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f0b80-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0b80-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="f0b80-113">occurrenceDateTime</span></span>|<span data-ttu-id="f0b80-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0b80-114">DateTimeOffset</span></span>|<span data-ttu-id="f0b80-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="f0b80-115">Time when the history item occurred.</span></span> <span data-ttu-id="f0b80-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0b80-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f0b80-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="f0b80-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="f0b80-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f0b80-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="f0b80-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="f0b80-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="f0b80-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="f0b80-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="f0b80-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="f0b80-121">runState</span></span>|[<span data-ttu-id="f0b80-122">рунстате</span><span class="sxs-lookup"><span data-stu-id="f0b80-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f0b80-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="f0b80-123">Status of the item.</span></span> <span data-ttu-id="f0b80-124">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="f0b80-124">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="f0b80-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="f0b80-125">errorCode</span></span>|<span data-ttu-id="f0b80-126">String</span><span class="sxs-lookup"><span data-stu-id="f0b80-126">String</span></span>|<span data-ttu-id="f0b80-127">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="f0b80-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0b80-128">Связи</span><span class="sxs-lookup"><span data-stu-id="f0b80-128">Relationships</span></span>
<span data-ttu-id="f0b80-129">Нет</span><span class="sxs-lookup"><span data-stu-id="f0b80-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0b80-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f0b80-130">JSON Representation</span></span>
<span data-ttu-id="f0b80-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0b80-131">Here is a JSON representation of the resource.</span></span>
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






