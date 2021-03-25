---
title: Создание объекта windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 725d6d5c0cb0f03c9fcb1b2c161959a4242e2a13
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153855"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="61cf3-103">Создание объекта windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="61cf3-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="61cf3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61cf3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61cf3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61cf3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61cf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61cf3-107">Создание нового [объекта windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="61cf3-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61cf3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="61cf3-108">Prerequisites</span></span>
<span data-ttu-id="61cf3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61cf3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61cf3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61cf3-111">Permission type</span></span>|<span data-ttu-id="61cf3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61cf3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61cf3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61cf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61cf3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cf3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61cf3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61cf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61cf3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61cf3-116">Not supported.</span></span>|
|<span data-ttu-id="61cf3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="61cf3-117">Application</span></span>|<span data-ttu-id="61cf3-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61cf3-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61cf3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61cf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="61cf3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="61cf3-120">Request headers</span></span>
|<span data-ttu-id="61cf3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="61cf3-121">Header</span></span>|<span data-ttu-id="61cf3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="61cf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61cf3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61cf3-123">Authorization</span></span>|<span data-ttu-id="61cf3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61cf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61cf3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="61cf3-125">Accept</span></span>|<span data-ttu-id="61cf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61cf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61cf3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61cf3-127">Request body</span></span>
<span data-ttu-id="61cf3-128">В теле запроса поставляем представление JSON для объекта windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="61cf3-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="61cf3-129">В следующей таблице показаны свойства, необходимые при создании объекта windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="61cf3-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="61cf3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="61cf3-130">Property</span></span>|<span data-ttu-id="61cf3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="61cf3-131">Type</span></span>|<span data-ttu-id="61cf3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="61cf3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61cf3-133">id</span><span class="sxs-lookup"><span data-stu-id="61cf3-133">id</span></span>|<span data-ttu-id="61cf3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-134">String</span></span>|<span data-ttu-id="61cf3-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="61cf3-135">The GUID for the object</span></span>|
|<span data-ttu-id="61cf3-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="61cf3-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="61cf3-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="61cf3-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="61cf3-138">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="61cf3-139">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="61cf3-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="61cf3-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="61cf3-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="61cf3-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="61cf3-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="61cf3-142">Назначение профиля подробное состояние устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="61cf3-143">Возможные значения: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span><span class="sxs-lookup"><span data-stu-id="61cf3-143">Possible values are: `none`, `hardwareRequirementsNotMet`, `surfaceHubProfileNotSupported`, `holoLensProfileNotSupported`, `windowsPcProfileNotSupported`.</span></span>|
|<span data-ttu-id="61cf3-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="61cf3-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="61cf3-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61cf3-145">DateTimeOffset</span></span>|<span data-ttu-id="61cf3-146">Время набора профилей устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-147">groupTag</span><span class="sxs-lookup"><span data-stu-id="61cf3-147">groupTag</span></span>|<span data-ttu-id="61cf3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-148">String</span></span>|<span data-ttu-id="61cf3-149">Групповой тег устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-149">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="61cf3-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="61cf3-151">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-151">String</span></span>|<span data-ttu-id="61cf3-152">Идентификатор заказа покупки устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="61cf3-153">serialNumber</span></span>|<span data-ttu-id="61cf3-154">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-154">String</span></span>|<span data-ttu-id="61cf3-155">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="61cf3-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-156">productKey</span><span class="sxs-lookup"><span data-stu-id="61cf3-156">productKey</span></span>|<span data-ttu-id="61cf3-157">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-157">String</span></span>|<span data-ttu-id="61cf3-158">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="61cf3-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="61cf3-159">manufacturer</span></span>|<span data-ttu-id="61cf3-160">String</span><span class="sxs-lookup"><span data-stu-id="61cf3-160">String</span></span>|<span data-ttu-id="61cf3-161">Oem производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-162">model</span><span class="sxs-lookup"><span data-stu-id="61cf3-162">model</span></span>|<span data-ttu-id="61cf3-163">String</span><span class="sxs-lookup"><span data-stu-id="61cf3-163">String</span></span>|<span data-ttu-id="61cf3-164">Имя модели устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="61cf3-165">enrollmentState</span></span>|[<span data-ttu-id="61cf3-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="61cf3-166">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="61cf3-167">Состояние регистрации intune устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="61cf3-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="61cf3-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="61cf3-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="61cf3-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="61cf3-169">lastContactedDateTime</span></span>|<span data-ttu-id="61cf3-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61cf3-170">DateTimeOffset</span></span>|<span data-ttu-id="61cf3-171">Intune Last Contacted Date Time of the Windows autopilot device.</span><span class="sxs-lookup"><span data-stu-id="61cf3-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="61cf3-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="61cf3-172">addressableUserName</span></span>|<span data-ttu-id="61cf3-173">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-173">String</span></span>|<span data-ttu-id="61cf3-174">Адресное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="61cf3-174">Addressable user name.</span></span>|
|<span data-ttu-id="61cf3-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="61cf3-175">userPrincipalName</span></span>|<span data-ttu-id="61cf3-176">String</span><span class="sxs-lookup"><span data-stu-id="61cf3-176">String</span></span>|<span data-ttu-id="61cf3-177">Имя главного пользователя.</span><span class="sxs-lookup"><span data-stu-id="61cf3-177">User Principal Name.</span></span>|
|<span data-ttu-id="61cf3-178">resourceName</span><span class="sxs-lookup"><span data-stu-id="61cf3-178">resourceName</span></span>|<span data-ttu-id="61cf3-179">String</span><span class="sxs-lookup"><span data-stu-id="61cf3-179">String</span></span>|<span data-ttu-id="61cf3-180">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="61cf3-180">Resource Name.</span></span>|
|<span data-ttu-id="61cf3-181">skuNumber</span><span class="sxs-lookup"><span data-stu-id="61cf3-181">skuNumber</span></span>|<span data-ttu-id="61cf3-182">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-182">String</span></span>|<span data-ttu-id="61cf3-183">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="61cf3-183">SKU Number</span></span>|
|<span data-ttu-id="61cf3-184">systemFamily</span><span class="sxs-lookup"><span data-stu-id="61cf3-184">systemFamily</span></span>|<span data-ttu-id="61cf3-185">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-185">String</span></span>|<span data-ttu-id="61cf3-186">Семейство system</span><span class="sxs-lookup"><span data-stu-id="61cf3-186">System Family</span></span>|
|<span data-ttu-id="61cf3-187">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="61cf3-187">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="61cf3-188">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-188">String</span></span>|<span data-ttu-id="61cf3-189">AAD Device ID - to be deprecated</span><span class="sxs-lookup"><span data-stu-id="61cf3-189">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="61cf3-190">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="61cf3-190">azureAdDeviceId</span></span>|<span data-ttu-id="61cf3-191">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-191">String</span></span>|<span data-ttu-id="61cf3-192">ID устройства AAD</span><span class="sxs-lookup"><span data-stu-id="61cf3-192">AAD Device ID</span></span>|
|<span data-ttu-id="61cf3-193">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="61cf3-193">managedDeviceId</span></span>|<span data-ttu-id="61cf3-194">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-194">String</span></span>|<span data-ttu-id="61cf3-195">Управляемый ID устройства</span><span class="sxs-lookup"><span data-stu-id="61cf3-195">Managed Device ID</span></span>|
|<span data-ttu-id="61cf3-196">displayName</span><span class="sxs-lookup"><span data-stu-id="61cf3-196">displayName</span></span>|<span data-ttu-id="61cf3-197">Строка</span><span class="sxs-lookup"><span data-stu-id="61cf3-197">String</span></span>|<span data-ttu-id="61cf3-198">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="61cf3-198">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="61cf3-199">Отклик</span><span class="sxs-lookup"><span data-stu-id="61cf3-199">Response</span></span>
<span data-ttu-id="61cf3-200">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="61cf3-200">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61cf3-201">Пример</span><span class="sxs-lookup"><span data-stu-id="61cf3-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="61cf3-202">Запрос</span><span class="sxs-lookup"><span data-stu-id="61cf3-202">Request</span></span>
<span data-ttu-id="61cf3-203">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="61cf3-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1077

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="61cf3-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="61cf3-204">Response</span></span>
<span data-ttu-id="61cf3-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="61cf3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
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
  "azureAdDeviceId": "Azure Ad Device Id value",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```




