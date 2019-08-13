---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 66b63566dcd7ca2b498e60e0a5e403492e37eeb9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356083"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="b8014-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b8014-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="b8014-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8014-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8014-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8014-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8014-106">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="b8014-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8014-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8014-107">Prerequisites</span></span>
<span data-ttu-id="b8014-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8014-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8014-110">Permission type</span></span>|<span data-ttu-id="b8014-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8014-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8014-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8014-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8014-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8014-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8014-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8014-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8014-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8014-115">Not supported.</span></span>|
|<span data-ttu-id="b8014-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8014-116">Application</span></span>|<span data-ttu-id="b8014-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8014-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8014-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8014-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="b8014-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8014-119">Request headers</span></span>
|<span data-ttu-id="b8014-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8014-120">Header</span></span>|<span data-ttu-id="b8014-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b8014-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8014-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8014-122">Authorization</span></span>|<span data-ttu-id="b8014-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8014-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8014-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b8014-124">Accept</span></span>|<span data-ttu-id="b8014-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8014-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8014-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8014-126">Request body</span></span>
<span data-ttu-id="b8014-127">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8014-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="b8014-128">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="b8014-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="b8014-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8014-129">Property</span></span>|<span data-ttu-id="b8014-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b8014-130">Type</span></span>|<span data-ttu-id="b8014-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b8014-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8014-132">id</span><span class="sxs-lookup"><span data-stu-id="b8014-132">id</span></span>|<span data-ttu-id="b8014-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b8014-133">String</span></span>|<span data-ttu-id="b8014-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b8014-134">The GUID for the object</span></span>|
|<span data-ttu-id="b8014-135">деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="b8014-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="b8014-136">виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="b8014-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="b8014-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="b8014-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b8014-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="b8014-139">деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="b8014-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="b8014-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="b8014-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="b8014-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="b8014-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="b8014-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="b8014-143">деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b8014-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="b8014-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8014-144">DateTimeOffset</span></span>|<span data-ttu-id="b8014-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8014-146">orderIdentifier</span></span>|<span data-ttu-id="b8014-147">String</span><span class="sxs-lookup"><span data-stu-id="b8014-147">String</span></span>|<span data-ttu-id="b8014-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="b8014-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="b8014-149">грауптаг</span><span class="sxs-lookup"><span data-stu-id="b8014-149">groupTag</span></span>|<span data-ttu-id="b8014-150">String</span><span class="sxs-lookup"><span data-stu-id="b8014-150">String</span></span>|<span data-ttu-id="b8014-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-152">пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="b8014-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="b8014-153">String</span><span class="sxs-lookup"><span data-stu-id="b8014-153">String</span></span>|<span data-ttu-id="b8014-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b8014-155">serialNumber</span></span>|<span data-ttu-id="b8014-156">String</span><span class="sxs-lookup"><span data-stu-id="b8014-156">String</span></span>|<span data-ttu-id="b8014-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b8014-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-158">productKey</span><span class="sxs-lookup"><span data-stu-id="b8014-158">productKey</span></span>|<span data-ttu-id="b8014-159">Строка</span><span class="sxs-lookup"><span data-stu-id="b8014-159">String</span></span>|<span data-ttu-id="b8014-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b8014-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b8014-161">manufacturer</span></span>|<span data-ttu-id="b8014-162">String</span><span class="sxs-lookup"><span data-stu-id="b8014-162">String</span></span>|<span data-ttu-id="b8014-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-164">model</span><span class="sxs-lookup"><span data-stu-id="b8014-164">model</span></span>|<span data-ttu-id="b8014-165">String</span><span class="sxs-lookup"><span data-stu-id="b8014-165">String</span></span>|<span data-ttu-id="b8014-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-167">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b8014-167">enrollmentState</span></span>|[<span data-ttu-id="b8014-168">енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b8014-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="b8014-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="b8014-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b8014-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b8014-171">ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b8014-171">lastContactedDateTime</span></span>|<span data-ttu-id="b8014-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8014-172">DateTimeOffset</span></span>|<span data-ttu-id="b8014-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8014-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8014-174">аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="b8014-174">addressableUserName</span></span>|<span data-ttu-id="b8014-175">String</span><span class="sxs-lookup"><span data-stu-id="b8014-175">String</span></span>|<span data-ttu-id="b8014-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="b8014-176">Addressable user name.</span></span>|
|<span data-ttu-id="b8014-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8014-177">userPrincipalName</span></span>|<span data-ttu-id="b8014-178">String</span><span class="sxs-lookup"><span data-stu-id="b8014-178">String</span></span>|<span data-ttu-id="b8014-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8014-179">User Principal Name.</span></span>|
|<span data-ttu-id="b8014-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="b8014-180">resourceName</span></span>|<span data-ttu-id="b8014-181">String</span><span class="sxs-lookup"><span data-stu-id="b8014-181">String</span></span>|<span data-ttu-id="b8014-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="b8014-182">Resource Name.</span></span>|
|<span data-ttu-id="b8014-183">скунумбер</span><span class="sxs-lookup"><span data-stu-id="b8014-183">skuNumber</span></span>|<span data-ttu-id="b8014-184">String</span><span class="sxs-lookup"><span data-stu-id="b8014-184">String</span></span>|<span data-ttu-id="b8014-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="b8014-185">SKU Number</span></span>|
|<span data-ttu-id="b8014-186">системфамили</span><span class="sxs-lookup"><span data-stu-id="b8014-186">systemFamily</span></span>|<span data-ttu-id="b8014-187">String</span><span class="sxs-lookup"><span data-stu-id="b8014-187">String</span></span>|<span data-ttu-id="b8014-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="b8014-188">System Family</span></span>|
|<span data-ttu-id="b8014-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="b8014-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="b8014-190">String</span><span class="sxs-lookup"><span data-stu-id="b8014-190">String</span></span>|<span data-ttu-id="b8014-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="b8014-191">AAD Device ID</span></span>|
|<span data-ttu-id="b8014-192">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="b8014-192">managedDeviceId</span></span>|<span data-ttu-id="b8014-193">String</span><span class="sxs-lookup"><span data-stu-id="b8014-193">String</span></span>|<span data-ttu-id="b8014-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="b8014-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="b8014-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8014-195">Response</span></span>
<span data-ttu-id="b8014-196">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8014-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8014-197">Пример</span><span class="sxs-lookup"><span data-stu-id="b8014-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8014-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8014-198">Request</span></span>
<span data-ttu-id="b8014-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8014-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b8014-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8014-200">Response</span></span>
<span data-ttu-id="b8014-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8014-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






