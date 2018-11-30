---
title: Тип ресурса mobileAppTroubleshootingAppStateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
ms.openlocfilehash: 415d018d3650819bce8defe651af8df77e3c6032
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077180"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="11acf-103">Тип ресурса mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="11acf-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="11acf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="11acf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11acf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11acf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="11acf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="11acf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="11acf-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="11acf-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="11acf-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="11acf-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11acf-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="11acf-109">Properties</span></span>
|<span data-ttu-id="11acf-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="11acf-110">Property</span></span>|<span data-ttu-id="11acf-111">Тип</span><span class="sxs-lookup"><span data-stu-id="11acf-111">Type</span></span>|<span data-ttu-id="11acf-112">Description</span><span class="sxs-lookup"><span data-stu-id="11acf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11acf-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="11acf-113">occurrenceDateTime</span></span>|<span data-ttu-id="11acf-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11acf-114">DateTimeOffset</span></span>|<span data-ttu-id="11acf-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="11acf-115">Time when the history item occurred.</span></span> <span data-ttu-id="11acf-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="11acf-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="11acf-117">actionType</span><span class="sxs-lookup"><span data-stu-id="11acf-117">actionType</span></span>|<span data-ttu-id="11acf-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="11acf-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="11acf-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="11acf-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="11acf-120">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="11acf-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="11acf-121">runState</span><span class="sxs-lookup"><span data-stu-id="11acf-121">runState</span></span>|[<span data-ttu-id="11acf-122">runState</span><span class="sxs-lookup"><span data-stu-id="11acf-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="11acf-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="11acf-123">Status of the item.</span></span> <span data-ttu-id="11acf-124">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="11acf-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="11acf-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="11acf-125">errorCode</span></span>|<span data-ttu-id="11acf-126">String</span><span class="sxs-lookup"><span data-stu-id="11acf-126">String</span></span>|<span data-ttu-id="11acf-127">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="11acf-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11acf-128">Связи</span><span class="sxs-lookup"><span data-stu-id="11acf-128">Relationships</span></span>
<span data-ttu-id="11acf-129">Нет</span><span class="sxs-lookup"><span data-stu-id="11acf-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="11acf-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11acf-130">JSON Representation</span></span>
<span data-ttu-id="11acf-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="11acf-131">Here is a JSON representation of the resource.</span></span>
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





