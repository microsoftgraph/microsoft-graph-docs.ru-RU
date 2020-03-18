---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 340dc21cce7b52ebc55c13488f7340c7b66f9e26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767045"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="d82f7-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d82f7-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d82f7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d82f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d82f7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d82f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d82f7-106">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="d82f7-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="d82f7-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d82f7-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d82f7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d82f7-108">Properties</span></span>
|<span data-ttu-id="d82f7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d82f7-109">Property</span></span>|<span data-ttu-id="d82f7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d82f7-110">Type</span></span>|<span data-ttu-id="d82f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d82f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82f7-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="d82f7-112">notifications</span></span>|[<span data-ttu-id="d82f7-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="d82f7-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="d82f7-114">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="d82f7-114">The notification status for this app assignment.</span></span> <span data-ttu-id="d82f7-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="d82f7-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="d82f7-116">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="d82f7-116">restartSettings</span></span>|[<span data-ttu-id="d82f7-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="d82f7-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="d82f7-118">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="d82f7-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="d82f7-119">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="d82f7-119">installTimeSettings</span></span>|[<span data-ttu-id="d82f7-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="d82f7-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="d82f7-121">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="d82f7-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="d82f7-122">деливерйоптимизатионприорити</span><span class="sxs-lookup"><span data-stu-id="d82f7-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="d82f7-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="d82f7-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="d82f7-124">Приоритет оптимизации доставки для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="d82f7-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="d82f7-125">Этот параметр не поддерживается в национальных облачных средах.</span><span class="sxs-lookup"><span data-stu-id="d82f7-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="d82f7-126">Возможные значения: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="d82f7-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d82f7-127">Связи</span><span class="sxs-lookup"><span data-stu-id="d82f7-127">Relationships</span></span>
<span data-ttu-id="d82f7-128">Нет</span><span class="sxs-lookup"><span data-stu-id="d82f7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d82f7-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d82f7-129">JSON Representation</span></span>
<span data-ttu-id="d82f7-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d82f7-130">Here is a JSON representation of the resource.</span></span>
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



