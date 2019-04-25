---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e7882a522eb3e3adcf9ebdf24e2b8f820b0f3581
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547048"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="761fe-103">Тип ресурса windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="761fe-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="761fe-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="761fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="761fe-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="761fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="761fe-106">Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="761fe-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="761fe-107">Методы</span><span class="sxs-lookup"><span data-stu-id="761fe-107">Methods</span></span>
|<span data-ttu-id="761fe-108">Метод</span><span class="sxs-lookup"><span data-stu-id="761fe-108">Method</span></span>|<span data-ttu-id="761fe-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="761fe-109">Return Type</span></span>|<span data-ttu-id="761fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="761fe-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="761fe-111">Получение windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="761fe-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="761fe-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="761fe-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="761fe-113">Чтение свойств и связей объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="761fe-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="761fe-114">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="761fe-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="761fe-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="761fe-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="761fe-116">Обновление свойств объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="761fe-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="761fe-117">Действие sync</span><span class="sxs-lookup"><span data-stu-id="761fe-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="761fe-118">Нет</span><span class="sxs-lookup"><span data-stu-id="761fe-118">None</span></span>|<span data-ttu-id="761fe-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="761fe-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="761fe-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="761fe-120">Properties</span></span>
|<span data-ttu-id="761fe-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="761fe-121">Property</span></span>|<span data-ttu-id="761fe-122">Тип</span><span class="sxs-lookup"><span data-stu-id="761fe-122">Type</span></span>|<span data-ttu-id="761fe-123">Описание</span><span class="sxs-lookup"><span data-stu-id="761fe-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="761fe-124">id</span><span class="sxs-lookup"><span data-stu-id="761fe-124">id</span></span>|<span data-ttu-id="761fe-125">String</span><span class="sxs-lookup"><span data-stu-id="761fe-125">String</span></span>|<span data-ttu-id="761fe-126">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="761fe-126">The GUID for the object</span></span>|
|<span data-ttu-id="761fe-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="761fe-127">lastSyncDateTime</span></span>|<span data-ttu-id="761fe-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="761fe-128">DateTimeOffset</span></span>|<span data-ttu-id="761fe-129">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="761fe-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="761fe-130">Ластмануалсинктригжердатетиме</span><span class="sxs-lookup"><span data-stu-id="761fe-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="761fe-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="761fe-131">DateTimeOffset</span></span>|<span data-ttu-id="761fe-132">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="761fe-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="761fe-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="761fe-133">syncStatus</span></span>|[<span data-ttu-id="761fe-134">Виндовсаутопилотсинкстатус</span><span class="sxs-lookup"><span data-stu-id="761fe-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="761fe-135">Указывает состояние синхронизации со службой синхронизации данных устройств (DDS).</span><span class="sxs-lookup"><span data-stu-id="761fe-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="761fe-136">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="761fe-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="761fe-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="761fe-137">Relationships</span></span>
<span data-ttu-id="761fe-138">Нет</span><span class="sxs-lookup"><span data-stu-id="761fe-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="761fe-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="761fe-139">JSON Representation</span></span>
<span data-ttu-id="761fe-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="761fe-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```





