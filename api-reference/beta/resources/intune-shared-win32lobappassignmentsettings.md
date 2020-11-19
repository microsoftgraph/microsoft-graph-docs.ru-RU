---
title: Тип ресурса win32LobAppAssignmentSettings
description: Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8de4c50115ccd819eca623bc4c3dd64d9b7bb49d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255779"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="61755-103">Тип ресурса win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="61755-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="61755-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61755-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61755-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61755-107">Содержит свойства, используемые для назначения бизнес-приложения Win32 для группы.</span><span class="sxs-lookup"><span data-stu-id="61755-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="61755-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="61755-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61755-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="61755-109">Properties</span></span>
|<span data-ttu-id="61755-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="61755-110">Property</span></span>|<span data-ttu-id="61755-111">Тип</span><span class="sxs-lookup"><span data-stu-id="61755-111">Type</span></span>|<span data-ttu-id="61755-112">Описание</span><span class="sxs-lookup"><span data-stu-id="61755-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61755-113">уведомления</span><span class="sxs-lookup"><span data-stu-id="61755-113">notifications</span></span>|[<span data-ttu-id="61755-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="61755-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="61755-115">Состояние уведомления для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="61755-115">The notification status for this app assignment.</span></span> <span data-ttu-id="61755-116">Возможные значения: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="61755-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="61755-117">рестартсеттингс</span><span class="sxs-lookup"><span data-stu-id="61755-117">restartSettings</span></span>|[<span data-ttu-id="61755-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="61755-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="61755-119">Параметры перезагрузки, которые необходимо применить к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="61755-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="61755-120">инсталлтимесеттингс</span><span class="sxs-lookup"><span data-stu-id="61755-120">installTimeSettings</span></span>|[<span data-ttu-id="61755-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="61755-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="61755-122">Параметры времени установки, применяемые к данному назначению приложения.</span><span class="sxs-lookup"><span data-stu-id="61755-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="61755-123">деливерйоптимизатионприорити</span><span class="sxs-lookup"><span data-stu-id="61755-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="61755-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="61755-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="61755-125">Приоритет оптимизации доставки для этого назначения приложения.</span><span class="sxs-lookup"><span data-stu-id="61755-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="61755-126">Этот параметр не поддерживается в национальных облачных средах.</span><span class="sxs-lookup"><span data-stu-id="61755-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="61755-127">Возможные значения: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="61755-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61755-128">Связи</span><span class="sxs-lookup"><span data-stu-id="61755-128">Relationships</span></span>
<span data-ttu-id="61755-129">Нет</span><span class="sxs-lookup"><span data-stu-id="61755-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61755-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61755-130">JSON Representation</span></span>
<span data-ttu-id="61755-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61755-131">Here is a JSON representation of the resource.</span></span>
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




