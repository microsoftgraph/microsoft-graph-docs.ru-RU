---
title: Тип ресурса mobileAppTroubleshootingAppStateHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: ebe38b852c6c6926b69e75379bc1a029ade0bb98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332160"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="00947-103">Тип ресурса mobileAppTroubleshootingAppStateHistory</span><span class="sxs-lookup"><span data-stu-id="00947-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="00947-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00947-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00947-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00947-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00947-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00947-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00947-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="00947-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="00947-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="00947-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00947-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="00947-109">Properties</span></span>
|<span data-ttu-id="00947-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="00947-110">Property</span></span>|<span data-ttu-id="00947-111">Тип</span><span class="sxs-lookup"><span data-stu-id="00947-111">Type</span></span>|<span data-ttu-id="00947-112">Описание</span><span class="sxs-lookup"><span data-stu-id="00947-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00947-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="00947-113">occurrenceDateTime</span></span>|<span data-ttu-id="00947-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00947-114">DateTimeOffset</span></span>|<span data-ttu-id="00947-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="00947-115">Time when the history item occurred.</span></span> <span data-ttu-id="00947-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="00947-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="00947-117">actionType</span><span class="sxs-lookup"><span data-stu-id="00947-117">actionType</span></span>|<span data-ttu-id="00947-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="00947-118">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="00947-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="00947-119">AAD security group id to which it was targeted.</span></span> <span data-ttu-id="00947-120">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="00947-120">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="00947-121">runState</span><span class="sxs-lookup"><span data-stu-id="00947-121">runState</span></span>|[<span data-ttu-id="00947-122">runState</span><span class="sxs-lookup"><span data-stu-id="00947-122">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="00947-123">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="00947-123">Status of the item.</span></span> <span data-ttu-id="00947-124">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="00947-124">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="00947-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="00947-125">errorCode</span></span>|<span data-ttu-id="00947-126">String</span><span class="sxs-lookup"><span data-stu-id="00947-126">String</span></span>|<span data-ttu-id="00947-127">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="00947-127">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00947-128">Связи</span><span class="sxs-lookup"><span data-stu-id="00947-128">Relationships</span></span>
<span data-ttu-id="00947-129">Нет</span><span class="sxs-lookup"><span data-stu-id="00947-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00947-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00947-130">JSON Representation</span></span>
<span data-ttu-id="00947-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00947-131">Here is a JSON representation of the resource.</span></span>
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





