---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 52fc89c4c3b9b77be30cf3cc8c651bde7e696bf2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003509"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="8895d-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="8895d-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="8895d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8895d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8895d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8895d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8895d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8895d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8895d-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="8895d-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="8895d-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8895d-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8895d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8895d-109">Properties</span></span>
|<span data-ttu-id="8895d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8895d-110">Property</span></span>|<span data-ttu-id="8895d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8895d-111">Type</span></span>|<span data-ttu-id="8895d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8895d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8895d-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="8895d-113">occurrenceDateTime</span></span>|<span data-ttu-id="8895d-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8895d-114">DateTimeOffset</span></span>|<span data-ttu-id="8895d-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="8895d-115">Time when the history item occurred.</span></span> <span data-ttu-id="8895d-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8895d-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8895d-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="8895d-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="8895d-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="8895d-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="8895d-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="8895d-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="8895d-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="8895d-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="8895d-121">секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="8895d-121">securityGroupId</span></span>|<span data-ttu-id="8895d-122">String</span><span class="sxs-lookup"><span data-stu-id="8895d-122">String</span></span>|<span data-ttu-id="8895d-123">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="8895d-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="8895d-124">рунстате</span><span class="sxs-lookup"><span data-stu-id="8895d-124">runState</span></span>|[<span data-ttu-id="8895d-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="8895d-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="8895d-126">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="8895d-126">Status of the item.</span></span> <span data-ttu-id="8895d-127">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="8895d-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="8895d-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="8895d-128">errorCode</span></span>|<span data-ttu-id="8895d-129">String</span><span class="sxs-lookup"><span data-stu-id="8895d-129">String</span></span>|<span data-ttu-id="8895d-130">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="8895d-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8895d-131">Связи</span><span class="sxs-lookup"><span data-stu-id="8895d-131">Relationships</span></span>
<span data-ttu-id="8895d-132">Нет</span><span class="sxs-lookup"><span data-stu-id="8895d-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8895d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8895d-133">JSON Representation</span></span>
<span data-ttu-id="8895d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8895d-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
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
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```






