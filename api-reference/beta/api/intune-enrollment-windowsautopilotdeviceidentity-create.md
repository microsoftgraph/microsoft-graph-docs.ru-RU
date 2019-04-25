---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1fe0f7195007eaf937b1d6d82b20f1978136559
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532550"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="be18d-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="be18d-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="be18d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be18d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be18d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be18d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be18d-106">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="be18d-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be18d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="be18d-107">Prerequisites</span></span>
<span data-ttu-id="be18d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be18d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be18d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="be18d-110">Permission type</span></span>|<span data-ttu-id="be18d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="be18d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be18d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="be18d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="be18d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be18d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="be18d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="be18d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be18d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be18d-115">Not supported.</span></span>|
|<span data-ttu-id="be18d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="be18d-116">Application</span></span>|<span data-ttu-id="be18d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be18d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be18d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="be18d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="be18d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="be18d-119">Request headers</span></span>
|<span data-ttu-id="be18d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="be18d-120">Header</span></span>|<span data-ttu-id="be18d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="be18d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be18d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="be18d-122">Authorization</span></span>|<span data-ttu-id="be18d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="be18d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be18d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="be18d-124">Accept</span></span>|<span data-ttu-id="be18d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="be18d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be18d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="be18d-126">Request body</span></span>
<span data-ttu-id="be18d-127">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be18d-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="be18d-128">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="be18d-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="be18d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="be18d-129">Property</span></span>|<span data-ttu-id="be18d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="be18d-130">Type</span></span>|<span data-ttu-id="be18d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="be18d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be18d-132">id</span><span class="sxs-lookup"><span data-stu-id="be18d-132">id</span></span>|<span data-ttu-id="be18d-133">Строка</span><span class="sxs-lookup"><span data-stu-id="be18d-133">String</span></span>|<span data-ttu-id="be18d-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="be18d-134">The GUID for the object</span></span>|
|<span data-ttu-id="be18d-135">Деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="be18d-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="be18d-136">Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="be18d-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="be18d-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="be18d-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="be18d-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="be18d-139">Деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="be18d-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="be18d-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="be18d-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="be18d-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="be18d-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="be18d-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="be18d-143">Деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="be18d-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="be18d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be18d-144">DateTimeOffset</span></span>|<span data-ttu-id="be18d-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="be18d-146">orderIdentifier</span></span>|<span data-ttu-id="be18d-147">String</span><span class="sxs-lookup"><span data-stu-id="be18d-147">String</span></span>|<span data-ttu-id="be18d-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="be18d-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="be18d-149">Грауптаг</span><span class="sxs-lookup"><span data-stu-id="be18d-149">groupTag</span></span>|<span data-ttu-id="be18d-150">String</span><span class="sxs-lookup"><span data-stu-id="be18d-150">String</span></span>|<span data-ttu-id="be18d-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-152">Пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="be18d-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="be18d-153">String</span><span class="sxs-lookup"><span data-stu-id="be18d-153">String</span></span>|<span data-ttu-id="be18d-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="be18d-155">serialNumber</span></span>|<span data-ttu-id="be18d-156">String</span><span class="sxs-lookup"><span data-stu-id="be18d-156">String</span></span>|<span data-ttu-id="be18d-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="be18d-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-158">productKey</span><span class="sxs-lookup"><span data-stu-id="be18d-158">productKey</span></span>|<span data-ttu-id="be18d-159">Строка</span><span class="sxs-lookup"><span data-stu-id="be18d-159">String</span></span>|<span data-ttu-id="be18d-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="be18d-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="be18d-161">manufacturer</span></span>|<span data-ttu-id="be18d-162">String</span><span class="sxs-lookup"><span data-stu-id="be18d-162">String</span></span>|<span data-ttu-id="be18d-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-164">model</span><span class="sxs-lookup"><span data-stu-id="be18d-164">model</span></span>|<span data-ttu-id="be18d-165">String</span><span class="sxs-lookup"><span data-stu-id="be18d-165">String</span></span>|<span data-ttu-id="be18d-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-167">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="be18d-167">enrollmentState</span></span>|[<span data-ttu-id="be18d-168">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="be18d-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="be18d-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="be18d-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="be18d-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="be18d-171">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="be18d-171">lastContactedDateTime</span></span>|<span data-ttu-id="be18d-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be18d-172">DateTimeOffset</span></span>|<span data-ttu-id="be18d-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="be18d-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="be18d-174">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="be18d-174">addressableUserName</span></span>|<span data-ttu-id="be18d-175">String</span><span class="sxs-lookup"><span data-stu-id="be18d-175">String</span></span>|<span data-ttu-id="be18d-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="be18d-176">Addressable user name.</span></span>|
|<span data-ttu-id="be18d-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="be18d-177">userPrincipalName</span></span>|<span data-ttu-id="be18d-178">String</span><span class="sxs-lookup"><span data-stu-id="be18d-178">String</span></span>|<span data-ttu-id="be18d-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="be18d-179">User Principal Name.</span></span>|
|<span data-ttu-id="be18d-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="be18d-180">resourceName</span></span>|<span data-ttu-id="be18d-181">String</span><span class="sxs-lookup"><span data-stu-id="be18d-181">String</span></span>|<span data-ttu-id="be18d-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="be18d-182">Resource Name.</span></span>|
|<span data-ttu-id="be18d-183">Скунумбер</span><span class="sxs-lookup"><span data-stu-id="be18d-183">skuNumber</span></span>|<span data-ttu-id="be18d-184">String</span><span class="sxs-lookup"><span data-stu-id="be18d-184">String</span></span>|<span data-ttu-id="be18d-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="be18d-185">SKU Number</span></span>|
|<span data-ttu-id="be18d-186">Системфамили</span><span class="sxs-lookup"><span data-stu-id="be18d-186">systemFamily</span></span>|<span data-ttu-id="be18d-187">String</span><span class="sxs-lookup"><span data-stu-id="be18d-187">String</span></span>|<span data-ttu-id="be18d-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="be18d-188">System Family</span></span>|
|<span data-ttu-id="be18d-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="be18d-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="be18d-190">String</span><span class="sxs-lookup"><span data-stu-id="be18d-190">String</span></span>|<span data-ttu-id="be18d-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="be18d-191">AAD Device ID</span></span>|
|<span data-ttu-id="be18d-192">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="be18d-192">managedDeviceId</span></span>|<span data-ttu-id="be18d-193">String</span><span class="sxs-lookup"><span data-stu-id="be18d-193">String</span></span>|<span data-ttu-id="be18d-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="be18d-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="be18d-195">Ответ</span><span class="sxs-lookup"><span data-stu-id="be18d-195">Response</span></span>
<span data-ttu-id="be18d-196">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="be18d-196">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be18d-197">Пример</span><span class="sxs-lookup"><span data-stu-id="be18d-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="be18d-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="be18d-198">Request</span></span>
<span data-ttu-id="be18d-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="be18d-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be18d-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="be18d-200">Response</span></span>
<span data-ttu-id="be18d-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="be18d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





