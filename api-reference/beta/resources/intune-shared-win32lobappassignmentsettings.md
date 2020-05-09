---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 53872d032bbb61cf57d191f1b58f1878ba5c0a91
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177662"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="7eb27-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7eb27-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="7eb27-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7eb27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7eb27-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7eb27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7eb27-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7eb27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7eb27-107">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="7eb27-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="7eb27-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7eb27-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7eb27-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="7eb27-109">Properties</span></span>
|<span data-ttu-id="7eb27-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="7eb27-110">Property</span></span>|<span data-ttu-id="7eb27-111">Тип</span><span class="sxs-lookup"><span data-stu-id="7eb27-111">Type</span></span>|<span data-ttu-id="7eb27-112">Описание</span><span class="sxs-lookup"><span data-stu-id="7eb27-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eb27-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="7eb27-113">notifications</span></span>|[<span data-ttu-id="7eb27-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="7eb27-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="7eb27-115">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="7eb27-115">The notification status for this app assignment.</span></span> <span data-ttu-id="7eb27-116">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="7eb27-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="7eb27-117">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="7eb27-117">restartSettings</span></span>|[<span data-ttu-id="7eb27-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="7eb27-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="7eb27-119">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="7eb27-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="7eb27-120">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="7eb27-120">installTimeSettings</span></span>|[<span data-ttu-id="7eb27-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="7eb27-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="7eb27-122">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="7eb27-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="7eb27-123">деливерйоптимизатионприорити</span><span class="sxs-lookup"><span data-stu-id="7eb27-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="7eb27-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="7eb27-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="7eb27-125">Приоритет оптимизации доставки для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="7eb27-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="7eb27-126">Этот параметр не поддерживается в национальных облачных средах.</span><span class="sxs-lookup"><span data-stu-id="7eb27-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="7eb27-127">Возможные значения: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="7eb27-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eb27-128">Связи</span><span class="sxs-lookup"><span data-stu-id="7eb27-128">Relationships</span></span>
<span data-ttu-id="7eb27-129">Нет</span><span class="sxs-lookup"><span data-stu-id="7eb27-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7eb27-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7eb27-130">JSON Representation</span></span>
<span data-ttu-id="7eb27-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7eb27-131">Here is a JSON representation of the resource.</span></span>
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



