---
title: Тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие повторную координацию после установки приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31f9fefd725f59c9884e3fe4442a7154aaed4529
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255639"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="d6140-103">Тип ресурса win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="d6140-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="d6140-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6140-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6140-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6140-107">Содержит свойства, описывающие повторную координацию после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="d6140-107">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="d6140-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6140-108">Properties</span></span>
|<span data-ttu-id="d6140-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6140-109">Property</span></span>|<span data-ttu-id="d6140-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6140-110">Type</span></span>|<span data-ttu-id="d6140-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6140-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6140-112">грацепериодинминутес</span><span class="sxs-lookup"><span data-stu-id="d6140-112">gracePeriodInMinutes</span></span>|<span data-ttu-id="d6140-113">Int32</span><span class="sxs-lookup"><span data-stu-id="d6140-113">Int32</span></span>|<span data-ttu-id="d6140-114">Время ожидания перед перезапуском устройства после установки приложения (в минутах).</span><span class="sxs-lookup"><span data-stu-id="d6140-114">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="d6140-115">каунтдовндисплайбефоререстартинминутес</span><span class="sxs-lookup"><span data-stu-id="d6140-115">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="d6140-116">Int32</span><span class="sxs-lookup"><span data-stu-id="d6140-116">Int32</span></span>|<span data-ttu-id="d6140-117">Время (в минутах) до того, как время перезапуска отображает диалоговое окно обратного отсчета для ожидающих перезапусков.</span><span class="sxs-lookup"><span data-stu-id="d6140-117">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="d6140-118">рестартнотификатионснузедуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="d6140-118">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="d6140-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d6140-119">Int32</span></span>|<span data-ttu-id="d6140-120">Количество минут, в течение которых будет отложиться диалоговое окно уведомления о перезапуске при нажатии кнопки "проложить".</span><span class="sxs-lookup"><span data-stu-id="d6140-120">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6140-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d6140-121">Relationships</span></span>
<span data-ttu-id="d6140-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d6140-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6140-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6140-123">JSON Representation</span></span>
<span data-ttu-id="d6140-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6140-124">Here is a JSON representation of the resource.</span></span>
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




