---
title: Тип ресурса remoteActionAudit
description: Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 369cf366cb05aca8b826f9f4a6df8c47fa95f471
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196744"
---
# <a name="remoteactionaudit-resource-type"></a><span data-ttu-id="d586d-103">Тип ресурса remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-103">remoteActionAudit resource type</span></span>

> <span data-ttu-id="d586d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d586d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d586d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d586d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d586d-106">Отчет о удаленных действиях, запущенных на устройствах, относящихся к определенному клиенту.</span><span class="sxs-lookup"><span data-stu-id="d586d-106">Report of remote actions initiated on the devices belonging to a certain tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="d586d-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d586d-107">Methods</span></span>
|<span data-ttu-id="d586d-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d586d-108">Method</span></span>|<span data-ttu-id="d586d-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d586d-109">Return Type</span></span>|<span data-ttu-id="d586d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d586d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d586d-111">Список Ремотеактионаудитс</span><span class="sxs-lookup"><span data-stu-id="d586d-111">List remoteActionAudits</span></span>](../api/intune-devices-remoteactionaudit-list.md)|<span data-ttu-id="d586d-112">Коллекция [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="d586d-112">[remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) collection</span></span>|<span data-ttu-id="d586d-113">Список свойств и связей объектов [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="d586d-113">List properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) objects.</span></span>|
|[<span data-ttu-id="d586d-114">Получение remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-114">Get remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-get.md)|[<span data-ttu-id="d586d-115">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-115">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="d586d-116">Чтение свойств и связей объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="d586d-116">Read properties and relationships of the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="d586d-117">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-117">Create remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-create.md)|[<span data-ttu-id="d586d-118">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-118">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="d586d-119">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="d586d-119">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|
|[<span data-ttu-id="d586d-120">Удаление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-120">Delete remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-delete.md)|<span data-ttu-id="d586d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d586d-121">None</span></span>|<span data-ttu-id="d586d-122">Удаляет объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="d586d-122">Deletes a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>|
|[<span data-ttu-id="d586d-123">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-123">Update remoteActionAudit</span></span>](../api/intune-devices-remoteactionaudit-update.md)|[<span data-ttu-id="d586d-124">remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="d586d-124">remoteActionAudit</span></span>](../resources/intune-devices-remoteactionaudit.md)|<span data-ttu-id="d586d-125">Обновление свойств объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="d586d-125">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d586d-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="d586d-126">Properties</span></span>
|<span data-ttu-id="d586d-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="d586d-127">Property</span></span>|<span data-ttu-id="d586d-128">Тип</span><span class="sxs-lookup"><span data-stu-id="d586d-128">Type</span></span>|<span data-ttu-id="d586d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="d586d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d586d-130">id</span><span class="sxs-lookup"><span data-stu-id="d586d-130">id</span></span>|<span data-ttu-id="d586d-131">String</span><span class="sxs-lookup"><span data-stu-id="d586d-131">String</span></span>|<span data-ttu-id="d586d-132">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="d586d-132">Report Id.</span></span>|
|<span data-ttu-id="d586d-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d586d-133">deviceDisplayName</span></span>|<span data-ttu-id="d586d-134">String</span><span class="sxs-lookup"><span data-stu-id="d586d-134">String</span></span>|<span data-ttu-id="d586d-135">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="d586d-135">Intune device name.</span></span>|
|<span data-ttu-id="d586d-136">userName</span><span class="sxs-lookup"><span data-stu-id="d586d-136">userName</span></span>|<span data-ttu-id="d586d-137">String.</span><span class="sxs-lookup"><span data-stu-id="d586d-137">String</span></span>|<span data-ttu-id="d586d-138">\[\] рекомендуется вместо этого использовать свойства initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="d586d-138">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="d586d-139">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="d586d-139">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="d586d-140">String.</span><span class="sxs-lookup"><span data-stu-id="d586d-140">String</span></span>|<span data-ttu-id="d586d-141">Пользователь, который инициировал действие с устройством, имеет формат UPN.</span><span class="sxs-lookup"><span data-stu-id="d586d-141">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="d586d-142">action</span><span class="sxs-lookup"><span data-stu-id="d586d-142">action</span></span>|[<span data-ttu-id="d586d-143">ремотеактион</span><span class="sxs-lookup"><span data-stu-id="d586d-143">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="d586d-144">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="d586d-144">The action name.</span></span> <span data-ttu-id="d586d-145">Возможные значения: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `logoutSharedAppleDeviceActiveUser` `quickScan`,,,,,,,,,,,,,,,,,,,,, `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` , `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span><span class="sxs-lookup"><span data-stu-id="d586d-145">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="d586d-146">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="d586d-146">requestDateTime</span></span>|<span data-ttu-id="d586d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d586d-147">DateTimeOffset</span></span>|<span data-ttu-id="d586d-148">Время, когда действие было выдано, заданное в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d586d-148">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="d586d-149">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d586d-149">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="d586d-150">String.</span><span class="sxs-lookup"><span data-stu-id="d586d-150">String</span></span>|<span data-ttu-id="d586d-151">Имя участника-пользователя для владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="d586d-151">Upn of the device owner.</span></span>|
|<span data-ttu-id="d586d-152">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="d586d-152">deviceIMEI</span></span>|<span data-ttu-id="d586d-153">String.</span><span class="sxs-lookup"><span data-stu-id="d586d-153">String</span></span>|<span data-ttu-id="d586d-154">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="d586d-154">IMEI of the device.</span></span>|
|<span data-ttu-id="d586d-155">actionState</span><span class="sxs-lookup"><span data-stu-id="d586d-155">actionState</span></span>|[<span data-ttu-id="d586d-156">actionState</span><span class="sxs-lookup"><span data-stu-id="d586d-156">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d586d-157">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="d586d-157">Action state.</span></span> <span data-ttu-id="d586d-158">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d586d-158">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d586d-159">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="d586d-159">managedDeviceId</span></span>|<span data-ttu-id="d586d-160">String.</span><span class="sxs-lookup"><span data-stu-id="d586d-160">String</span></span>|<span data-ttu-id="d586d-161">Цель действия.</span><span class="sxs-lookup"><span data-stu-id="d586d-161">Action target.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d586d-162">Отношения</span><span class="sxs-lookup"><span data-stu-id="d586d-162">Relationships</span></span>
<span data-ttu-id="d586d-163">Нет</span><span class="sxs-lookup"><span data-stu-id="d586d-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d586d-164">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d586d-164">JSON Representation</span></span>
<span data-ttu-id="d586d-165">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d586d-165">Here is a JSON representation of the resource.</span></span>
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
  "actionState": "String",
  "managedDeviceId": "String"
}
```



