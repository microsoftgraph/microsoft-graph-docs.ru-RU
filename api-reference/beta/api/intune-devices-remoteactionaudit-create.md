---
title: Создание remoteActionAudit
description: Создание нового объекта remoteActionAudit.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4195b2d244295d670df64dfaa851bc744509fdd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234526"
---
# <a name="create-remoteactionaudit"></a><span data-ttu-id="004ed-103">Создание remoteActionAudit</span><span class="sxs-lookup"><span data-stu-id="004ed-103">Create remoteActionAudit</span></span>

<span data-ttu-id="004ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="004ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="004ed-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="004ed-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="004ed-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="004ed-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="004ed-107">Создание нового объекта [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) .</span><span class="sxs-lookup"><span data-stu-id="004ed-107">Create a new [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="004ed-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="004ed-108">Prerequisites</span></span>
<span data-ttu-id="004ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="004ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="004ed-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="004ed-111">Permission type</span></span>|<span data-ttu-id="004ed-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="004ed-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="004ed-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="004ed-113">Delegated (work or school account)</span></span>|<span data-ttu-id="004ed-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004ed-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="004ed-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="004ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="004ed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="004ed-116">Not supported.</span></span>|
|<span data-ttu-id="004ed-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="004ed-117">Application</span></span>|<span data-ttu-id="004ed-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="004ed-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="004ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="004ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteActionAudits
```

## <a name="request-headers"></a><span data-ttu-id="004ed-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="004ed-120">Request headers</span></span>
|<span data-ttu-id="004ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="004ed-121">Header</span></span>|<span data-ttu-id="004ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="004ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="004ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="004ed-123">Authorization</span></span>|<span data-ttu-id="004ed-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="004ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="004ed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="004ed-125">Accept</span></span>|<span data-ttu-id="004ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="004ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="004ed-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="004ed-127">Request body</span></span>
<span data-ttu-id="004ed-128">В тексте запроса добавьте представление объекта remoteActionAudit в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="004ed-128">In the request body, supply a JSON representation for the remoteActionAudit object.</span></span>

<span data-ttu-id="004ed-129">В следующей таблице приведены свойства, необходимые при создании remoteActionAudit.</span><span class="sxs-lookup"><span data-stu-id="004ed-129">The following table shows the properties that are required when you create the remoteActionAudit.</span></span>

|<span data-ttu-id="004ed-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="004ed-130">Property</span></span>|<span data-ttu-id="004ed-131">Тип</span><span class="sxs-lookup"><span data-stu-id="004ed-131">Type</span></span>|<span data-ttu-id="004ed-132">Описание</span><span class="sxs-lookup"><span data-stu-id="004ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="004ed-133">id</span><span class="sxs-lookup"><span data-stu-id="004ed-133">id</span></span>|<span data-ttu-id="004ed-134">String</span><span class="sxs-lookup"><span data-stu-id="004ed-134">String</span></span>|<span data-ttu-id="004ed-135">Идентификатор отчета.</span><span class="sxs-lookup"><span data-stu-id="004ed-135">Report Id.</span></span>|
|<span data-ttu-id="004ed-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="004ed-136">deviceDisplayName</span></span>|<span data-ttu-id="004ed-137">String</span><span class="sxs-lookup"><span data-stu-id="004ed-137">String</span></span>|<span data-ttu-id="004ed-138">Имя устройства Intune.</span><span class="sxs-lookup"><span data-stu-id="004ed-138">Intune device name.</span></span>|
|<span data-ttu-id="004ed-139">userName</span><span class="sxs-lookup"><span data-stu-id="004ed-139">userName</span></span>|<span data-ttu-id="004ed-140">String</span><span class="sxs-lookup"><span data-stu-id="004ed-140">String</span></span>|<span data-ttu-id="004ed-141">\[рекомендуется \] вместо этого использовать свойства initiatedbyuserprincipalname.</span><span class="sxs-lookup"><span data-stu-id="004ed-141">\[deprecated\] Please use InitiatedByUserPrincipalName instead.</span></span>|
|<span data-ttu-id="004ed-142">Свойства initiatedbyuserprincipalname</span><span class="sxs-lookup"><span data-stu-id="004ed-142">initiatedByUserPrincipalName</span></span>|<span data-ttu-id="004ed-143">String</span><span class="sxs-lookup"><span data-stu-id="004ed-143">String</span></span>|<span data-ttu-id="004ed-144">Пользователь, который инициировал действие с устройством, имеет формат UPN.</span><span class="sxs-lookup"><span data-stu-id="004ed-144">User who initiated the device action, format is UPN.</span></span>|
|<span data-ttu-id="004ed-145">action</span><span class="sxs-lookup"><span data-stu-id="004ed-145">action</span></span>|[<span data-ttu-id="004ed-146">ремотеактион</span><span class="sxs-lookup"><span data-stu-id="004ed-146">remoteAction</span></span>](../resources/intune-devices-remoteaction.md)|<span data-ttu-id="004ed-147">Имя действия.</span><span class="sxs-lookup"><span data-stu-id="004ed-147">The action name.</span></span> <span data-ttu-id="004ed-148">Возможные значения:,,,,,,,,,,, `unknown` `factoryReset` `removeCompanyData` `resetPasscode` `remoteLock` `enableLostMode` `disableLostMode` `locateDevice` `rebootNow` `recoverPasscode` `cleanWindowsDevice` `logoutSharedAppleDeviceActiveUser` `quickScan` , `fullScan` , `windowsDefenderUpdateSignatures` , `factoryResetKeepEnrollmentData` `updateDeviceAccount` `automaticRedeployment` `shutDown` `rotateBitLockerKeys` `rotateFileVaultKey` `getFileVaultKey` `setDeviceName` ,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="004ed-148">Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.</span></span>|
|<span data-ttu-id="004ed-149">рекуестдатетиме</span><span class="sxs-lookup"><span data-stu-id="004ed-149">requestDateTime</span></span>|<span data-ttu-id="004ed-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="004ed-150">DateTimeOffset</span></span>|<span data-ttu-id="004ed-151">Время, когда действие было выдано, заданное в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="004ed-151">Time when the action was issued, given in UTC.</span></span>|
|<span data-ttu-id="004ed-152">deviceOwnerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="004ed-152">deviceOwnerUserPrincipalName</span></span>|<span data-ttu-id="004ed-153">String</span><span class="sxs-lookup"><span data-stu-id="004ed-153">String</span></span>|<span data-ttu-id="004ed-154">Имя участника-пользователя для владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="004ed-154">Upn of the device owner.</span></span>|
|<span data-ttu-id="004ed-155">deviceIMEI</span><span class="sxs-lookup"><span data-stu-id="004ed-155">deviceIMEI</span></span>|<span data-ttu-id="004ed-156">String</span><span class="sxs-lookup"><span data-stu-id="004ed-156">String</span></span>|<span data-ttu-id="004ed-157">IMEI устройства.</span><span class="sxs-lookup"><span data-stu-id="004ed-157">IMEI of the device.</span></span>|
|<span data-ttu-id="004ed-158">actionState</span><span class="sxs-lookup"><span data-stu-id="004ed-158">actionState</span></span>|[<span data-ttu-id="004ed-159">actionState</span><span class="sxs-lookup"><span data-stu-id="004ed-159">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="004ed-160">Состояние действия.</span><span class="sxs-lookup"><span data-stu-id="004ed-160">Action state.</span></span> <span data-ttu-id="004ed-161">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="004ed-161">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="004ed-162">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="004ed-162">managedDeviceId</span></span>|<span data-ttu-id="004ed-163">String</span><span class="sxs-lookup"><span data-stu-id="004ed-163">String</span></span>|<span data-ttu-id="004ed-164">Цель действия.</span><span class="sxs-lookup"><span data-stu-id="004ed-164">Action target.</span></span>|



## <a name="response"></a><span data-ttu-id="004ed-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="004ed-165">Response</span></span>
<span data-ttu-id="004ed-166">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="004ed-166">If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/intune-devices-remoteactionaudit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="004ed-167">Пример</span><span class="sxs-lookup"><span data-stu-id="004ed-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="004ed-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="004ed-168">Request</span></span>
<span data-ttu-id="004ed-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="004ed-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
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

### <a name="response"></a><span data-ttu-id="004ed-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="004ed-170">Response</span></span>
<span data-ttu-id="004ed-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="004ed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




