---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7bbdfa28061b48a0c2ca3ed2e0b714e1f1a1159
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989716"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="fb047-103">Тип ресурса windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="fb047-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="fb047-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb047-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb047-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb047-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb047-106">Ресурс windowsAutopilotSettings представляет учетную запись автопилота Windows для синхронизации данных с службой синхронизации данных устройств Windows.</span><span class="sxs-lookup"><span data-stu-id="fb047-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="fb047-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fb047-107">Methods</span></span>
|<span data-ttu-id="fb047-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fb047-108">Method</span></span>|<span data-ttu-id="fb047-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb047-109">Return Type</span></span>|<span data-ttu-id="fb047-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fb047-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fb047-111">Получение windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="fb047-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="fb047-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="fb047-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="fb047-113">Чтение свойств и связей объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="fb047-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="fb047-114">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="fb047-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="fb047-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="fb047-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="fb047-116">Обновление свойств объекта [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) .</span><span class="sxs-lookup"><span data-stu-id="fb047-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="fb047-117">Действие sync</span><span class="sxs-lookup"><span data-stu-id="fb047-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="fb047-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fb047-118">None</span></span>|<span data-ttu-id="fb047-119">Н/Д</span><span class="sxs-lookup"><span data-stu-id="fb047-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fb047-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb047-120">Properties</span></span>
|<span data-ttu-id="fb047-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb047-121">Property</span></span>|<span data-ttu-id="fb047-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fb047-122">Type</span></span>|<span data-ttu-id="fb047-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fb047-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb047-124">id</span><span class="sxs-lookup"><span data-stu-id="fb047-124">id</span></span>|<span data-ttu-id="fb047-125">String</span><span class="sxs-lookup"><span data-stu-id="fb047-125">String</span></span>|<span data-ttu-id="fb047-126">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="fb047-126">The GUID for the object</span></span>|
|<span data-ttu-id="fb047-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fb047-127">lastSyncDateTime</span></span>|<span data-ttu-id="fb047-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb047-128">DateTimeOffset</span></span>|<span data-ttu-id="fb047-129">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="fb047-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="fb047-130">Ластмануалсинктригжердатетиме</span><span class="sxs-lookup"><span data-stu-id="fb047-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="fb047-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb047-131">DateTimeOffset</span></span>|<span data-ttu-id="fb047-132">Дата и время последней синхронизации данных в службе DDS.</span><span class="sxs-lookup"><span data-stu-id="fb047-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="fb047-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="fb047-133">syncStatus</span></span>|[<span data-ttu-id="fb047-134">Виндовсаутопилотсинкстатус</span><span class="sxs-lookup"><span data-stu-id="fb047-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="fb047-135">Указывает состояние синхронизации со службой синхронизации данных устройств (DDS).</span><span class="sxs-lookup"><span data-stu-id="fb047-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="fb047-136">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="fb047-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb047-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="fb047-137">Relationships</span></span>
<span data-ttu-id="fb047-138">Нет</span><span class="sxs-lookup"><span data-stu-id="fb047-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb047-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb047-139">JSON Representation</span></span>
<span data-ttu-id="fb047-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb047-140">Here is a JSON representation of the resource.</span></span>
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





