---
title: Тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие повторную координацию после установки приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d60cbb11e5b08fc0badd651b846f3d108e12af5b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48036769"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="47792-103">Тип ресурса win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="47792-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="47792-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47792-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47792-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47792-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47792-106">Содержит свойства, описывающие повторную координацию после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="47792-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="47792-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="47792-107">Properties</span></span>
|<span data-ttu-id="47792-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="47792-108">Property</span></span>|<span data-ttu-id="47792-109">Тип</span><span class="sxs-lookup"><span data-stu-id="47792-109">Type</span></span>|<span data-ttu-id="47792-110">Описание</span><span class="sxs-lookup"><span data-stu-id="47792-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47792-111">грацепериодинминутес</span><span class="sxs-lookup"><span data-stu-id="47792-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="47792-112">Int32</span><span class="sxs-lookup"><span data-stu-id="47792-112">Int32</span></span>|<span data-ttu-id="47792-113">Время ожидания перед перезапуском устройства после установки приложения (в минутах).</span><span class="sxs-lookup"><span data-stu-id="47792-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="47792-114">каунтдовндисплайбефоререстартинминутес</span><span class="sxs-lookup"><span data-stu-id="47792-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="47792-115">Int32</span><span class="sxs-lookup"><span data-stu-id="47792-115">Int32</span></span>|<span data-ttu-id="47792-116">Время (в минутах) до того, как время перезапуска отображает диалоговое окно обратного отсчета для ожидающих перезапусков.</span><span class="sxs-lookup"><span data-stu-id="47792-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="47792-117">рестартнотификатионснузедуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="47792-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="47792-118">Int32</span><span class="sxs-lookup"><span data-stu-id="47792-118">Int32</span></span>|<span data-ttu-id="47792-119">Количество минут, в течение которых будет отложиться диалоговое окно уведомления о перезапуске при нажатии кнопки "проложить".</span><span class="sxs-lookup"><span data-stu-id="47792-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47792-120">Связи</span><span class="sxs-lookup"><span data-stu-id="47792-120">Relationships</span></span>
<span data-ttu-id="47792-121">Нет</span><span class="sxs-lookup"><span data-stu-id="47792-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47792-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47792-122">JSON Representation</span></span>
<span data-ttu-id="47792-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47792-123">Here is a JSON representation of the resource.</span></span>
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





