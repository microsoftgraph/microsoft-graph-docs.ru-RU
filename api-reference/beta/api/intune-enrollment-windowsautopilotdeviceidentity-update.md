---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойств объекта windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d93ab57b09cec2b5de12f908b2bb4268d72b0456
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726761"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="5589b-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5589b-103">Update windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="5589b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5589b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5589b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5589b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5589b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5589b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5589b-107">Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5589b-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5589b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5589b-108">Prerequisites</span></span>
<span data-ttu-id="5589b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5589b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5589b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5589b-111">Permission type</span></span>|<span data-ttu-id="5589b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5589b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5589b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5589b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5589b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5589b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5589b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5589b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5589b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5589b-116">Not supported.</span></span>|
|<span data-ttu-id="5589b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5589b-117">Application</span></span>|<span data-ttu-id="5589b-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5589b-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5589b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5589b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="5589b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5589b-120">Request headers</span></span>
|<span data-ttu-id="5589b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5589b-121">Header</span></span>|<span data-ttu-id="5589b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5589b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5589b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5589b-123">Authorization</span></span>|<span data-ttu-id="5589b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5589b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5589b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5589b-125">Accept</span></span>|<span data-ttu-id="5589b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5589b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5589b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5589b-127">Request body</span></span>
<span data-ttu-id="5589b-128">В тексте запроса добавьте представление объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5589b-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="5589b-129">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5589b-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="5589b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5589b-130">Property</span></span>|<span data-ttu-id="5589b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5589b-131">Type</span></span>|<span data-ttu-id="5589b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5589b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5589b-133">id</span><span class="sxs-lookup"><span data-stu-id="5589b-133">id</span></span>|<span data-ttu-id="5589b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-134">String</span></span>|<span data-ttu-id="5589b-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="5589b-135">The GUID for the object</span></span>|
|<span data-ttu-id="5589b-136">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="5589b-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="5589b-137">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="5589b-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="5589b-138">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="5589b-139">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5589b-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="5589b-140">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="5589b-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="5589b-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="5589b-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="5589b-142">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="5589b-143">Возможные значения: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="5589b-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="5589b-144">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="5589b-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="5589b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5589b-145">DateTimeOffset</span></span>|<span data-ttu-id="5589b-146">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="5589b-147">orderIdentifier</span></span>|<span data-ttu-id="5589b-148">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-148">String</span></span>|<span data-ttu-id="5589b-149">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="5589b-149">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="5589b-150">грауптаг</span><span class="sxs-lookup"><span data-stu-id="5589b-150">groupTag</span></span>|<span data-ttu-id="5589b-151">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-151">String</span></span>|<span data-ttu-id="5589b-152">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-152">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-153">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="5589b-153">purchaseOrderIdentifier</span></span>|<span data-ttu-id="5589b-154">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-154">String</span></span>|<span data-ttu-id="5589b-155">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-155">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-156">serialNumber</span><span class="sxs-lookup"><span data-stu-id="5589b-156">serialNumber</span></span>|<span data-ttu-id="5589b-157">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-157">String</span></span>|<span data-ttu-id="5589b-158">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5589b-158">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-159">productKey</span><span class="sxs-lookup"><span data-stu-id="5589b-159">productKey</span></span>|<span data-ttu-id="5589b-160">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-160">String</span></span>|<span data-ttu-id="5589b-161">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5589b-161">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="5589b-162">manufacturer</span></span>|<span data-ttu-id="5589b-163">String</span><span class="sxs-lookup"><span data-stu-id="5589b-163">String</span></span>|<span data-ttu-id="5589b-164">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-164">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-165">model</span><span class="sxs-lookup"><span data-stu-id="5589b-165">model</span></span>|<span data-ttu-id="5589b-166">String</span><span class="sxs-lookup"><span data-stu-id="5589b-166">String</span></span>|<span data-ttu-id="5589b-167">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-167">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="5589b-168">enrollmentState</span></span>|[<span data-ttu-id="5589b-169">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="5589b-169">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="5589b-170">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-170">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="5589b-171">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5589b-171">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5589b-172">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="5589b-172">lastContactedDateTime</span></span>|<span data-ttu-id="5589b-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5589b-173">DateTimeOffset</span></span>|<span data-ttu-id="5589b-174">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="5589b-174">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="5589b-175">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="5589b-175">addressableUserName</span></span>|<span data-ttu-id="5589b-176">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-176">String</span></span>|<span data-ttu-id="5589b-177">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="5589b-177">Addressable user name.</span></span>|
|<span data-ttu-id="5589b-178">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5589b-178">userPrincipalName</span></span>|<span data-ttu-id="5589b-179">String</span><span class="sxs-lookup"><span data-stu-id="5589b-179">String</span></span>|<span data-ttu-id="5589b-180">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="5589b-180">User Principal Name.</span></span>|
|<span data-ttu-id="5589b-181">resourceName</span><span class="sxs-lookup"><span data-stu-id="5589b-181">resourceName</span></span>|<span data-ttu-id="5589b-182">String</span><span class="sxs-lookup"><span data-stu-id="5589b-182">String</span></span>|<span data-ttu-id="5589b-183">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="5589b-183">Resource Name.</span></span>|
|<span data-ttu-id="5589b-184">скунумбер</span><span class="sxs-lookup"><span data-stu-id="5589b-184">skuNumber</span></span>|<span data-ttu-id="5589b-185">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-185">String</span></span>|<span data-ttu-id="5589b-186">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="5589b-186">SKU Number</span></span>|
|<span data-ttu-id="5589b-187">системфамили</span><span class="sxs-lookup"><span data-stu-id="5589b-187">systemFamily</span></span>|<span data-ttu-id="5589b-188">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-188">String</span></span>|<span data-ttu-id="5589b-189">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="5589b-189">System Family</span></span>|
|<span data-ttu-id="5589b-190">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="5589b-190">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="5589b-191">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-191">String</span></span>|<span data-ttu-id="5589b-192">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="5589b-192">AAD Device ID</span></span>|
|<span data-ttu-id="5589b-193">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="5589b-193">managedDeviceId</span></span>|<span data-ttu-id="5589b-194">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-194">String</span></span>|<span data-ttu-id="5589b-195">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="5589b-195">Managed Device ID</span></span>|
|<span data-ttu-id="5589b-196">displayName</span><span class="sxs-lookup"><span data-stu-id="5589b-196">displayName</span></span>|<span data-ttu-id="5589b-197">Строка</span><span class="sxs-lookup"><span data-stu-id="5589b-197">String</span></span>|<span data-ttu-id="5589b-198">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="5589b-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="5589b-199">Ответ</span><span class="sxs-lookup"><span data-stu-id="5589b-199">Response</span></span>
<span data-ttu-id="5589b-200">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5589b-200">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5589b-201">Пример</span><span class="sxs-lookup"><span data-stu-id="5589b-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="5589b-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="5589b-202">Request</span></span>
<span data-ttu-id="5589b-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5589b-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 1075

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="5589b-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="5589b-204">Response</span></span>
<span data-ttu-id="5589b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5589b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
  "groupTag": "Group Tag value",
  "purchaseOrderIdentifier": "Purchase Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "enrollmentState": "enrolled",
  "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
  "addressableUserName": "Addressable User Name value",
  "userPrincipalName": "User Principal Name value",
  "resourceName": "Resource Name value",
  "skuNumber": "Sku Number value",
  "systemFamily": "System Family value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```





