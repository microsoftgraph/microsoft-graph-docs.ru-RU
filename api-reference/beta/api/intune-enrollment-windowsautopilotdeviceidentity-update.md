---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойств объекта windowsAutopilotDeviceIdentity.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4d54568b2d45a4742f4dd36be5fdd700e7ea16f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42804991"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="8f853-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8f853-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="8f853-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f853-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f853-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8f853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f853-106">Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="8f853-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f853-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8f853-107">Prerequisites</span></span>
<span data-ttu-id="8f853-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8f853-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f853-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8f853-110">Permission type</span></span>|<span data-ttu-id="8f853-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8f853-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f853-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8f853-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f853-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f853-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8f853-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8f853-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f853-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8f853-115">Not supported.</span></span>|
|<span data-ttu-id="8f853-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8f853-116">Application</span></span>|<span data-ttu-id="8f853-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f853-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f853-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8f853-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="8f853-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8f853-119">Request headers</span></span>
|<span data-ttu-id="8f853-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8f853-120">Header</span></span>|<span data-ttu-id="8f853-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8f853-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f853-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f853-122">Authorization</span></span>|<span data-ttu-id="8f853-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8f853-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f853-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8f853-124">Accept</span></span>|<span data-ttu-id="8f853-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f853-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f853-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8f853-126">Request body</span></span>
<span data-ttu-id="8f853-127">В тексте запроса добавьте представление объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f853-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="8f853-128">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="8f853-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="8f853-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f853-129">Property</span></span>|<span data-ttu-id="8f853-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8f853-130">Type</span></span>|<span data-ttu-id="8f853-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8f853-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f853-132">id</span><span class="sxs-lookup"><span data-stu-id="8f853-132">id</span></span>|<span data-ttu-id="8f853-133">String</span><span class="sxs-lookup"><span data-stu-id="8f853-133">String</span></span>|<span data-ttu-id="8f853-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="8f853-134">The GUID for the object</span></span>|
|<span data-ttu-id="8f853-135">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="8f853-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="8f853-136">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="8f853-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="8f853-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="8f853-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8f853-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="8f853-139">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="8f853-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="8f853-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="8f853-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="8f853-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="8f853-142">Возможные значения: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="8f853-142">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="8f853-143">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8f853-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="8f853-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f853-144">DateTimeOffset</span></span>|<span data-ttu-id="8f853-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="8f853-146">orderIdentifier</span></span>|<span data-ttu-id="8f853-147">String</span><span class="sxs-lookup"><span data-stu-id="8f853-147">String</span></span>|<span data-ttu-id="8f853-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="8f853-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="8f853-149">грауптаг</span><span class="sxs-lookup"><span data-stu-id="8f853-149">groupTag</span></span>|<span data-ttu-id="8f853-150">String</span><span class="sxs-lookup"><span data-stu-id="8f853-150">String</span></span>|<span data-ttu-id="8f853-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-152">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="8f853-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="8f853-153">String</span><span class="sxs-lookup"><span data-stu-id="8f853-153">String</span></span>|<span data-ttu-id="8f853-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="8f853-155">serialNumber</span></span>|<span data-ttu-id="8f853-156">String</span><span class="sxs-lookup"><span data-stu-id="8f853-156">String</span></span>|<span data-ttu-id="8f853-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="8f853-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-158">productKey</span><span class="sxs-lookup"><span data-stu-id="8f853-158">productKey</span></span>|<span data-ttu-id="8f853-159">Строка</span><span class="sxs-lookup"><span data-stu-id="8f853-159">String</span></span>|<span data-ttu-id="8f853-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="8f853-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="8f853-161">manufacturer</span></span>|<span data-ttu-id="8f853-162">String</span><span class="sxs-lookup"><span data-stu-id="8f853-162">String</span></span>|<span data-ttu-id="8f853-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-164">model</span><span class="sxs-lookup"><span data-stu-id="8f853-164">model</span></span>|<span data-ttu-id="8f853-165">String</span><span class="sxs-lookup"><span data-stu-id="8f853-165">String</span></span>|<span data-ttu-id="8f853-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-167">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="8f853-167">enrollmentState</span></span>|[<span data-ttu-id="8f853-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="8f853-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="8f853-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="8f853-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="8f853-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="8f853-171">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="8f853-171">lastContactedDateTime</span></span>|<span data-ttu-id="8f853-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f853-172">DateTimeOffset</span></span>|<span data-ttu-id="8f853-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="8f853-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="8f853-174">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="8f853-174">addressableUserName</span></span>|<span data-ttu-id="8f853-175">String</span><span class="sxs-lookup"><span data-stu-id="8f853-175">String</span></span>|<span data-ttu-id="8f853-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="8f853-176">Addressable user name.</span></span>|
|<span data-ttu-id="8f853-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f853-177">userPrincipalName</span></span>|<span data-ttu-id="8f853-178">String</span><span class="sxs-lookup"><span data-stu-id="8f853-178">String</span></span>|<span data-ttu-id="8f853-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f853-179">User Principal Name.</span></span>|
|<span data-ttu-id="8f853-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="8f853-180">resourceName</span></span>|<span data-ttu-id="8f853-181">String</span><span class="sxs-lookup"><span data-stu-id="8f853-181">String</span></span>|<span data-ttu-id="8f853-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="8f853-182">Resource Name.</span></span>|
|<span data-ttu-id="8f853-183">скунумбер</span><span class="sxs-lookup"><span data-stu-id="8f853-183">skuNumber</span></span>|<span data-ttu-id="8f853-184">String</span><span class="sxs-lookup"><span data-stu-id="8f853-184">String</span></span>|<span data-ttu-id="8f853-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="8f853-185">SKU Number</span></span>|
|<span data-ttu-id="8f853-186">системфамили</span><span class="sxs-lookup"><span data-stu-id="8f853-186">systemFamily</span></span>|<span data-ttu-id="8f853-187">String</span><span class="sxs-lookup"><span data-stu-id="8f853-187">String</span></span>|<span data-ttu-id="8f853-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="8f853-188">System Family</span></span>|
|<span data-ttu-id="8f853-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="8f853-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="8f853-190">String</span><span class="sxs-lookup"><span data-stu-id="8f853-190">String</span></span>|<span data-ttu-id="8f853-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="8f853-191">AAD Device ID</span></span>|
|<span data-ttu-id="8f853-192">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="8f853-192">managedDeviceId</span></span>|<span data-ttu-id="8f853-193">String</span><span class="sxs-lookup"><span data-stu-id="8f853-193">String</span></span>|<span data-ttu-id="8f853-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="8f853-194">Managed Device ID</span></span>|
|<span data-ttu-id="8f853-195">displayName</span><span class="sxs-lookup"><span data-stu-id="8f853-195">displayName</span></span>|<span data-ttu-id="8f853-196">Строка</span><span class="sxs-lookup"><span data-stu-id="8f853-196">String</span></span>|<span data-ttu-id="8f853-197">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="8f853-197">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="8f853-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f853-198">Response</span></span>
<span data-ttu-id="8f853-199">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8f853-199">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f853-200">Пример</span><span class="sxs-lookup"><span data-stu-id="8f853-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f853-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="8f853-201">Request</span></span>
<span data-ttu-id="8f853-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8f853-202">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8f853-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="8f853-203">Response</span></span>
<span data-ttu-id="8f853-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8f853-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




