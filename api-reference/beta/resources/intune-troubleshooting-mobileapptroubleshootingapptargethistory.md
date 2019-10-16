---
title: Тип ресурса Мобилеапптраублешутингапптаржесистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 489410ec904e012504683e960bc1f4c2b157206f
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37524477"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="0bea3-103">Тип ресурса Мобилеапптраублешутингапптаржесистори</span><span class="sxs-lookup"><span data-stu-id="0bea3-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="0bea3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bea3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bea3-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0bea3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bea3-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0bea3-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="0bea3-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0bea3-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0bea3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0bea3-108">Properties</span></span>
|<span data-ttu-id="0bea3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0bea3-109">Property</span></span>|<span data-ttu-id="0bea3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0bea3-110">Type</span></span>|<span data-ttu-id="0bea3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0bea3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bea3-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="0bea3-112">occurrenceDateTime</span></span>|<span data-ttu-id="0bea3-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bea3-113">DateTimeOffset</span></span>|<span data-ttu-id="0bea3-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="0bea3-114">Time when the history item occurred.</span></span> <span data-ttu-id="0bea3-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0bea3-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="0bea3-116">секуритиграупид</span><span class="sxs-lookup"><span data-stu-id="0bea3-116">securityGroupId</span></span>|<span data-ttu-id="0bea3-117">String</span><span class="sxs-lookup"><span data-stu-id="0bea3-117">String</span></span>|<span data-ttu-id="0bea3-118">Идентификатор группы безопасности AAD, к которой назначена эта группа.</span><span class="sxs-lookup"><span data-stu-id="0bea3-118">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="0bea3-119">рунстате</span><span class="sxs-lookup"><span data-stu-id="0bea3-119">runState</span></span>|[<span data-ttu-id="0bea3-120">рунстате</span><span class="sxs-lookup"><span data-stu-id="0bea3-120">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0bea3-121">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="0bea3-121">Status of the item.</span></span> <span data-ttu-id="0bea3-122">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="0bea3-122">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="0bea3-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="0bea3-123">errorCode</span></span>|<span data-ttu-id="0bea3-124">String</span><span class="sxs-lookup"><span data-stu-id="0bea3-124">String</span></span>|<span data-ttu-id="0bea3-125">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="0bea3-125">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0bea3-126">Связи</span><span class="sxs-lookup"><span data-stu-id="0bea3-126">Relationships</span></span>
<span data-ttu-id="0bea3-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0bea3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0bea3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0bea3-128">JSON Representation</span></span>
<span data-ttu-id="0bea3-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0bea3-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```



