---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad7bf9d9066edb4e6494c39d72b8fa9f88788d81
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37179973"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="ecbce-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="ecbce-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="ecbce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecbce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecbce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ecbce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecbce-106">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="ecbce-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecbce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ecbce-107">Prerequisites</span></span>
<span data-ttu-id="ecbce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecbce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecbce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ecbce-110">Permission type</span></span>|<span data-ttu-id="ecbce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ecbce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecbce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ecbce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecbce-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbce-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ecbce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ecbce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecbce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ecbce-115">Not supported.</span></span>|
|<span data-ttu-id="ecbce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ecbce-116">Application</span></span>|<span data-ttu-id="ecbce-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecbce-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecbce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ecbce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="ecbce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ecbce-119">Request headers</span></span>
|<span data-ttu-id="ecbce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ecbce-120">Header</span></span>|<span data-ttu-id="ecbce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ecbce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecbce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ecbce-122">Authorization</span></span>|<span data-ttu-id="ecbce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ecbce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecbce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ecbce-124">Accept</span></span>|<span data-ttu-id="ecbce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecbce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecbce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ecbce-126">Request body</span></span>
<span data-ttu-id="ecbce-127">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecbce-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="ecbce-128">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="ecbce-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="ecbce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecbce-129">Property</span></span>|<span data-ttu-id="ecbce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ecbce-130">Type</span></span>|<span data-ttu-id="ecbce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ecbce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecbce-132">id</span><span class="sxs-lookup"><span data-stu-id="ecbce-132">id</span></span>|<span data-ttu-id="ecbce-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ecbce-133">String</span></span>|<span data-ttu-id="ecbce-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="ecbce-134">The GUID for the object</span></span>|
|<span data-ttu-id="ecbce-135">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="ecbce-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="ecbce-136">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="ecbce-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="ecbce-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="ecbce-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ecbce-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="ecbce-139">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="ecbce-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="ecbce-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="ecbce-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="ecbce-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="ecbce-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="ecbce-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="ecbce-143">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="ecbce-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="ecbce-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbce-144">DateTimeOffset</span></span>|<span data-ttu-id="ecbce-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="ecbce-146">orderIdentifier</span></span>|<span data-ttu-id="ecbce-147">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-147">String</span></span>|<span data-ttu-id="ecbce-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="ecbce-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="ecbce-149">грауптаг</span><span class="sxs-lookup"><span data-stu-id="ecbce-149">groupTag</span></span>|<span data-ttu-id="ecbce-150">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-150">String</span></span>|<span data-ttu-id="ecbce-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-152">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="ecbce-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="ecbce-153">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-153">String</span></span>|<span data-ttu-id="ecbce-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ecbce-155">serialNumber</span></span>|<span data-ttu-id="ecbce-156">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-156">String</span></span>|<span data-ttu-id="ecbce-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="ecbce-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-158">productKey</span><span class="sxs-lookup"><span data-stu-id="ecbce-158">productKey</span></span>|<span data-ttu-id="ecbce-159">Строка</span><span class="sxs-lookup"><span data-stu-id="ecbce-159">String</span></span>|<span data-ttu-id="ecbce-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="ecbce-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ecbce-161">manufacturer</span></span>|<span data-ttu-id="ecbce-162">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-162">String</span></span>|<span data-ttu-id="ecbce-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-164">model</span><span class="sxs-lookup"><span data-stu-id="ecbce-164">model</span></span>|<span data-ttu-id="ecbce-165">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-165">String</span></span>|<span data-ttu-id="ecbce-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-167">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="ecbce-167">enrollmentState</span></span>|[<span data-ttu-id="ecbce-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="ecbce-168">enrollmentState</span></span>](../resources/intune-shared-enrollmentstate.md)|<span data-ttu-id="ecbce-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="ecbce-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="ecbce-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="ecbce-171">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="ecbce-171">lastContactedDateTime</span></span>|<span data-ttu-id="ecbce-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecbce-172">DateTimeOffset</span></span>|<span data-ttu-id="ecbce-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="ecbce-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="ecbce-174">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="ecbce-174">addressableUserName</span></span>|<span data-ttu-id="ecbce-175">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-175">String</span></span>|<span data-ttu-id="ecbce-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="ecbce-176">Addressable user name.</span></span>|
|<span data-ttu-id="ecbce-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ecbce-177">userPrincipalName</span></span>|<span data-ttu-id="ecbce-178">String</span><span class="sxs-lookup"><span data-stu-id="ecbce-178">String</span></span>|<span data-ttu-id="ecbce-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="ecbce-179">User Principal Name.</span></span>|
|<span data-ttu-id="ecbce-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="ecbce-180">resourceName</span></span>|<span data-ttu-id="ecbce-181">String</span><span class="sxs-lookup"><span data-stu-id="ecbce-181">String</span></span>|<span data-ttu-id="ecbce-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="ecbce-182">Resource Name.</span></span>|
|<span data-ttu-id="ecbce-183">скунумбер</span><span class="sxs-lookup"><span data-stu-id="ecbce-183">skuNumber</span></span>|<span data-ttu-id="ecbce-184">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-184">String</span></span>|<span data-ttu-id="ecbce-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="ecbce-185">SKU Number</span></span>|
|<span data-ttu-id="ecbce-186">системфамили</span><span class="sxs-lookup"><span data-stu-id="ecbce-186">systemFamily</span></span>|<span data-ttu-id="ecbce-187">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-187">String</span></span>|<span data-ttu-id="ecbce-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="ecbce-188">System Family</span></span>|
|<span data-ttu-id="ecbce-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="ecbce-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="ecbce-190">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-190">String</span></span>|<span data-ttu-id="ecbce-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="ecbce-191">AAD Device ID</span></span>|
|<span data-ttu-id="ecbce-192">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="ecbce-192">managedDeviceId</span></span>|<span data-ttu-id="ecbce-193">String.</span><span class="sxs-lookup"><span data-stu-id="ecbce-193">String</span></span>|<span data-ttu-id="ecbce-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="ecbce-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="ecbce-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecbce-195">Response</span></span>
<span data-ttu-id="ecbce-196">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ecbce-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecbce-197">Пример</span><span class="sxs-lookup"><span data-stu-id="ecbce-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecbce-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="ecbce-198">Request</span></span>
<span data-ttu-id="ecbce-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ecbce-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 1035

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
  "managedDeviceId": "Managed Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="ecbce-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="ecbce-200">Response</span></span>
<span data-ttu-id="ecbce-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ecbce-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1084

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
  "managedDeviceId": "Managed Device Id value"
}
```




