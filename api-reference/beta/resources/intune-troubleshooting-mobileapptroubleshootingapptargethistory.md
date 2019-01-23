---
title: Тип ресурса mobileAppTroubleshootingAppTargetHistory
description: Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402967"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a><span data-ttu-id="60996-103">Тип ресурса mobileAppTroubleshootingAppTargetHistory</span><span class="sxs-lookup"><span data-stu-id="60996-103">mobileAppTroubleshootingAppTargetHistory resource type</span></span>

> <span data-ttu-id="60996-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="60996-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60996-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60996-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60996-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60996-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60996-107">Элемент журнала, содержащихся в событии Устранение неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="60996-107">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="60996-108">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="60996-108">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60996-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="60996-109">Properties</span></span>
|<span data-ttu-id="60996-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="60996-110">Property</span></span>|<span data-ttu-id="60996-111">Тип</span><span class="sxs-lookup"><span data-stu-id="60996-111">Type</span></span>|<span data-ttu-id="60996-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60996-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60996-113">occurrenceDateTime</span><span class="sxs-lookup"><span data-stu-id="60996-113">occurrenceDateTime</span></span>|<span data-ttu-id="60996-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60996-114">DateTimeOffset</span></span>|<span data-ttu-id="60996-115">Время возникновения элемент журнала.</span><span class="sxs-lookup"><span data-stu-id="60996-115">Time when the history item occurred.</span></span> <span data-ttu-id="60996-116">Наследуется от [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="60996-116">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="60996-117">securityGroupId</span><span class="sxs-lookup"><span data-stu-id="60996-117">securityGroupId</span></span>|<span data-ttu-id="60996-118">String</span><span class="sxs-lookup"><span data-stu-id="60996-118">String</span></span>|<span data-ttu-id="60996-119">К которому нацелено AAD идентификатор группы безопасности.</span><span class="sxs-lookup"><span data-stu-id="60996-119">AAD security group id to which it was targeted.</span></span>|
|<span data-ttu-id="60996-120">runState</span><span class="sxs-lookup"><span data-stu-id="60996-120">runState</span></span>|[<span data-ttu-id="60996-121">runState</span><span class="sxs-lookup"><span data-stu-id="60996-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="60996-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="60996-122">Status of the item.</span></span> <span data-ttu-id="60996-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="60996-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="60996-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="60996-124">errorCode</span></span>|<span data-ttu-id="60996-125">String</span><span class="sxs-lookup"><span data-stu-id="60996-125">String</span></span>|<span data-ttu-id="60996-126">Код ошибки сбоя, пустой, если нет сбоев.</span><span class="sxs-lookup"><span data-stu-id="60996-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60996-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="60996-127">Relationships</span></span>
<span data-ttu-id="60996-128">Нет</span><span class="sxs-lookup"><span data-stu-id="60996-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60996-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60996-129">JSON Representation</span></span>
<span data-ttu-id="60996-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60996-130">Here is a JSON representation of the resource.</span></span>
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




