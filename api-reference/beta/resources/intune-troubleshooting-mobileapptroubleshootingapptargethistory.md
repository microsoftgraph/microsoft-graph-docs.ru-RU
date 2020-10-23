---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58aba41699737f0ee76fa7f9aded726d981dec9b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732455"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="3f6eb-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="3f6eb-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

<span data-ttu-id="3f6eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f6eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f6eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f6eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f6eb-107">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="3f6eb-108">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f6eb-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f6eb-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f6eb-109">Properties</span></span>
|<span data-ttu-id="3f6eb-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f6eb-110">Property</span></span>|<span data-ttu-id="3f6eb-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3f6eb-111">Type</span></span>|<span data-ttu-id="3f6eb-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3f6eb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f6eb-113">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="3f6eb-113">occurrenceDateTime</span></span>|<span data-ttu-id="3f6eb-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f6eb-114">DateTimeOffset</span></span>|<span data-ttu-id="3f6eb-115">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-115">Time when the history item occurred.</span></span> <span data-ttu-id="3f6eb-116">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f6eb-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3f6eb-117">траублешутинжеррордетаилс</span><span class="sxs-lookup"><span data-stu-id="3f6eb-117">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="3f6eb-118">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="3f6eb-118">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="3f6eb-119">Объект, содержащий подробные сведения об ошибке и ее исправлении.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-119">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="3f6eb-120">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="3f6eb-120">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="3f6eb-121">секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="3f6eb-121">securityGroupId</span></span>|<span data-ttu-id="3f6eb-122">Строка</span><span class="sxs-lookup"><span data-stu-id="3f6eb-122">String</span></span>|<span data-ttu-id="3f6eb-123">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-123">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="3f6eb-124">рунстате</span><span class="sxs-lookup"><span data-stu-id="3f6eb-124">runState</span></span>|[<span data-ttu-id="3f6eb-125">рунстате</span><span class="sxs-lookup"><span data-stu-id="3f6eb-125">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="3f6eb-126">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-126">Status of the item.</span></span> <span data-ttu-id="3f6eb-127">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-127">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="3f6eb-128">errorCode</span><span class="sxs-lookup"><span data-stu-id="3f6eb-128">errorCode</span></span>|<span data-ttu-id="3f6eb-129">String</span><span class="sxs-lookup"><span data-stu-id="3f6eb-129">String</span></span>|<span data-ttu-id="3f6eb-130">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-130">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f6eb-131">Связи</span><span class="sxs-lookup"><span data-stu-id="3f6eb-131">Relationships</span></span>
<span data-ttu-id="3f6eb-132">Нет</span><span class="sxs-lookup"><span data-stu-id="3f6eb-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f6eb-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f6eb-133">JSON Representation</span></span>
<span data-ttu-id="3f6eb-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f6eb-134">Here is a JSON representation of the resource.</span></span>
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





