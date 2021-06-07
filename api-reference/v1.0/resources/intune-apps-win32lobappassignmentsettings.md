---
title: тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76e189d684999e3922b625def26d4d0cfcb6a3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752212"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="56990-103">тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="56990-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="56990-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56990-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56990-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56990-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56990-106">Содержит свойства, используемые для назначения мобильного приложения Win32 LOB группе.</span><span class="sxs-lookup"><span data-stu-id="56990-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="56990-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="56990-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56990-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56990-108">Properties</span></span>
|<span data-ttu-id="56990-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56990-109">Property</span></span>|<span data-ttu-id="56990-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56990-110">Type</span></span>|<span data-ttu-id="56990-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56990-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56990-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="56990-112">notifications</span></span>|[<span data-ttu-id="56990-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="56990-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="56990-114">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="56990-114">The notification status for this app assignment.</span></span> <span data-ttu-id="56990-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="56990-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="56990-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="56990-116">restartSettings</span></span>|[<span data-ttu-id="56990-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="56990-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="56990-118">Параметры перезагрузки, которые необходимо применить для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="56990-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="56990-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="56990-119">installTimeSettings</span></span>|[<span data-ttu-id="56990-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="56990-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="56990-121">Параметры времени установки, которые необходимо применить для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="56990-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="56990-122">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="56990-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="56990-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="56990-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="56990-124">Приоритет оптимизации доставки для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="56990-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="56990-125">Этот параметр не поддерживается в национальных облачных средах.</span><span class="sxs-lookup"><span data-stu-id="56990-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="56990-126">Возможные значения: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="56990-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56990-127">Отношения</span><span class="sxs-lookup"><span data-stu-id="56990-127">Relationships</span></span>
<span data-ttu-id="56990-128">Нет</span><span class="sxs-lookup"><span data-stu-id="56990-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56990-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56990-129">JSON Representation</span></span>
<span data-ttu-id="56990-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56990-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```




