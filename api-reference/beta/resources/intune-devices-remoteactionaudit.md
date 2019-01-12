---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad583f13311e5baece70c5ec28ca8f7c73f5349e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972595"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="53cdf-103">Тип ресурса remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="53cdf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="53cdf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53cdf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53cdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53cdf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="53cdf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53cdf-107">Отчет о удаленного действия, которые запускаются на устройствах, относящегося к определенной клиента.</span><span class="sxs-lookup"><span data-stu-id="53cdf-107">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="53cdf-108">Методы</span><span class="sxs-lookup"><span data-stu-id="53cdf-108">Methods</span></span>
|<span data-ttu-id="53cdf-109">Метод</span><span class="sxs-lookup"><span data-stu-id="53cdf-109">Method</span></span>|<span data-ttu-id="53cdf-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="53cdf-110">Return Type</span></span>|<span data-ttu-id="53cdf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="53cdf-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53cdf-112">Список remoteActionAudits</span><span class="sxs-lookup"><span data-stu-id="53cdf-112">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="53cdf-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="53cdf-113">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="53cdf-114">Свойства списка и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="53cdf-114">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="53cdf-115">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-115">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="53cdf-116">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-116">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="53cdf-117">Чтение свойства и связи объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="53cdf-117">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="53cdf-118">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-118">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="53cdf-119">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-119">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="53cdf-120">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="53cdf-120">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="53cdf-121">Удаление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-121">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="53cdf-122">Нет</span><span class="sxs-lookup"><span data-stu-id="53cdf-122">None</span></span>|<span data-ttu-id="53cdf-123">Удаляет [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="53cdf-123">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="53cdf-124">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-124">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="53cdf-125">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="53cdf-125">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="53cdf-126">Обновление свойства объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="53cdf-126">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53cdf-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="53cdf-127">Properties</span></span>
|<span data-ttu-id="53cdf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="53cdf-128">Property</span></span>|<span data-ttu-id="53cdf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="53cdf-129">Type</span></span>|<span data-ttu-id="53cdf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="53cdf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53cdf-131">id</span><span class="sxs-lookup"><span data-stu-id="53cdf-131">id</span></span>|<span data-ttu-id="53cdf-132">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-132">String</span></span>|<span data-ttu-id="53cdf-133">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="53cdf-133">Report Id.</span></span>|
|<span data-ttu-id="53cdf-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="53cdf-134">deviceDisplayName</span></span>|<span data-ttu-id="53cdf-135">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-135">String</span></span>|<span data-ttu-id="53cdf-136">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="53cdf-136">Intune device name.</span></span>|
|<span data-ttu-id="53cdf-137">userName</span><span class="sxs-lookup"><span data-stu-id="53cdf-137">userName</span></span>|<span data-ttu-id="53cdf-138">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-138">String</span></span>|<span data-ttu-id="53cdf-139">\[устаревшие\] вместо этого используйте InitiatedByUserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="53cdf-139">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="53cdf-140">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53cdf-140">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="53cdf-141">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-141">String</span></span>|<span data-ttu-id="53cdf-142">Пользователя, который инициировал действие устройства имеет формат имени участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="53cdf-142">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="53cdf-143">action</span><span class="sxs-lookup"><span data-stu-id="53cdf-143">action</span></span>|[<span data-ttu-id="53cdf-144">remoteAction</span><span class="sxs-lookup"><span data-stu-id="53cdf-144">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="53cdf-145">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="53cdf-145">The action name.</span></span> <span data-ttu-id="53cdf-146">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown` .</span><span class="sxs-lookup"><span data-stu-id="53cdf-146">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="53cdf-147">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="53cdf-147">requestDateTime</span></span>|<span data-ttu-id="53cdf-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53cdf-148">DateTimeOffset</span></span>|<span data-ttu-id="53cdf-149">Время, когда действие был отправлен, в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="53cdf-149">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="53cdf-150">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53cdf-150">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="53cdf-151">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-151">String</span></span>|<span data-ttu-id="53cdf-152">Имя участника-пользователя владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="53cdf-152">Upn of the device owner.</span></span>|
|<span data-ttu-id="53cdf-153">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="53cdf-153">deviceIMEI</span></span>|<span data-ttu-id="53cdf-154">String</span><span class="sxs-lookup"><span data-stu-id="53cdf-154">String</span></span>|<span data-ttu-id="53cdf-155">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="53cdf-155">IMEI of the device.</span></span>|
|<span data-ttu-id="53cdf-156">actionState</span><span class="sxs-lookup"><span data-stu-id="53cdf-156">actionState</span></span>|[<span data-ttu-id="53cdf-157">actionState</span><span class="sxs-lookup"><span data-stu-id="53cdf-157">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="53cdf-158">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="53cdf-158">Action state.</span></span> <span data-ttu-id="53cdf-159">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="53cdf-159">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53cdf-160">Связи</span><span class="sxs-lookup"><span data-stu-id="53cdf-160">Relationships</span></span>
<span data-ttu-id="53cdf-161">Нет</span><span class="sxs-lookup"><span data-stu-id="53cdf-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="53cdf-162">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="53cdf-162">JSON Representation</span></span>
<span data-ttu-id="53cdf-163">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53cdf-163">Here is a JSON representation of the resource.</span></span>
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





