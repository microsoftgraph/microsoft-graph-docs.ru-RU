---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e1f650919e3e7cd9fa55d7e05d3fc706b18f95db
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538695"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="56d7d-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="56d7d-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="56d7d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56d7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56d7d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="56d7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56d7d-106">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="56d7d-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="56d7d-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="56d7d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56d7d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="56d7d-108">Properties</span></span>
|<span data-ttu-id="56d7d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="56d7d-109">Property</span></span>|<span data-ttu-id="56d7d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="56d7d-110">Type</span></span>|<span data-ttu-id="56d7d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="56d7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56d7d-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="56d7d-112">notifications</span></span>|[<span data-ttu-id="56d7d-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="56d7d-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="56d7d-114">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="56d7d-114">The notification status for this app assignment.</span></span> <span data-ttu-id="56d7d-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="56d7d-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="56d7d-116">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="56d7d-116">restartSettings</span></span>|[<span data-ttu-id="56d7d-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="56d7d-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="56d7d-118">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="56d7d-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="56d7d-119">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="56d7d-119">installTimeSettings</span></span>|[<span data-ttu-id="56d7d-120">мобилеаппинсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="56d7d-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="56d7d-121">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="56d7d-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56d7d-122">Связи</span><span class="sxs-lookup"><span data-stu-id="56d7d-122">Relationships</span></span>
<span data-ttu-id="56d7d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="56d7d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56d7d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56d7d-124">JSON Representation</span></span>
<span data-ttu-id="56d7d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56d7d-125">Here is a JSON representation of the resource.</span></span>
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



