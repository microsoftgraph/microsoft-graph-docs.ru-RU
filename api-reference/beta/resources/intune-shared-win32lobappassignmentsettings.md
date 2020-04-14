---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 199a2444a814e989d1567830c400762556f7a6fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436970"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="9c95f-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9c95f-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="9c95f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c95f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c95f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c95f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c95f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9c95f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c95f-107">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="9c95f-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="9c95f-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9c95f-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c95f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c95f-109">Properties</span></span>
|<span data-ttu-id="9c95f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c95f-110">Property</span></span>|<span data-ttu-id="9c95f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9c95f-111">Type</span></span>|<span data-ttu-id="9c95f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9c95f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c95f-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="9c95f-113">notifications</span></span>|[<span data-ttu-id="9c95f-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="9c95f-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="9c95f-115">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="9c95f-115">The notification status for this app assignment.</span></span> <span data-ttu-id="9c95f-116">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="9c95f-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="9c95f-117">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="9c95f-117">restartSettings</span></span>|[<span data-ttu-id="9c95f-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="9c95f-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="9c95f-119">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="9c95f-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="9c95f-120">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="9c95f-120">installTimeSettings</span></span>|[<span data-ttu-id="9c95f-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="9c95f-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="9c95f-122">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="9c95f-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="9c95f-123">деливерйоптимизатионприорити</span><span class="sxs-lookup"><span data-stu-id="9c95f-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="9c95f-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="9c95f-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="9c95f-125">Приоритет оптимизации доставки для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="9c95f-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="9c95f-126">Этот параметр не поддерживается в национальных облачных средах.</span><span class="sxs-lookup"><span data-stu-id="9c95f-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="9c95f-127">Возможные значения: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="9c95f-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c95f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="9c95f-128">Relationships</span></span>
<span data-ttu-id="9c95f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="9c95f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c95f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c95f-130">JSON Representation</span></span>
<span data-ttu-id="9c95f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c95f-131">Here is a JSON representation of the resource.</span></span>
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



