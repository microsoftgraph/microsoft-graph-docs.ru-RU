---
title: Обновление remoteActionAudit
description: Обновление свойств объекта remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d75694a242619e548c1bda775e8798f67b09b30d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158180"
---
# <a name="update-remoteactionaudit"></a><span data-ttu-id="97a57-103">Обновление remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="97a57-103">Update remoteActionAudit</span></span>

<span data-ttu-id="97a57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97a57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97a57-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97a57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="97a57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97a57-107">Обновление свойств объекта [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="97a57-107">Update the properties of a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97a57-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="97a57-108">Prerequisites</span></span>
<span data-ttu-id="97a57-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97a57-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="97a57-111">Permission type</span></span>|<span data-ttu-id="97a57-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="97a57-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97a57-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="97a57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="97a57-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97a57-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="97a57-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="97a57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97a57-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="97a57-116">Not supported.</span></span>|
|<span data-ttu-id="97a57-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="97a57-117">Application</span></span>|<span data-ttu-id="97a57-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97a57-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97a57-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="97a57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## <a name="request-headers"></a><span data-ttu-id="97a57-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="97a57-120">Request headers</span></span>
|<span data-ttu-id="97a57-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="97a57-121">Header</span></span>|<span data-ttu-id="97a57-122">Значение</span><span class="sxs-lookup"><span data-stu-id="97a57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97a57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="97a57-123">Authorization</span></span>|<span data-ttu-id="97a57-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="97a57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97a57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="97a57-125">Accept</span></span>|<span data-ttu-id="97a57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="97a57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97a57-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="97a57-127">Request body</span></span>
<span data-ttu-id="97a57-128">В теле запроса поставляем представление JSON для [объекта remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="97a57-128">In the request body, supply a JSON representation for the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

<span data-ttu-id="97a57-129">В следующей таблице показаны свойства, необходимые при создании [remoteActionAudit.](../resources/intune-devices-remoteactionaudit.md)</span><span class="sxs-lookup"><span data-stu-id="97a57-129">The following table shows the properties that are required when you create the [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md).</span></span>

|<span data-ttu-id="97a57-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="97a57-130">Property</span></span>|<span data-ttu-id="97a57-131">Тип</span><span class="sxs-lookup"><span data-stu-id="97a57-131">Type</span></span>|<span data-ttu-id="97a57-132">Описание</span><span class="sxs-lookup"><span data-stu-id="97a57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97a57-133">id</span><span class="sxs-lookup"><span data-stu-id="97a57-133">id</span></span>|<span data-ttu-id="97a57-134">Строка</span><span class="sxs-lookup"><span data-stu-id="97a57-134">String</span></span>|<span data-ttu-id="97a57-135">Report Id.</span><span class="sxs-lookup"><span data-stu-id="97a57-135">Report Id.</span></span>|
|<span data-ttu-id="97a57-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="97a57-136">deviceDisplayName</span></span>|<span data-ttu-id="97a57-137">String</span><span class="sxs-lookup"><span data-stu-id="97a57-137">String</span></span>|<span data-ttu-id="97a57-138">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="97a57-138">Intune device name.</span></span>|
|<span data-ttu-id="97a57-139">userName</span><span class="sxs-lookup"><span data-stu-id="97a57-139">userName</span></span>|<span data-ttu-id="97a57-140">String</span><span class="sxs-lookup"><span data-stu-id="97a57-140">String</span></span>|<span data-ttu-id="97a57-141">\[deprecated \] Please use InitiatedByUserPrincipalName instead.</span><span class="sxs-lookup"><span data-stu-id="97a57-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="97a57-142">initiatedByUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97a57-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="97a57-143">Строка</span><span class="sxs-lookup"><span data-stu-id="97a57-143">String</span></span>|<span data-ttu-id="97a57-144">Пользователь, который инициировал действие устройства, формат upN.</span><span class="sxs-lookup"><span data-stu-id="97a57-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="97a57-145">action</span><span class="sxs-lookup"><span data-stu-id="97a57-145">action</span></span>|[<span data-ttu-id="97a57-146">remoteAction</span><span class="sxs-lookup"><span data-stu-id="97a57-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="97a57-147">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="97a57-147">The action name.</span></span> <span data-ttu-id="97a57-148">Возможные значения: `unknown` `factoryReset` , , `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` , `quickScan` `fullScan` `windowsDefenderUpdateSignatures` `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` .</span><span class="sxs-lookup"><span data-stu-id="97a57-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="97a57-149">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="97a57-149">requestDateTime</span></span>|<span data-ttu-id="97a57-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97a57-150">DateTimeOffset</span></span>|<span data-ttu-id="97a57-151">Время, когда действие было выдано, дано в UTC.</span><span class="sxs-lookup"><span data-stu-id="97a57-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="97a57-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="97a57-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="97a57-153">Строка</span><span class="sxs-lookup"><span data-stu-id="97a57-153">String</span></span>|<span data-ttu-id="97a57-154">Upn владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="97a57-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="97a57-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="97a57-155">deviceIMEI</span></span>|<span data-ttu-id="97a57-156">Строка</span><span class="sxs-lookup"><span data-stu-id="97a57-156">String</span></span>|<span data-ttu-id="97a57-157">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="97a57-157">IMEI of the device.</span></span>|
|<span data-ttu-id="97a57-158">actionState</span><span class="sxs-lookup"><span data-stu-id="97a57-158">actionState</span></span>|[<span data-ttu-id="97a57-159">actionState</span><span class="sxs-lookup"><span data-stu-id="97a57-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="97a57-160">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="97a57-160">Action state.</span></span> <span data-ttu-id="97a57-161">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="97a57-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="97a57-162">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="97a57-162">managedDeviceId</span></span>|<span data-ttu-id="97a57-163">Строка</span><span class="sxs-lookup"><span data-stu-id="97a57-163">String</span></span>|<span data-ttu-id="97a57-164">Цель действия.</span><span class="sxs-lookup"><span data-stu-id="97a57-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="97a57-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a57-165">Response</span></span>
<span data-ttu-id="97a57-166">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="97a57-166">If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97a57-167">Пример</span><span class="sxs-lookup"><span data-stu-id="97a57-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="97a57-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="97a57-168">Request</span></span>
<span data-ttu-id="97a57-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="97a57-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="97a57-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="97a57-170">Response</span></span>
<span data-ttu-id="97a57-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="97a57-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




