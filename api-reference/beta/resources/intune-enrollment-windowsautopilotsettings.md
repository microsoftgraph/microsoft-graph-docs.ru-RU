---
title: Тип ресурса windowsAutopilotSettings
description: Ресурс windowsAutopilotSettings представляет учетную запись Windows Autopilot для синхронизации данных со службой синхронизации данных устройств с Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e49191d204a040327c510606c6ca8186644beb7
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159530"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="8047e-103">Тип ресурса windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="8047e-103">windowsAutopilotSettings resource type</span></span>

<span data-ttu-id="8047e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8047e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8047e-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8047e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8047e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8047e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8047e-107">Ресурс windowsAutopilotSettings представляет учетную запись Windows Autopilot для синхронизации данных со службой синхронизации данных устройств с Windows.</span><span class="sxs-lookup"><span data-stu-id="8047e-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="8047e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="8047e-108">Methods</span></span>
|<span data-ttu-id="8047e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="8047e-109">Method</span></span>|<span data-ttu-id="8047e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8047e-110">Return Type</span></span>|<span data-ttu-id="8047e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8047e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8047e-112">Get windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="8047e-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="8047e-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="8047e-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="8047e-114">Чтение свойств и связей объекта [windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8047e-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="8047e-115">Обновление windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="8047e-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="8047e-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="8047e-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="8047e-117">Обновление свойств объекта [windowsAutopilotSettings.](../resources/intune-enrollment-windowsautopilotsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8047e-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="8047e-118">Действие sync</span><span class="sxs-lookup"><span data-stu-id="8047e-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="8047e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8047e-119">None</span></span>|<span data-ttu-id="8047e-120">Инициирует синхронизацию всех зарегистрированных AutoPilot устройств из Магазина для бизнеса и других порталов.</span><span class="sxs-lookup"><span data-stu-id="8047e-120">Initiates a sync of all AutoPilot registered devices from Store for Business and other portals.</span></span> <span data-ttu-id="8047e-121">Если синхронизация прошла успешно, это действие возвращает код отклика "204 Без содержимого".</span><span class="sxs-lookup"><span data-stu-id="8047e-121">If the sync successful, this action returns a 204 No Content response code.</span></span> <span data-ttu-id="8047e-122">Если синхронизация уже идет, действие возвращает код ответа на конфликт 409.</span><span class="sxs-lookup"><span data-stu-id="8047e-122">If a sync is already in progress, the action returns a 409 Conflict response code.</span></span>  <span data-ttu-id="8047e-123">Если это действие синхронизации вызвано в течение 10 минут после предыдущей синхронизации, это действие возвращает код ответа 429 Too Many Requests.</span><span class="sxs-lookup"><span data-stu-id="8047e-123">If this sync action is called within 10 minutes of the previous sync, the action returns a 429 Too Many Requests response code.</span></span>|

## <a name="properties"></a><span data-ttu-id="8047e-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="8047e-124">Properties</span></span>
|<span data-ttu-id="8047e-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="8047e-125">Property</span></span>|<span data-ttu-id="8047e-126">Тип</span><span class="sxs-lookup"><span data-stu-id="8047e-126">Type</span></span>|<span data-ttu-id="8047e-127">Описание</span><span class="sxs-lookup"><span data-stu-id="8047e-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8047e-128">id</span><span class="sxs-lookup"><span data-stu-id="8047e-128">id</span></span>|<span data-ttu-id="8047e-129">String</span><span class="sxs-lookup"><span data-stu-id="8047e-129">String</span></span>|<span data-ttu-id="8047e-130">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="8047e-130">The GUID for the object</span></span>|
|<span data-ttu-id="8047e-131">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8047e-131">lastSyncDateTime</span></span>|<span data-ttu-id="8047e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8047e-132">DateTimeOffset</span></span>|<span data-ttu-id="8047e-133">Время последней даты синхронизации данных со службой DDS.</span><span class="sxs-lookup"><span data-stu-id="8047e-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="8047e-134">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="8047e-134">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="8047e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8047e-135">DateTimeOffset</span></span>|<span data-ttu-id="8047e-136">Время последней синхронизации данных со службой DDS.</span><span class="sxs-lookup"><span data-stu-id="8047e-136">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="8047e-137">syncStatus</span><span class="sxs-lookup"><span data-stu-id="8047e-137">syncStatus</span></span>|[<span data-ttu-id="8047e-138">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8047e-138">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="8047e-139">Указывает состояние синхронизации со службой синхронизации данных устройства (DDS).</span><span class="sxs-lookup"><span data-stu-id="8047e-139">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="8047e-140">Возможные значения: `unknown`, `inProgress`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8047e-140">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8047e-141">Связи</span><span class="sxs-lookup"><span data-stu-id="8047e-141">Relationships</span></span>
<span data-ttu-id="8047e-142">Нет</span><span class="sxs-lookup"><span data-stu-id="8047e-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8047e-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8047e-143">JSON Representation</span></span>
<span data-ttu-id="8047e-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8047e-144">Here is a JSON representation of the resource.</span></span>
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




