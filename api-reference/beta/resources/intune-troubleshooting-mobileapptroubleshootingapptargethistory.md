---
title: Тип ресурса mobileAppTroubleshootingAppTargetHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
author: tfitzmac
ms.openlocfilehash: cdb901d4c532b57025837a2fb0cc0975ceba3f8c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312735"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="d5367-103">Тип ресурса mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="d5367-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="d5367-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d5367-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5367-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5367-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5367-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d5367-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5367-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="d5367-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>

<span data-ttu-id="d5367-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5367-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5367-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5367-109">Properties</span></span>
|<span data-ttu-id="d5367-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5367-110">Property</span></span>|<span data-ttu-id="d5367-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d5367-111">Type</span></span>|<span data-ttu-id="d5367-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d5367-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5367-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="d5367-113">occurrenceDateTime</span></span>|<span data-ttu-id="d5367-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5367-114">DateTimeOffset</span></span>|<span data-ttu-id="d5367-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="d5367-115">Time when the history item occurred.</span></span> <span data-ttu-id="d5367-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="d5367-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="d5367-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="d5367-117">securityGroupId</span></span>|<span data-ttu-id="d5367-118">String.</span><span class="sxs-lookup"><span data-stu-id="d5367-118">String</span></span>|<span data-ttu-id="d5367-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="d5367-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="d5367-120">runState</span><span class="sxs-lookup"><span data-stu-id="d5367-120">runState</span></span>|[<span data-ttu-id="d5367-121">runState</span><span class="sxs-lookup"><span data-stu-id="d5367-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="d5367-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="d5367-122">Status of the item.</span></span> <span data-ttu-id="d5367-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="d5367-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="d5367-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="d5367-124">errorCode</span></span>|<span data-ttu-id="d5367-125">String</span><span class="sxs-lookup"><span data-stu-id="d5367-125">String</span></span>|<span data-ttu-id="d5367-126">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="d5367-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5367-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d5367-127">Relationships</span></span>
<span data-ttu-id="d5367-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d5367-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d5367-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5367-129">JSON Representation</span></span>
<span data-ttu-id="d5367-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d5367-130">Here is a JSON representation of the resource.</span></span>
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





