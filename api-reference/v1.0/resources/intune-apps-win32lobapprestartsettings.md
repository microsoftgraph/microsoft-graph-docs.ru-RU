---
title: тип ресурса win32LobAppRestartSettings
description: Содержит свойства, описывающие координацию перезапуска после установки приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1db011486f1ec26afcc7e045afd2e1be1b553ec7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757832"
---
# <a name="win32lobapprestartsettings-resource-type"></a><span data-ttu-id="455cf-103">тип ресурса win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="455cf-103">win32LobAppRestartSettings resource type</span></span>

<span data-ttu-id="455cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="455cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="455cf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="455cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="455cf-106">Содержит свойства, описывающие координацию перезапуска после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="455cf-106">Contains properties describing restart coordination following an app installation.</span></span>

## <a name="properties"></a><span data-ttu-id="455cf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="455cf-107">Properties</span></span>
|<span data-ttu-id="455cf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="455cf-108">Property</span></span>|<span data-ttu-id="455cf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="455cf-109">Type</span></span>|<span data-ttu-id="455cf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="455cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="455cf-111">gracePeriodInMinutes</span><span class="sxs-lookup"><span data-stu-id="455cf-111">gracePeriodInMinutes</span></span>|<span data-ttu-id="455cf-112">Int32</span><span class="sxs-lookup"><span data-stu-id="455cf-112">Int32</span></span>|<span data-ttu-id="455cf-113">Количество минут, которые необходимо подождать перед перезапуском устройства после установки приложения.</span><span class="sxs-lookup"><span data-stu-id="455cf-113">The number of minutes to wait before restarting the device after an app installation.</span></span>|
|<span data-ttu-id="455cf-114">countdownDisplayBeforeRestartInMinutes</span><span class="sxs-lookup"><span data-stu-id="455cf-114">countdownDisplayBeforeRestartInMinutes</span></span>|<span data-ttu-id="455cf-115">Int32</span><span class="sxs-lookup"><span data-stu-id="455cf-115">Int32</span></span>|<span data-ttu-id="455cf-116">Количество минут до начала перезагрузки, чтобы отобразить диалоговое окно обратного отсчета для ожидающих перезапусков.</span><span class="sxs-lookup"><span data-stu-id="455cf-116">The number of minutes before the restart time to display the countdown dialog for pending restarts.</span></span>|
|<span data-ttu-id="455cf-117">restartNotificationSnoozeDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="455cf-117">restartNotificationSnoozeDurationInMinutes</span></span>|<span data-ttu-id="455cf-118">Int32</span><span class="sxs-lookup"><span data-stu-id="455cf-118">Int32</span></span>|<span data-ttu-id="455cf-119">Количество минут, за которые нужно отсмеять диалоговое окно уведомления о перезапуске при выборе кнопки snooze.</span><span class="sxs-lookup"><span data-stu-id="455cf-119">The number of minutes to snooze the restart notification dialog when the snooze button is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="455cf-120">Связи</span><span class="sxs-lookup"><span data-stu-id="455cf-120">Relationships</span></span>
<span data-ttu-id="455cf-121">Нет</span><span class="sxs-lookup"><span data-stu-id="455cf-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="455cf-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="455cf-122">JSON Representation</span></span>
<span data-ttu-id="455cf-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="455cf-123">Here is a JSON representation of the resource.</span></span>
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




