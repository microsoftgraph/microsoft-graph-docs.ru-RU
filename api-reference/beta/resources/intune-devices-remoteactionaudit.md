---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c06f7472addff7c475eeeb8ac3f1a26cc7ea78bc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165879"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="4a030-103">Тип ресурса remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="4a030-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a030-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a030-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4a030-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a030-106">Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.</span><span class="sxs-lookup"><span data-stu-id="4a030-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="4a030-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4a030-107">Methods</span></span>
|<span data-ttu-id="4a030-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4a030-108">Method</span></span>|<span data-ttu-id="4a030-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4a030-109">Return Type</span></span>|<span data-ttu-id="4a030-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4a030-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4a030-111">Список Ремотеактионаудитс</span><span class="sxs-lookup"><span data-stu-id="4a030-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="4a030-112">Коллекция [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="4a030-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="4a030-113">Список свойств и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="4a030-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="4a030-114">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="4a030-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="4a030-116">Чтение свойств и связей объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="4a030-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="4a030-117">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="4a030-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="4a030-119">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="4a030-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="4a030-120">Удаление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="4a030-121">Нет</span><span class="sxs-lookup"><span data-stu-id="4a030-121">None</span></span>|<span data-ttu-id="4a030-122">Удаляет объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="4a030-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="4a030-123">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="4a030-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="4a030-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="4a030-125">Обновление свойств объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="4a030-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a030-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a030-126">Properties</span></span>
|<span data-ttu-id="4a030-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a030-127">Property</span></span>|<span data-ttu-id="4a030-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4a030-128">Type</span></span>|<span data-ttu-id="4a030-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4a030-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a030-130">id</span><span class="sxs-lookup"><span data-stu-id="4a030-130">id</span></span>|<span data-ttu-id="4a030-131">Строка</span><span class="sxs-lookup"><span data-stu-id="4a030-131">String</span></span>|<span data-ttu-id="4a030-132">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="4a030-132">Report Id.</span></span>|
|<span data-ttu-id="4a030-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4a030-133">deviceDisplayName</span></span>|<span data-ttu-id="4a030-134">String</span><span class="sxs-lookup"><span data-stu-id="4a030-134">String</span></span>|<span data-ttu-id="4a030-135">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="4a030-135">Intune device name.</span></span>|
|<span data-ttu-id="4a030-136">userName</span><span class="sxs-lookup"><span data-stu-id="4a030-136">userName</span></span>|<span data-ttu-id="4a030-137">String</span><span class="sxs-lookup"><span data-stu-id="4a030-137">String</span></span>|<span data-ttu-id="4a030-138">\[\] рекомендуется вместо этого использовать свойства initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="4a030-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="4a030-139">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="4a030-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="4a030-140">String</span><span class="sxs-lookup"><span data-stu-id="4a030-140">String</span></span>|<span data-ttu-id="4a030-141">Пользователь, который инициировал действие с устройством, имеет формат UPN.</span><span class="sxs-lookup"><span data-stu-id="4a030-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="4a030-142">action</span><span class="sxs-lookup"><span data-stu-id="4a030-142">action</span></span>|[<span data-ttu-id="4a030-143">Ремотеактион</span><span class="sxs-lookup"><span data-stu-id="4a030-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="4a030-144">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="4a030-144">The action name.</span></span> <span data-ttu-id="4a030-145">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `logoutSharedAppleDeviceActiveUser` `quickScan`,,,,,,,,,,,,,,,,,,,,, `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` .</span><span class="sxs-lookup"><span data-stu-id="4a030-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`.</span></span>|
|<span data-ttu-id="4a030-146">Рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="4a030-146">requestDateTime</span></span>|<span data-ttu-id="4a030-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a030-147">DateTimeOffset</span></span>|<span data-ttu-id="4a030-148">Время, когда действие было выдано, заданное в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="4a030-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="4a030-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4a030-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="4a030-150">String</span><span class="sxs-lookup"><span data-stu-id="4a030-150">String</span></span>|<span data-ttu-id="4a030-151">Имя участника-пользователя для владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="4a030-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="4a030-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="4a030-152">deviceIMEI</span></span>|<span data-ttu-id="4a030-153">String</span><span class="sxs-lookup"><span data-stu-id="4a030-153">String</span></span>|<span data-ttu-id="4a030-154">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="4a030-154">IMEI of the device.</span></span>|
|<span data-ttu-id="4a030-155">actionState</span><span class="sxs-lookup"><span data-stu-id="4a030-155">actionState</span></span>|[<span data-ttu-id="4a030-156">actionState</span><span class="sxs-lookup"><span data-stu-id="4a030-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="4a030-157">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="4a030-157">Action state.</span></span> <span data-ttu-id="4a030-158">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="4a030-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a030-159">Связи</span><span class="sxs-lookup"><span data-stu-id="4a030-159">Relationships</span></span>
<span data-ttu-id="4a030-160">Нет</span><span class="sxs-lookup"><span data-stu-id="4a030-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a030-161">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a030-161">JSON Representation</span></span>
<span data-ttu-id="4a030-162">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a030-162">Here is a JSON representation of the resource.</span></span>
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




