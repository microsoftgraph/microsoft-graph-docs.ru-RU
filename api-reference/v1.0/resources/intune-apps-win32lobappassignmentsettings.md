---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e84a740a45cb57417c81b5c99a892642097413b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020396"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="f4811-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f4811-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="f4811-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4811-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f4811-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f4811-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4811-106">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="f4811-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="f4811-107">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f4811-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4811-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4811-108">Properties</span></span>
|<span data-ttu-id="f4811-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4811-109">Property</span></span>|<span data-ttu-id="f4811-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f4811-110">Type</span></span>|<span data-ttu-id="f4811-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f4811-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4811-112">уведомления</span><span class="sxs-lookup"><span data-stu-id="f4811-112">notifications</span></span>|[<span data-ttu-id="f4811-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="f4811-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="f4811-114">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="f4811-114">The notification status for this app assignment.</span></span> <span data-ttu-id="f4811-115">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="f4811-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="f4811-116">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="f4811-116">restartSettings</span></span>|[<span data-ttu-id="f4811-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="f4811-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="f4811-118">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="f4811-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="f4811-119">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="f4811-119">installTimeSettings</span></span>|[<span data-ttu-id="f4811-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="f4811-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="f4811-121">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="f4811-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4811-122">Связи</span><span class="sxs-lookup"><span data-stu-id="f4811-122">Relationships</span></span>
<span data-ttu-id="f4811-123">Нет</span><span class="sxs-lookup"><span data-stu-id="f4811-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4811-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4811-124">JSON Representation</span></span>
<span data-ttu-id="f4811-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4811-125">Here is a JSON representation of the resource.</span></span>
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





