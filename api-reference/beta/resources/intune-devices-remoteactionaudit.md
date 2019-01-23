---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ebe93b2f2e70011fb75a08b91938f26d723d1d5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404913"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="6121d-103">Тип ресурса remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="6121d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6121d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6121d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6121d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6121d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6121d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6121d-107">Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.</span><span class="sxs-lookup"><span data-stu-id="6121d-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="6121d-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6121d-108">Methods</span></span>
|<span data-ttu-id="6121d-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6121d-109">Method</span></span>|<span data-ttu-id="6121d-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6121d-110">Return Type</span></span>|<span data-ttu-id="6121d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6121d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6121d-112">Список remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="6121d-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="6121d-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="6121d-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="6121d-114">Свойства списка и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="6121d-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="6121d-115">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="6121d-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="6121d-117">Чтение свойства и связи объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="6121d-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="6121d-118">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="6121d-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="6121d-120">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="6121d-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="6121d-121">Удаление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="6121d-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6121d-122">None</span></span>|<span data-ttu-id="6121d-123">Удаляет [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="6121d-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="6121d-124">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="6121d-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="6121d-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="6121d-126">Обновление свойства объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="6121d-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6121d-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="6121d-127">Properties</span></span>
|<span data-ttu-id="6121d-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6121d-128">Property</span></span>|<span data-ttu-id="6121d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6121d-129">Type</span></span>|<span data-ttu-id="6121d-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6121d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6121d-131">id</span><span class="sxs-lookup"><span data-stu-id="6121d-131">id</span></span>|<span data-ttu-id="6121d-132">String</span><span class="sxs-lookup"><span data-stu-id="6121d-132">String</span></span>|<span data-ttu-id="6121d-133">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="6121d-133">Report Id.</span></span>|
|<span data-ttu-id="6121d-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6121d-134">deviceDisplayName</span></span>|<span data-ttu-id="6121d-135">String</span><span class="sxs-lookup"><span data-stu-id="6121d-135">String</span></span>|<span data-ttu-id="6121d-136">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="6121d-136">Intune device name.</span></span>|
|<span data-ttu-id="6121d-137">userName</span><span class="sxs-lookup"><span data-stu-id="6121d-137">userName</span></span>|<span data-ttu-id="6121d-138">String</span><span class="sxs-lookup"><span data-stu-id="6121d-138">String</span></span>|<span data-ttu-id="6121d-139">\[устаревшие\] вместо этого используйте InitiatedByUserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="6121d-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="6121d-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6121d-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="6121d-141">String</span><span class="sxs-lookup"><span data-stu-id="6121d-141">String</span></span>|<span data-ttu-id="6121d-142">Пользователя, который инициировал действие устройства имеет формат имени участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="6121d-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="6121d-143">action</span><span class="sxs-lookup"><span data-stu-id="6121d-143">action</span></span>|[<span data-ttu-id="6121d-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="6121d-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="6121d-145">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="6121d-145">The action name.</span></span> <span data-ttu-id="6121d-146">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="6121d-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="6121d-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="6121d-147">requestDateTime</span></span>|<span data-ttu-id="6121d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6121d-148">DateTimeOffset</span></span>|<span data-ttu-id="6121d-149">Время, когда действие был отправлен, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6121d-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="6121d-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6121d-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="6121d-151">String</span><span class="sxs-lookup"><span data-stu-id="6121d-151">String</span></span>|<span data-ttu-id="6121d-152">Имя участника-пользователя владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="6121d-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="6121d-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="6121d-153">deviceIMEI</span></span>|<span data-ttu-id="6121d-154">String</span><span class="sxs-lookup"><span data-stu-id="6121d-154">String</span></span>|<span data-ttu-id="6121d-155">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="6121d-155">IMEI of the device.</span></span>|
|<span data-ttu-id="6121d-156">actionState</span><span class="sxs-lookup"><span data-stu-id="6121d-156">actionState</span></span>|[<span data-ttu-id="6121d-157">actionState</span><span class="sxs-lookup"><span data-stu-id="6121d-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="6121d-158">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="6121d-158">Action state.</span></span> <span data-ttu-id="6121d-159">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="6121d-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6121d-160">Связи</span><span class="sxs-lookup"><span data-stu-id="6121d-160">Relationships</span></span>
<span data-ttu-id="6121d-161">Нет</span><span class="sxs-lookup"><span data-stu-id="6121d-161">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6121d-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6121d-162">JSON Representation</span></span>
<span data-ttu-id="6121d-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6121d-163">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteActionAudit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "initiatedByUserPrincipalName": "String",
  "action": "String",
  "requestDateTime": "String (timestamp)",
  "deviceOwnerUserPrincipalName": "String",
  "deviceIMEI": "String",
  "actionState": "String"
}
```




