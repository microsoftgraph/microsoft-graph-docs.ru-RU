---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6a0f9e25145040347b8124442fa2639bbbcd0072
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385439"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="90734-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="90734-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

<span data-ttu-id="90734-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90734-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90734-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90734-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90734-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90734-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90734-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="90734-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="90734-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90734-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90734-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="90734-109">Properties</span></span>
|<span data-ttu-id="90734-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="90734-110">Property</span></span>|<span data-ttu-id="90734-111">Тип</span><span class="sxs-lookup"><span data-stu-id="90734-111">Type</span></span>|<span data-ttu-id="90734-112">Описание</span><span class="sxs-lookup"><span data-stu-id="90734-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90734-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="90734-113">occurrenceDateTime</span></span>|<span data-ttu-id="90734-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90734-114">DateTimeOffset</span></span>|<span data-ttu-id="90734-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="90734-115">Time when the history item occurred.</span></span> <span data-ttu-id="90734-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90734-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="90734-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="90734-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="90734-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="90734-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="90734-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="90734-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="90734-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="90734-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="90734-121">рунстате</span><span class="sxs-lookup"><span data-stu-id="90734-121">runState</span></span>|[<span data-ttu-id="90734-122">рунстате</span><span class="sxs-lookup"><span data-stu-id="90734-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="90734-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="90734-123">Status of the item.</span></span> <span data-ttu-id="90734-124">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="90734-124">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="90734-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="90734-125">errorCode</span></span>|<span data-ttu-id="90734-126">String</span><span class="sxs-lookup"><span data-stu-id="90734-126">String</span></span>|<span data-ttu-id="90734-127">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="90734-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90734-128">Связи</span><span class="sxs-lookup"><span data-stu-id="90734-128">Relationships</span></span>
<span data-ttu-id="90734-129">Нет</span><span class="sxs-lookup"><span data-stu-id="90734-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90734-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90734-130">JSON Representation</span></span>
<span data-ttu-id="90734-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90734-131">Here is a JSON representation of the resource.</span></span>
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



