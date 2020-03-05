---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f8a10002d39f09c801c431332f709c93a2099c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523319"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="8bc92-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="8bc92-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

<span data-ttu-id="8bc92-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8bc92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8bc92-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8bc92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8bc92-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8bc92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bc92-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8bc92-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="8bc92-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bc92-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8bc92-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8bc92-109">Properties</span></span>
|<span data-ttu-id="8bc92-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8bc92-110">Property</span></span>|<span data-ttu-id="8bc92-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8bc92-111">Type</span></span>|<span data-ttu-id="8bc92-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8bc92-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bc92-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="8bc92-113">occurrenceDateTime</span></span>|<span data-ttu-id="8bc92-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bc92-114">DateTimeOffset</span></span>|<span data-ttu-id="8bc92-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="8bc92-115">Time when the history item occurred.</span></span> <span data-ttu-id="8bc92-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bc92-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8bc92-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="8bc92-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="8bc92-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8bc92-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="8bc92-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="8bc92-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="8bc92-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8bc92-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8bc92-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="8bc92-121">runState</span></span>|[<span data-ttu-id="8bc92-122">рунстате</span><span class="sxs-lookup"><span data-stu-id="8bc92-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8bc92-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="8bc92-123">Status of the item.</span></span> <span data-ttu-id="8bc92-124">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="8bc92-124">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="8bc92-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="8bc92-125">errorCode</span></span>|<span data-ttu-id="8bc92-126">String</span><span class="sxs-lookup"><span data-stu-id="8bc92-126">String</span></span>|<span data-ttu-id="8bc92-127">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="8bc92-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8bc92-128">Связи</span><span class="sxs-lookup"><span data-stu-id="8bc92-128">Relationships</span></span>
<span data-ttu-id="8bc92-129">Нет</span><span class="sxs-lookup"><span data-stu-id="8bc92-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bc92-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8bc92-130">JSON Representation</span></span>
<span data-ttu-id="8bc92-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8bc92-131">Here is a JSON representation of the resource.</span></span>
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



