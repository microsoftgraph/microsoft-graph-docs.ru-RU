---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efef2bb43c34c004df48453ca6a2713d445ec970
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737365"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="4cafd-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="4cafd-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="4cafd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4cafd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cafd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4cafd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cafd-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="4cafd-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="4cafd-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cafd-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4cafd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cafd-108">Properties</span></span>
|<span data-ttu-id="4cafd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cafd-109">Property</span></span>|<span data-ttu-id="4cafd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4cafd-110">Type</span></span>|<span data-ttu-id="4cafd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4cafd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cafd-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="4cafd-112">occurrenceDateTime</span></span>|<span data-ttu-id="4cafd-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cafd-113">DateTimeOffset</span></span>|<span data-ttu-id="4cafd-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="4cafd-114">Time when the history item occurred.</span></span> <span data-ttu-id="4cafd-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="4cafd-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="4cafd-116">actionType</span><span class="sxs-lookup"><span data-stu-id="4cafd-116">actionType</span></span>|<span data-ttu-id="4cafd-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="4cafd-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="4cafd-118">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="4cafd-118">Action type for Intune Application.</span></span> <span data-ttu-id="4cafd-119">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="4cafd-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="4cafd-120">Рунстате</span><span class="sxs-lookup"><span data-stu-id="4cafd-120">runState</span></span>|[<span data-ttu-id="4cafd-121">Рунстате</span><span class="sxs-lookup"><span data-stu-id="4cafd-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4cafd-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="4cafd-122">Status of the item.</span></span> <span data-ttu-id="4cafd-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="4cafd-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="4cafd-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="4cafd-124">errorCode</span></span>|<span data-ttu-id="4cafd-125">String</span><span class="sxs-lookup"><span data-stu-id="4cafd-125">String</span></span>|<span data-ttu-id="4cafd-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="4cafd-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cafd-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="4cafd-127">Relationships</span></span>
<span data-ttu-id="4cafd-128">Нет</span><span class="sxs-lookup"><span data-stu-id="4cafd-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cafd-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cafd-129">JSON Representation</span></span>
<span data-ttu-id="4cafd-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cafd-130">Here is a JSON representation of the resource.</span></span>
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





