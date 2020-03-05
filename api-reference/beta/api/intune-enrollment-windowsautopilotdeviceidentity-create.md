---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 842eb424926a5673ca33b768c7bd999245dca8bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42466320"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="133cc-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="133cc-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="133cc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="133cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="133cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="133cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="133cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="133cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="133cc-107">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="133cc-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="133cc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="133cc-108">Prerequisites</span></span>
<span data-ttu-id="133cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="133cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="133cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="133cc-111">Permission type</span></span>|<span data-ttu-id="133cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="133cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="133cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="133cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="133cc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="133cc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="133cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="133cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="133cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="133cc-116">Not supported.</span></span>|
|<span data-ttu-id="133cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="133cc-117">Application</span></span>|<span data-ttu-id="133cc-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="133cc-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="133cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="133cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="133cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="133cc-120">Request headers</span></span>
|<span data-ttu-id="133cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="133cc-121">Header</span></span>|<span data-ttu-id="133cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="133cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="133cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="133cc-123">Authorization</span></span>|<span data-ttu-id="133cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="133cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="133cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="133cc-125">Accept</span></span>|<span data-ttu-id="133cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="133cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="133cc-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="133cc-127">Request body</span></span>
<span data-ttu-id="133cc-128">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="133cc-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="133cc-129">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="133cc-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="133cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="133cc-130">Property</span></span>|<span data-ttu-id="133cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="133cc-131">Type</span></span>|<span data-ttu-id="133cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="133cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="133cc-133">id</span><span class="sxs-lookup"><span data-stu-id="133cc-133">id</span></span>|<span data-ttu-id="133cc-134">String</span><span class="sxs-lookup"><span data-stu-id="133cc-134">String</span></span>|<span data-ttu-id="133cc-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="133cc-135">The GUID for the object</span></span>|
|<span data-ttu-id="133cc-136">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="133cc-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="133cc-137">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="133cc-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="133cc-138">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="133cc-139">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="133cc-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="133cc-140">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="133cc-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="133cc-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="133cc-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="133cc-142">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="133cc-143">Возможные значения: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="133cc-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="133cc-144">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="133cc-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="133cc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133cc-145">DateTimeOffset</span></span>|<span data-ttu-id="133cc-146">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="133cc-147">orderIdentifier</span></span>|<span data-ttu-id="133cc-148">String</span><span class="sxs-lookup"><span data-stu-id="133cc-148">String</span></span>|<span data-ttu-id="133cc-149">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="133cc-149">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="133cc-150">грауптаг</span><span class="sxs-lookup"><span data-stu-id="133cc-150">groupTag</span></span>|<span data-ttu-id="133cc-151">String</span><span class="sxs-lookup"><span data-stu-id="133cc-151">String</span></span>|<span data-ttu-id="133cc-152">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-152">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-153">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="133cc-153">purchaseOrderIdentifier</span></span>|<span data-ttu-id="133cc-154">String</span><span class="sxs-lookup"><span data-stu-id="133cc-154">String</span></span>|<span data-ttu-id="133cc-155">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-155">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-156">serialNumber</span><span class="sxs-lookup"><span data-stu-id="133cc-156">serialNumber</span></span>|<span data-ttu-id="133cc-157">String</span><span class="sxs-lookup"><span data-stu-id="133cc-157">String</span></span>|<span data-ttu-id="133cc-158">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="133cc-158">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-159">productKey</span><span class="sxs-lookup"><span data-stu-id="133cc-159">productKey</span></span>|<span data-ttu-id="133cc-160">Строка</span><span class="sxs-lookup"><span data-stu-id="133cc-160">String</span></span>|<span data-ttu-id="133cc-161">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="133cc-161">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-162">manufacturer</span><span class="sxs-lookup"><span data-stu-id="133cc-162">manufacturer</span></span>|<span data-ttu-id="133cc-163">String</span><span class="sxs-lookup"><span data-stu-id="133cc-163">String</span></span>|<span data-ttu-id="133cc-164">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-164">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-165">model</span><span class="sxs-lookup"><span data-stu-id="133cc-165">model</span></span>|<span data-ttu-id="133cc-166">String</span><span class="sxs-lookup"><span data-stu-id="133cc-166">String</span></span>|<span data-ttu-id="133cc-167">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-167">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="133cc-168">enrollmentState</span></span>|[<span data-ttu-id="133cc-169">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="133cc-169">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="133cc-170">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-170">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="133cc-171">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="133cc-171">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="133cc-172">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="133cc-172">lastContactedDateTime</span></span>|<span data-ttu-id="133cc-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="133cc-173">DateTimeOffset</span></span>|<span data-ttu-id="133cc-174">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="133cc-174">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="133cc-175">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="133cc-175">addressableUserName</span></span>|<span data-ttu-id="133cc-176">String</span><span class="sxs-lookup"><span data-stu-id="133cc-176">String</span></span>|<span data-ttu-id="133cc-177">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="133cc-177">Addressable user name.</span></span>|
|<span data-ttu-id="133cc-178">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="133cc-178">userPrincipalName</span></span>|<span data-ttu-id="133cc-179">String</span><span class="sxs-lookup"><span data-stu-id="133cc-179">String</span></span>|<span data-ttu-id="133cc-180">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="133cc-180">User Principal Name.</span></span>|
|<span data-ttu-id="133cc-181">resourceName</span><span class="sxs-lookup"><span data-stu-id="133cc-181">resourceName</span></span>|<span data-ttu-id="133cc-182">String</span><span class="sxs-lookup"><span data-stu-id="133cc-182">String</span></span>|<span data-ttu-id="133cc-183">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="133cc-183">Resource Name.</span></span>|
|<span data-ttu-id="133cc-184">скунумбер</span><span class="sxs-lookup"><span data-stu-id="133cc-184">skuNumber</span></span>|<span data-ttu-id="133cc-185">String</span><span class="sxs-lookup"><span data-stu-id="133cc-185">String</span></span>|<span data-ttu-id="133cc-186">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="133cc-186">SKU Number</span></span>|
|<span data-ttu-id="133cc-187">системфамили</span><span class="sxs-lookup"><span data-stu-id="133cc-187">systemFamily</span></span>|<span data-ttu-id="133cc-188">String</span><span class="sxs-lookup"><span data-stu-id="133cc-188">String</span></span>|<span data-ttu-id="133cc-189">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="133cc-189">System Family</span></span>|
|<span data-ttu-id="133cc-190">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="133cc-190">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="133cc-191">String</span><span class="sxs-lookup"><span data-stu-id="133cc-191">String</span></span>|<span data-ttu-id="133cc-192">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="133cc-192">AAD Device ID</span></span>|
|<span data-ttu-id="133cc-193">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="133cc-193">managedDeviceId</span></span>|<span data-ttu-id="133cc-194">String</span><span class="sxs-lookup"><span data-stu-id="133cc-194">String</span></span>|<span data-ttu-id="133cc-195">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="133cc-195">Managed Device ID</span></span>|
|<span data-ttu-id="133cc-196">displayName</span><span class="sxs-lookup"><span data-stu-id="133cc-196">displayName</span></span>|<span data-ttu-id="133cc-197">Строка</span><span class="sxs-lookup"><span data-stu-id="133cc-197">String</span></span>|<span data-ttu-id="133cc-198">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="133cc-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="133cc-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="133cc-199">Response</span></span>
<span data-ttu-id="133cc-200">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="133cc-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="133cc-201">Пример</span><span class="sxs-lookup"><span data-stu-id="133cc-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="133cc-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="133cc-202">Request</span></span>
<span data-ttu-id="133cc-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="133cc-203">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="133cc-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="133cc-204">Response</span></span>
<span data-ttu-id="133cc-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="133cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





