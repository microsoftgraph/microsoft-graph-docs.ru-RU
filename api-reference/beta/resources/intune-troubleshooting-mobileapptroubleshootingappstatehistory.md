---
title: Тип ресурса mobileAppTroubleshootingAppStateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57e10fcabc0aa3def07872c0e520f09c6ee90fc3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411241"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="5af34-103">Тип ресурса mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="5af34-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="5af34-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5af34-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5af34-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5af34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5af34-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5af34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5af34-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="5af34-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="5af34-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5af34-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5af34-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5af34-109">Properties</span></span>
|<span data-ttu-id="5af34-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5af34-110">Property</span></span>|<span data-ttu-id="5af34-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5af34-111">Type</span></span>|<span data-ttu-id="5af34-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5af34-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5af34-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="5af34-113">occurrenceDateTime</span></span>|<span data-ttu-id="5af34-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5af34-114">DateTimeOffset</span></span>|<span data-ttu-id="5af34-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="5af34-115">Time when the history item occurred.</span></span> <span data-ttu-id="5af34-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="5af34-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="5af34-117">actionType</span><span class="sxs-lookup"><span data-stu-id="5af34-117">actionType</span></span>|<span data-ttu-id="5af34-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="5af34-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="5af34-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="5af34-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="5af34-120">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="5af34-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="5af34-121">runState</span><span class="sxs-lookup"><span data-stu-id="5af34-121">runState</span></span>|[<span data-ttu-id="5af34-122">runState</span><span class="sxs-lookup"><span data-stu-id="5af34-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="5af34-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="5af34-123">Status of the item.</span></span> <span data-ttu-id="5af34-124">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="5af34-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="5af34-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="5af34-125">errorCode</span></span>|<span data-ttu-id="5af34-126">String</span><span class="sxs-lookup"><span data-stu-id="5af34-126">String</span></span>|<span data-ttu-id="5af34-127">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="5af34-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5af34-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="5af34-128">Relationships</span></span>
<span data-ttu-id="5af34-129">Нет</span><span class="sxs-lookup"><span data-stu-id="5af34-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5af34-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5af34-130">JSON Representation</span></span>
<span data-ttu-id="5af34-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5af34-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppStateHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppStateHistory",
  "occurrenceDateTime": "String (timestamp)",
  "actionType": "String",
  "runState": "String",
  "errorCode": "String"
}
```




