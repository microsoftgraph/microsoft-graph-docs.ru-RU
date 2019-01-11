---
title: Тип ресурса mobileAppTroubleshootingAppTargetHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76595f4fd643e985d28bcb84ad1c4ea6d7be2ad6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810341"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="e5b4f-103">Тип ресурса mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="e5b4f-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="e5b4f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5b4f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5b4f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5b4f-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="e5b4f-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5b4f-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5b4f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5b4f-109">Properties</span></span>
|<span data-ttu-id="e5b4f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5b4f-110">Property</span></span>|<span data-ttu-id="e5b4f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e5b4f-111">Type</span></span>|<span data-ttu-id="e5b4f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e5b4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b4f-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="e5b4f-113">occurrenceDateTime</span></span>|<span data-ttu-id="e5b4f-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5b4f-114">DateTimeOffset</span></span>|<span data-ttu-id="e5b4f-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-115">Time when the history item occurred.</span></span> <span data-ttu-id="e5b4f-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="e5b4f-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="e5b4f-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="e5b4f-117">securityGroupId</span></span>|<span data-ttu-id="e5b4f-118">Строка</span><span class="sxs-lookup"><span data-stu-id="e5b4f-118">String</span></span>|<span data-ttu-id="e5b4f-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="e5b4f-120">runState</span><span class="sxs-lookup"><span data-stu-id="e5b4f-120">runState</span></span>|[<span data-ttu-id="e5b4f-121">runState</span><span class="sxs-lookup"><span data-stu-id="e5b4f-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="e5b4f-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-122">Status of the item.</span></span> <span data-ttu-id="e5b4f-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="e5b4f-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="e5b4f-124">errorCode</span></span>|<span data-ttu-id="e5b4f-125">String</span><span class="sxs-lookup"><span data-stu-id="e5b4f-125">String</span></span>|<span data-ttu-id="e5b4f-126">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5b4f-127">Связи</span><span class="sxs-lookup"><span data-stu-id="e5b4f-127">Relationships</span></span>
<span data-ttu-id="e5b4f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="e5b4f-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e5b4f-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5b4f-129">JSON Representation</span></span>
<span data-ttu-id="e5b4f-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5b4f-130">Here is a JSON representation of the resource.</span></span>
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





