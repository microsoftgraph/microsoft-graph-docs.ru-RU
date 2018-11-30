---
title: Тип ресурса mobileAppTroubleshootingAppTargetHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
ms.openlocfilehash: c7397e182c1af4c01753623a655579f5f8c6ee08
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078058"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="62278-103">Тип ресурса mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="62278-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="62278-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62278-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62278-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62278-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62278-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62278-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62278-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="62278-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="62278-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="62278-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62278-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="62278-109">Properties</span></span>
|<span data-ttu-id="62278-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="62278-110">Property</span></span>|<span data-ttu-id="62278-111">Тип</span><span class="sxs-lookup"><span data-stu-id="62278-111">Type</span></span>|<span data-ttu-id="62278-112">Description</span><span class="sxs-lookup"><span data-stu-id="62278-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62278-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="62278-113">occurrenceDateTime</span></span>|<span data-ttu-id="62278-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62278-114">DateTimeOffset</span></span>|<span data-ttu-id="62278-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="62278-115">Time when the history item occurred.</span></span> <span data-ttu-id="62278-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="62278-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="62278-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="62278-117">securityGroupId</span></span>|<span data-ttu-id="62278-118">String</span><span class="sxs-lookup"><span data-stu-id="62278-118">String</span></span>|<span data-ttu-id="62278-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="62278-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="62278-120">runState</span><span class="sxs-lookup"><span data-stu-id="62278-120">runState</span></span>|[<span data-ttu-id="62278-121">runState</span><span class="sxs-lookup"><span data-stu-id="62278-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="62278-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="62278-122">Status of the item.</span></span> <span data-ttu-id="62278-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="62278-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="62278-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="62278-124">errorCode</span></span>|<span data-ttu-id="62278-125">String</span><span class="sxs-lookup"><span data-stu-id="62278-125">String</span></span>|<span data-ttu-id="62278-126">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="62278-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62278-127">Связи</span><span class="sxs-lookup"><span data-stu-id="62278-127">Relationships</span></span>
<span data-ttu-id="62278-128">Нет</span><span class="sxs-lookup"><span data-stu-id="62278-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62278-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62278-129">JSON Representation</span></span>
<span data-ttu-id="62278-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62278-130">Here is a JSON representation of the resource.</span></span>
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





