---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 072f5eaf856943c78a761644ceea93761e67cc21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003520"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="93770-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="93770-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

<span data-ttu-id="93770-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93770-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93770-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="93770-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93770-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93770-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93770-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="93770-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="93770-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="93770-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="93770-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="93770-109">Properties</span></span>
|<span data-ttu-id="93770-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="93770-110">Property</span></span>|<span data-ttu-id="93770-111">Тип</span><span class="sxs-lookup"><span data-stu-id="93770-111">Type</span></span>|<span data-ttu-id="93770-112">Описание</span><span class="sxs-lookup"><span data-stu-id="93770-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93770-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="93770-113">occurrenceDateTime</span></span>|<span data-ttu-id="93770-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93770-114">DateTimeOffset</span></span>|<span data-ttu-id="93770-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="93770-115">Time when the history item occurred.</span></span> <span data-ttu-id="93770-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="93770-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="93770-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="93770-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="93770-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="93770-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="93770-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="93770-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="93770-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="93770-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="93770-121">actionType</span><span class="sxs-lookup"><span data-stu-id="93770-121">actionType</span></span>|<span data-ttu-id="93770-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="93770-122">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="93770-123">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="93770-123">Action type for Intune Application.</span></span> <span data-ttu-id="93770-124">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="93770-124">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="93770-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="93770-125">runState</span></span>|[<span data-ttu-id="93770-126">рунстате</span><span class="sxs-lookup"><span data-stu-id="93770-126">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="93770-127">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="93770-127">Status of the item.</span></span> <span data-ttu-id="93770-128">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="93770-128">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="93770-129">errorCode</span><span class="sxs-lookup"><span data-stu-id="93770-129">errorCode</span></span>|<span data-ttu-id="93770-130">String</span><span class="sxs-lookup"><span data-stu-id="93770-130">String</span></span>|<span data-ttu-id="93770-131">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="93770-131">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93770-132">Связи</span><span class="sxs-lookup"><span data-stu-id="93770-132">Relationships</span></span>
<span data-ttu-id="93770-133">Нет</span><span class="sxs-lookup"><span data-stu-id="93770-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93770-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93770-134">JSON Representation</span></span>
<span data-ttu-id="93770-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93770-135">Here is a JSON representation of the resource.</span></span>
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






