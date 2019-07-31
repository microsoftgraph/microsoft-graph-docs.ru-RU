---
title: Тип ресурса Мобилеапптраублешутингаппстатехистори
description: Элемент History, содержащийся в событии устранения неполадок мобильного приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d145212645283738d1248bd05c50b1f6658460f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967219"
---
# <a name="mobileapptroubleshootingappstatehistory-resource-type"></a><span data-ttu-id="c914b-103">Тип ресурса Мобилеапптраублешутингаппстатехистори</span><span class="sxs-lookup"><span data-stu-id="c914b-103">mobileAppTroubleshootingAppStateHistory resource type</span></span>

> <span data-ttu-id="c914b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c914b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c914b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c914b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c914b-106">Элемент History, содержащийся в событии устранения неполадок мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c914b-106">History Item contained in the Mobile App Troubleshooting Event.</span></span>


<span data-ttu-id="c914b-107">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c914b-107">Inherits from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c914b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c914b-108">Properties</span></span>
|<span data-ttu-id="c914b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c914b-109">Property</span></span>|<span data-ttu-id="c914b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c914b-110">Type</span></span>|<span data-ttu-id="c914b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c914b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c914b-112">Оккурренцедатетиме</span><span class="sxs-lookup"><span data-stu-id="c914b-112">occurrenceDateTime</span></span>|<span data-ttu-id="c914b-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c914b-113">DateTimeOffset</span></span>|<span data-ttu-id="c914b-114">Время возникновения элемента журнала.</span><span class="sxs-lookup"><span data-stu-id="c914b-114">Time when the history item occurred.</span></span> <span data-ttu-id="c914b-115">Наследуется от [мобилеапптраублешутингхисторитем](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="c914b-115">Inherited from [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)</span></span>|
|<span data-ttu-id="c914b-116">actionType</span><span class="sxs-lookup"><span data-stu-id="c914b-116">actionType</span></span>|<span data-ttu-id="c914b-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md);</span><span class="sxs-lookup"><span data-stu-id="c914b-117">[mobileAppActionType](../resources/intune-troubleshooting-mobileappactiontype.md)</span></span>|<span data-ttu-id="c914b-118">Тип действия для приложения Intune.</span><span class="sxs-lookup"><span data-stu-id="c914b-118">Action type for Intune Application.</span></span> <span data-ttu-id="c914b-119">Возможные значения: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span><span class="sxs-lookup"><span data-stu-id="c914b-119">Possible values are: `unknown`, `installCommandSent`, `installed`, `uninstalled`, `userRequestedInstall`.</span></span>|
|<span data-ttu-id="c914b-120">Рунстате</span><span class="sxs-lookup"><span data-stu-id="c914b-120">runState</span></span>|[<span data-ttu-id="c914b-121">Рунстате</span><span class="sxs-lookup"><span data-stu-id="c914b-121">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="c914b-122">Состояние элемента.</span><span class="sxs-lookup"><span data-stu-id="c914b-122">Status of the item.</span></span> <span data-ttu-id="c914b-123">Возможные значения: `unknown`, `success`, `fail`.</span><span class="sxs-lookup"><span data-stu-id="c914b-123">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="c914b-124">errorCode</span><span class="sxs-lookup"><span data-stu-id="c914b-124">errorCode</span></span>|<span data-ttu-id="c914b-125">String</span><span class="sxs-lookup"><span data-stu-id="c914b-125">String</span></span>|<span data-ttu-id="c914b-126">Код ошибки для сбоя, пустой при отсутствии ошибки.</span><span class="sxs-lookup"><span data-stu-id="c914b-126">Error code for the failure, empty if no failure.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c914b-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="c914b-127">Relationships</span></span>
<span data-ttu-id="c914b-128">Нет</span><span class="sxs-lookup"><span data-stu-id="c914b-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c914b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c914b-129">JSON Representation</span></span>
<span data-ttu-id="c914b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c914b-130">Here is a JSON representation of the resource.</span></span>
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





