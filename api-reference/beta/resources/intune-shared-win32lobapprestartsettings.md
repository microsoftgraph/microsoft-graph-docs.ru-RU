---
title: Тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие повторную координацию после установки приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84e4b231c189f02cf1e19401933ae517d8955263
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538765"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="ad293-103">Тип ресурса win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="ad293-103">win32LobAppRestartSettings resource type</span></span>

> <span data-ttu-id="ad293-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad293-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad293-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad293-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad293-106">Содержит свойства, описывающие повторную координацию после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="ad293-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="ad293-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad293-107">Properties</span></span>
|<span data-ttu-id="ad293-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad293-108">Property</span></span>|<span data-ttu-id="ad293-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ad293-109">Type</span></span>|<span data-ttu-id="ad293-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad293-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad293-111">грацепериодинминутес</span><span class="sxs-lookup"><span data-stu-id="ad293-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="ad293-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ad293-112">Int32</span></span>|<span data-ttu-id="ad293-113">Время ожидания перед перезапуском устройства после установки приложения (в минутах).</span><span class="sxs-lookup"><span data-stu-id="ad293-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="ad293-114">каунтдовндисплайбефоререстартинминутес</span><span class="sxs-lookup"><span data-stu-id="ad293-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="ad293-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ad293-115">Int32</span></span>|<span data-ttu-id="ad293-116">Время (в минутах) до того, как время перезапуска отображает диалоговое окно обратного отсчета для ожидающих перезапусков.</span><span class="sxs-lookup"><span data-stu-id="ad293-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="ad293-117">рестартнотификатионснузедуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="ad293-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="ad293-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ad293-118">Int32</span></span>|<span data-ttu-id="ad293-119">Количество минут, в течение которых будет отложиться диалоговое окно уведомления о перезапуске при нажатии кнопки "проложить".</span><span class="sxs-lookup"><span data-stu-id="ad293-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad293-120">Связи</span><span class="sxs-lookup"><span data-stu-id="ad293-120">Relationships</span></span>
<span data-ttu-id="ad293-121">Нет</span><span class="sxs-lookup"><span data-stu-id="ad293-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad293-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad293-122">JSON Representation</span></span>
<span data-ttu-id="ad293-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad293-123">Here is a JSON representation of the resource.</span></span>
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



