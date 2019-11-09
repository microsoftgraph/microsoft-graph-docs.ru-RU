---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9bf0ca680a245ece0d3731edb64539186b4c3dae
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/09/2019
ms.locfileid: "38087231"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="1b49b-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="1b49b-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="1b49b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b49b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b49b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1b49b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b49b-106">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="1b49b-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b49b-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1b49b-107">Prerequisites</span></span>
<span data-ttu-id="1b49b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b49b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b49b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b49b-110">Permission type</span></span>|<span data-ttu-id="1b49b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b49b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b49b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b49b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b49b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b49b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1b49b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b49b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b49b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b49b-115">Not supported.</span></span>|
|<span data-ttu-id="1b49b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b49b-116">Application</span></span>|<span data-ttu-id="1b49b-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b49b-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b49b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b49b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="1b49b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1b49b-119">Request headers</span></span>
|<span data-ttu-id="1b49b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1b49b-120">Header</span></span>|<span data-ttu-id="1b49b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1b49b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b49b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b49b-122">Authorization</span></span>|<span data-ttu-id="1b49b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1b49b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b49b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1b49b-124">Accept</span></span>|<span data-ttu-id="1b49b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b49b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b49b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b49b-126">Request body</span></span>
<span data-ttu-id="1b49b-127">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b49b-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="1b49b-128">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="1b49b-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="1b49b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b49b-129">Property</span></span>|<span data-ttu-id="1b49b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b49b-130">Type</span></span>|<span data-ttu-id="1b49b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b49b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b49b-132">id</span><span class="sxs-lookup"><span data-stu-id="1b49b-132">id</span></span>|<span data-ttu-id="1b49b-133">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-133">String</span></span>|<span data-ttu-id="1b49b-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="1b49b-134">The GUID for the object</span></span>|
|<span data-ttu-id="1b49b-135">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="1b49b-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="1b49b-136">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="1b49b-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="1b49b-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="1b49b-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="1b49b-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="1b49b-139">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="1b49b-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="1b49b-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="1b49b-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="1b49b-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="1b49b-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="1b49b-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="1b49b-143">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="1b49b-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="1b49b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b49b-144">DateTimeOffset</span></span>|<span data-ttu-id="1b49b-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b49b-146">orderIdentifier</span></span>|<span data-ttu-id="1b49b-147">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-147">String</span></span>|<span data-ttu-id="1b49b-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="1b49b-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="1b49b-149">грауптаг</span><span class="sxs-lookup"><span data-stu-id="1b49b-149">groupTag</span></span>|<span data-ttu-id="1b49b-150">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-150">String</span></span>|<span data-ttu-id="1b49b-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-152">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="1b49b-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="1b49b-153">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-153">String</span></span>|<span data-ttu-id="1b49b-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1b49b-155">serialNumber</span></span>|<span data-ttu-id="1b49b-156">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-156">String</span></span>|<span data-ttu-id="1b49b-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="1b49b-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-158">productKey</span><span class="sxs-lookup"><span data-stu-id="1b49b-158">productKey</span></span>|<span data-ttu-id="1b49b-159">Строка</span><span class="sxs-lookup"><span data-stu-id="1b49b-159">String</span></span>|<span data-ttu-id="1b49b-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="1b49b-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1b49b-161">manufacturer</span></span>|<span data-ttu-id="1b49b-162">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-162">String</span></span>|<span data-ttu-id="1b49b-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-164">model</span><span class="sxs-lookup"><span data-stu-id="1b49b-164">model</span></span>|<span data-ttu-id="1b49b-165">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-165">String</span></span>|<span data-ttu-id="1b49b-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-167">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1b49b-167">enrollmentState</span></span>|[<span data-ttu-id="1b49b-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="1b49b-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="1b49b-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="1b49b-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="1b49b-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="1b49b-171">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="1b49b-171">lastContactedDateTime</span></span>|<span data-ttu-id="1b49b-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b49b-172">DateTimeOffset</span></span>|<span data-ttu-id="1b49b-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="1b49b-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="1b49b-174">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="1b49b-174">addressableUserName</span></span>|<span data-ttu-id="1b49b-175">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-175">String</span></span>|<span data-ttu-id="1b49b-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="1b49b-176">Addressable user name.</span></span>|
|<span data-ttu-id="1b49b-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b49b-177">userPrincipalName</span></span>|<span data-ttu-id="1b49b-178">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-178">String</span></span>|<span data-ttu-id="1b49b-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b49b-179">User Principal Name.</span></span>|
|<span data-ttu-id="1b49b-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="1b49b-180">resourceName</span></span>|<span data-ttu-id="1b49b-181">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-181">String</span></span>|<span data-ttu-id="1b49b-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="1b49b-182">Resource Name.</span></span>|
|<span data-ttu-id="1b49b-183">скунумбер</span><span class="sxs-lookup"><span data-stu-id="1b49b-183">skuNumber</span></span>|<span data-ttu-id="1b49b-184">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-184">String</span></span>|<span data-ttu-id="1b49b-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="1b49b-185">SKU Number</span></span>|
|<span data-ttu-id="1b49b-186">системфамили</span><span class="sxs-lookup"><span data-stu-id="1b49b-186">systemFamily</span></span>|<span data-ttu-id="1b49b-187">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-187">String</span></span>|<span data-ttu-id="1b49b-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="1b49b-188">System Family</span></span>|
|<span data-ttu-id="1b49b-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="1b49b-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="1b49b-190">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-190">String</span></span>|<span data-ttu-id="1b49b-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="1b49b-191">AAD Device ID</span></span>|
|<span data-ttu-id="1b49b-192">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="1b49b-192">managedDeviceId</span></span>|<span data-ttu-id="1b49b-193">String</span><span class="sxs-lookup"><span data-stu-id="1b49b-193">String</span></span>|<span data-ttu-id="1b49b-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="1b49b-194">Managed Device ID</span></span>|
|<span data-ttu-id="1b49b-195">displayName</span><span class="sxs-lookup"><span data-stu-id="1b49b-195">displayName</span></span>|<span data-ttu-id="1b49b-196">Строка</span><span class="sxs-lookup"><span data-stu-id="1b49b-196">String</span></span>|<span data-ttu-id="1b49b-197">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="1b49b-197">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="1b49b-198">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b49b-198">Response</span></span>
<span data-ttu-id="1b49b-199">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b49b-199">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b49b-200">Пример</span><span class="sxs-lookup"><span data-stu-id="1b49b-200">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b49b-201">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b49b-201">Request</span></span>
<span data-ttu-id="1b49b-202">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b49b-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="1b49b-203">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b49b-203">Response</span></span>
<span data-ttu-id="1b49b-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b49b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






