---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c56d236c48918592394dc143bc6f2c45fb80401
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523501"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="43943-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="43943-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="43943-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="43943-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43943-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43943-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43943-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43943-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43943-107">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="43943-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="43943-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="43943-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43943-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="43943-109">Properties</span></span>
|<span data-ttu-id="43943-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="43943-110">Property</span></span>|<span data-ttu-id="43943-111">Тип</span><span class="sxs-lookup"><span data-stu-id="43943-111">Type</span></span>|<span data-ttu-id="43943-112">Описание</span><span class="sxs-lookup"><span data-stu-id="43943-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43943-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="43943-113">notifications</span></span>|[<span data-ttu-id="43943-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="43943-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="43943-115">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="43943-115">The notification status for this app assignment.</span></span> <span data-ttu-id="43943-116">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="43943-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="43943-117">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="43943-117">restartSettings</span></span>|[<span data-ttu-id="43943-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="43943-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="43943-119">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="43943-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="43943-120">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="43943-120">installTimeSettings</span></span>|[<span data-ttu-id="43943-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="43943-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="43943-122">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="43943-122">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43943-123">Связи</span><span class="sxs-lookup"><span data-stu-id="43943-123">Relationships</span></span>
<span data-ttu-id="43943-124">Нет</span><span class="sxs-lookup"><span data-stu-id="43943-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43943-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="43943-125">JSON Representation</span></span>
<span data-ttu-id="43943-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43943-126">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



