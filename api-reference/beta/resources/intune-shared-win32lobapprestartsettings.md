---
title: Тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие повторную координацию после установки приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66e5bbfe925dfc6ee023e06d58b70aa4ed680ee4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766912"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="84f0d-103">Тип ресурса win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="84f0d-103">win32LobAppRestartSettings resource type</span></span>

> <span data-ttu-id="84f0d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84f0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84f0d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="84f0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84f0d-106">Содержит свойства, описывающие повторную координацию после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="84f0d-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="84f0d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="84f0d-107">Properties</span></span>
|<span data-ttu-id="84f0d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="84f0d-108">Property</span></span>|<span data-ttu-id="84f0d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="84f0d-109">Type</span></span>|<span data-ttu-id="84f0d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="84f0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84f0d-111">грацепериодинминутес</span><span class="sxs-lookup"><span data-stu-id="84f0d-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="84f0d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-112">Int32</span></span>|<span data-ttu-id="84f0d-113">Время ожидания перед перезапуском устройства после установки приложения (в минутах).</span><span class="sxs-lookup"><span data-stu-id="84f0d-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="84f0d-114">каунтдовндисплайбефоререстартинминутес</span><span class="sxs-lookup"><span data-stu-id="84f0d-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="84f0d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-115">Int32</span></span>|<span data-ttu-id="84f0d-116">Время (в минутах) до того, как время перезапуска отображает диалоговое окно обратного отсчета для ожидающих перезапусков.</span><span class="sxs-lookup"><span data-stu-id="84f0d-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="84f0d-117">рестартнотификатионснузедуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="84f0d-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="84f0d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="84f0d-118">Int32</span></span>|<span data-ttu-id="84f0d-119">Количество минут, в течение которых будет отложиться диалоговое окно уведомления о перезапуске при нажатии кнопки "проложить".</span><span class="sxs-lookup"><span data-stu-id="84f0d-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84f0d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="84f0d-120">Relationships</span></span>
<span data-ttu-id="84f0d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="84f0d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84f0d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84f0d-122">JSON Representation</span></span>
<span data-ttu-id="84f0d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84f0d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRestartSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRestartSettings",
  "gracePeriodInMinutes": 1024,
  "countdownDisplayBeforeRestartInMinutes": 1024,
  "restartNotificationSnoozeDurationInMinutes": 1024
}
```



