---
title: Обновление remoteActionAudit
description: Обновление свойств объекта remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7f579d5f982daa1bc1ab045cfca464a8f3b6d5f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43323453"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="c33d5-103">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="c33d5-103">Update remoteActionAudit</span></span>

<span data-ttu-id="c33d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c33d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c33d5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c33d5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c33d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c33d5-107">Обновление свойств объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="c33d5-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c33d5-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c33d5-108">Prerequisites</span></span>
<span data-ttu-id="c33d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c33d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c33d5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c33d5-111">Permission type</span></span>|<span data-ttu-id="c33d5-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c33d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c33d5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c33d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c33d5-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c33d5-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c33d5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c33d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c33d5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c33d5-116">Not supported.</span></span>|
|<span data-ttu-id="c33d5-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c33d5-117">Application</span></span>|<span data-ttu-id="c33d5-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c33d5-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c33d5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c33d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="c33d5-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c33d5-120">Request headers</span></span>
|<span data-ttu-id="c33d5-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c33d5-121">Header</span></span>|<span data-ttu-id="c33d5-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c33d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c33d5-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c33d5-123">Authorization</span></span>|<span data-ttu-id="c33d5-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c33d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c33d5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c33d5-125">Accept</span></span>|<span data-ttu-id="c33d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c33d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c33d5-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c33d5-127">Request body</span></span>
<span data-ttu-id="c33d5-128">В тексте запроса добавьте представление объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c33d5-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="c33d5-129">В следующей таблице приведены свойства, необходимые при создании [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span><span class="sxs-lookup"><span data-stu-id="c33d5-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="c33d5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c33d5-130">Property</span></span>|<span data-ttu-id="c33d5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c33d5-131">Type</span></span>|<span data-ttu-id="c33d5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c33d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c33d5-133">id</span><span class="sxs-lookup"><span data-stu-id="c33d5-133">id</span></span>|<span data-ttu-id="c33d5-134">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-134">String</span></span>|<span data-ttu-id="c33d5-135">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="c33d5-135">Report Id.</span></span>|
|<span data-ttu-id="c33d5-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c33d5-136">deviceDisplayName</span></span>|<span data-ttu-id="c33d5-137">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-137">String</span></span>|<span data-ttu-id="c33d5-138">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="c33d5-138">Intune device name.</span></span>|
|<span data-ttu-id="c33d5-139">userName</span><span class="sxs-lookup"><span data-stu-id="c33d5-139">userName</span></span>|<span data-ttu-id="c33d5-140">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-140">String</span></span>|<span data-ttu-id="c33d5-141">\[\] рекомендуется вместо этого использовать свойства initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="c33d5-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="c33d5-142">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="c33d5-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="c33d5-143">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-143">String</span></span>|<span data-ttu-id="c33d5-144">Пользователь, который инициировал действие с устройством, имеет формат UPN.</span><span class="sxs-lookup"><span data-stu-id="c33d5-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="c33d5-145">action</span><span class="sxs-lookup"><span data-stu-id="c33d5-145">action</span></span>|[<span data-ttu-id="c33d5-146">ремотеактион</span><span class="sxs-lookup"><span data-stu-id="c33d5-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="c33d5-147">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="c33d5-147">The action name.</span></span> <span data-ttu-id="c33d5-148">Возможные `unknown`значения:, `factoryReset`, `removeCompanyData`, `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName`,,,,,,, `quickScan`,,,,,,,,,,,,,,,,,,. `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser`</span><span class="sxs-lookup"><span data-stu-id="c33d5-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="c33d5-149">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="c33d5-149">requestDateTime</span></span>|<span data-ttu-id="c33d5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c33d5-150">DateTimeOffset</span></span>|<span data-ttu-id="c33d5-151">Время, когда действие было выдано, заданное в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c33d5-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="c33d5-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c33d5-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="c33d5-153">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-153">String</span></span>|<span data-ttu-id="c33d5-154">Имя участника-пользователя для владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="c33d5-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="c33d5-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="c33d5-155">deviceIMEI</span></span>|<span data-ttu-id="c33d5-156">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-156">String</span></span>|<span data-ttu-id="c33d5-157">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="c33d5-157">IMEI of the device.</span></span>|
|<span data-ttu-id="c33d5-158">actionState</span><span class="sxs-lookup"><span data-stu-id="c33d5-158">actionState</span></span>|[<span data-ttu-id="c33d5-159">actionState</span><span class="sxs-lookup"><span data-stu-id="c33d5-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c33d5-160">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="c33d5-160">Action state.</span></span> <span data-ttu-id="c33d5-161">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c33d5-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c33d5-162">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="c33d5-162">managedDeviceId</span></span>|<span data-ttu-id="c33d5-163">String</span><span class="sxs-lookup"><span data-stu-id="c33d5-163">String</span></span>|<span data-ttu-id="c33d5-164">Цель действия.</span><span class="sxs-lookup"><span data-stu-id="c33d5-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="c33d5-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="c33d5-165">Response</span></span>
<span data-ttu-id="c33d5-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c33d5-166">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c33d5-167">Пример</span><span class="sxs-lookup"><span data-stu-id="c33d5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="c33d5-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="c33d5-168">Request</span></span>
<span data-ttu-id="c33d5-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c33d5-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 504

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="c33d5-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="c33d5-170">Response</span></span>
<span data-ttu-id="c33d5-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c33d5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "factoryReset",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "pending",
  "managedDeviceId": "Managed Device Id value"
}
```



