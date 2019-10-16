---
title: Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2993967e1340ebb29e0a794f8204f75c5d431de0
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37525219"
---
# <a name="mobileapptroubleshootingapppolicycreationhistory-resource-type"></a><span data-ttu-id="a24bc-103">Тип ресурса Мобилеапптраублешутингаппполицикреатионхистори</span><span class="sxs-lookup"><span data-stu-id="a24bc-103">mobileAppTroubleshootingAppPolicyCreationHistory resource type</span></span>

> <span data-ttu-id="a24bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a24bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a24bc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a24bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a24bc-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="a24bc-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="a24bc-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a24bc-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a24bc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a24bc-108">Properties</span></span>
|<span data-ttu-id="a24bc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a24bc-109">Property</span></span>|<span data-ttu-id="a24bc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a24bc-110">Type</span></span>|<span data-ttu-id="a24bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a24bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a24bc-112">оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="a24bc-112">occurrenceDateTime</span></span>|<span data-ttu-id="a24bc-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a24bc-113">DateTimeOffset</span></span>|<span data-ttu-id="a24bc-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="a24bc-114">Time when the history item occurred.</span></span> <span data-ttu-id="a24bc-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="a24bc-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="a24bc-116">рунстате</span><span class="sxs-lookup"><span data-stu-id="a24bc-116">runState</span></span>|[<span data-ttu-id="a24bc-117">рунстате</span><span class="sxs-lookup"><span data-stu-id="a24bc-117">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="a24bc-118">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="a24bc-118">Status of the item.</span></span> <span data-ttu-id="a24bc-119">Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="a24bc-119">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="a24bc-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="a24bc-120">errorCode</span></span>|<span data-ttu-id="a24bc-121">String</span><span class="sxs-lookup"><span data-stu-id="a24bc-121">String</span></span>|<span data-ttu-id="a24bc-122">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="a24bc-122">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a24bc-123">Связи</span><span class="sxs-lookup"><span data-stu-id="a24bc-123">Relationships</span></span>
<span data-ttu-id="a24bc-124">Нет</span><span class="sxs-lookup"><span data-stu-id="a24bc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a24bc-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a24bc-125">JSON Representation</span></span>
<span data-ttu-id="a24bc-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a24bc-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppPolicyCreationHistory",
  "occurrenceDateTime": "String (timestamp)",
  "runState": "String",
  "errorCode": "String"
}
```



