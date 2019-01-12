---
title: Тип ресурса mobileAppTroubleshootingAppStateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 03a7cd7a67790dca8824b7e446b5add5304c6f0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917743"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="0ceb9-103">Тип ресурса mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="0ceb9-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="0ceb9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ceb9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ceb9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ceb9-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="0ceb9-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb9-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0ceb9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ceb9-109">Properties</span></span>
|<span data-ttu-id="0ceb9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ceb9-110">Property</span></span>|<span data-ttu-id="0ceb9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="0ceb9-111">Type</span></span>|<span data-ttu-id="0ceb9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="0ceb9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ceb9-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="0ceb9-113">occurrenceDateTime</span></span>|<span data-ttu-id="0ceb9-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ceb9-114">DateTimeOffset</span></span>|<span data-ttu-id="0ceb9-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-115">Time when the history item occurred.</span></span> <span data-ttu-id="0ceb9-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="0ceb9-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="0ceb9-117">actionType</span><span class="sxs-lookup"><span data-stu-id="0ceb9-117">actionType</span></span>|<span data-ttu-id="0ceb9-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="0ceb9-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="0ceb9-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="0ceb9-120">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="0ceb9-121">runState</span><span class="sxs-lookup"><span data-stu-id="0ceb9-121">runState</span></span>|[<span data-ttu-id="0ceb9-122">runState</span><span class="sxs-lookup"><span data-stu-id="0ceb9-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="0ceb9-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-123">Status of the item.</span></span> <span data-ttu-id="0ceb9-124">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="0ceb9-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="0ceb9-125">errorCode</span></span>|<span data-ttu-id="0ceb9-126">String</span><span class="sxs-lookup"><span data-stu-id="0ceb9-126">String</span></span>|<span data-ttu-id="0ceb9-127">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ceb9-128">Связи</span><span class="sxs-lookup"><span data-stu-id="0ceb9-128">Relationships</span></span>
<span data-ttu-id="0ceb9-129">Нет</span><span class="sxs-lookup"><span data-stu-id="0ceb9-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0ceb9-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ceb9-130">JSON Representation</span></span>
<span data-ttu-id="0ceb9-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ceb9-131">Here is a JSON representation of the resource.</span></span>
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





