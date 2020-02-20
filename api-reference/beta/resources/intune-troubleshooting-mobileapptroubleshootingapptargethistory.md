---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d53c03b508dc0298c9ed928acc406cdc63e08781
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159054"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="50ddd-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="50ddd-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="50ddd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50ddd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="50ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ddd-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="50ddd-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="50ddd-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ddd-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="50ddd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="50ddd-108">Properties</span></span>
|<span data-ttu-id="50ddd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="50ddd-109">Property</span></span>|<span data-ttu-id="50ddd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="50ddd-110">Type</span></span>|<span data-ttu-id="50ddd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50ddd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50ddd-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="50ddd-112">occurrenceDateTime</span></span>|<span data-ttu-id="50ddd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50ddd-113">DateTimeOffset</span></span>|<span data-ttu-id="50ddd-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="50ddd-114">Time when the history item occurred.</span></span> <span data-ttu-id="50ddd-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ddd-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="50ddd-116">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="50ddd-116">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="50ddd-117">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="50ddd-117">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="50ddd-118">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="50ddd-118">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="50ddd-119">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="50ddd-119">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="50ddd-120">секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="50ddd-120">securityGroupId</span></span>|<span data-ttu-id="50ddd-121">String</span><span class="sxs-lookup"><span data-stu-id="50ddd-121">String</span></span>|<span data-ttu-id="50ddd-122">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="50ddd-122">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="50ddd-123">рунстате</span><span class="sxs-lookup"><span data-stu-id="50ddd-123">runState</span></span>|[<span data-ttu-id="50ddd-124">рунстате</span><span class="sxs-lookup"><span data-stu-id="50ddd-124">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="50ddd-125">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="50ddd-125">Status of the item.</span></span> <span data-ttu-id="50ddd-126">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="50ddd-126">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="50ddd-127">errorCode</span><span class="sxs-lookup"><span data-stu-id="50ddd-127">errorCode</span></span>|<span data-ttu-id="50ddd-128">String</span><span class="sxs-lookup"><span data-stu-id="50ddd-128">String</span></span>|<span data-ttu-id="50ddd-129">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="50ddd-129">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50ddd-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="50ddd-130">Relationships</span></span>
<span data-ttu-id="50ddd-131">Нет</span><span class="sxs-lookup"><span data-stu-id="50ddd-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50ddd-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50ddd-132">JSON Representation</span></span>
<span data-ttu-id="50ddd-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50ddd-133">Here is a JSON representation of the resource.</span></span>
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



