---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойств объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ed1e8159b91aed11cc631e26aa02d79dbb4cce4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775907"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="2f99f-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2f99f-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="2f99f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f99f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f99f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f99f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f99f-106">Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="2f99f-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f99f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="2f99f-107">Prerequisites</span></span>
<span data-ttu-id="2f99f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f99f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f99f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f99f-110">Permission type</span></span>|<span data-ttu-id="2f99f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f99f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f99f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f99f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f99f-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f99f-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2f99f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f99f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f99f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f99f-115">Not supported.</span></span>|
|<span data-ttu-id="2f99f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f99f-116">Application</span></span>|<span data-ttu-id="2f99f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f99f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f99f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f99f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="2f99f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f99f-119">Request headers</span></span>
|<span data-ttu-id="2f99f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f99f-120">Header</span></span>|<span data-ttu-id="2f99f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2f99f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f99f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f99f-122">Authorization</span></span>|<span data-ttu-id="2f99f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f99f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f99f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="2f99f-124">Accept</span></span>|<span data-ttu-id="2f99f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f99f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f99f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f99f-126">Request body</span></span>
<span data-ttu-id="2f99f-127">В тексте запроса добавьте представление объекта [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f99f-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="2f99f-128">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="2f99f-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="2f99f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f99f-129">Property</span></span>|<span data-ttu-id="2f99f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2f99f-130">Type</span></span>|<span data-ttu-id="2f99f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2f99f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f99f-132">id</span><span class="sxs-lookup"><span data-stu-id="2f99f-132">id</span></span>|<span data-ttu-id="2f99f-133">Строка</span><span class="sxs-lookup"><span data-stu-id="2f99f-133">String</span></span>|<span data-ttu-id="2f99f-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="2f99f-134">The GUID for the object</span></span>|
|<span data-ttu-id="2f99f-135">Деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="2f99f-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="2f99f-136">Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="2f99f-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="2f99f-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="2f99f-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2f99f-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="2f99f-139">Деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="2f99f-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="2f99f-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="2f99f-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="2f99f-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="2f99f-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="2f99f-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="2f99f-143">Деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="2f99f-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="2f99f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f99f-144">DateTimeOffset</span></span>|<span data-ttu-id="2f99f-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="2f99f-146">orderIdentifier</span></span>|<span data-ttu-id="2f99f-147">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-147">String</span></span>|<span data-ttu-id="2f99f-148">Идентификатор заказа устройства с автопилотом Windows — не является устаревшим</span><span class="sxs-lookup"><span data-stu-id="2f99f-148">Order Identifier of the Windows autopilot device - Deprecated</span></span>|
|<span data-ttu-id="2f99f-149">Грауптаг</span><span class="sxs-lookup"><span data-stu-id="2f99f-149">groupTag</span></span>|<span data-ttu-id="2f99f-150">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-150">String</span></span>|<span data-ttu-id="2f99f-151">Тег Group для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-151">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-152">Пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="2f99f-152">purchaseOrderIdentifier</span></span>|<span data-ttu-id="2f99f-153">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-153">String</span></span>|<span data-ttu-id="2f99f-154">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-154">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-155">serialNumber</span><span class="sxs-lookup"><span data-stu-id="2f99f-155">serialNumber</span></span>|<span data-ttu-id="2f99f-156">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-156">String</span></span>|<span data-ttu-id="2f99f-157">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2f99f-157">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-158">productKey</span><span class="sxs-lookup"><span data-stu-id="2f99f-158">productKey</span></span>|<span data-ttu-id="2f99f-159">Строка</span><span class="sxs-lookup"><span data-stu-id="2f99f-159">String</span></span>|<span data-ttu-id="2f99f-160">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2f99f-160">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-161">manufacturer</span><span class="sxs-lookup"><span data-stu-id="2f99f-161">manufacturer</span></span>|<span data-ttu-id="2f99f-162">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-162">String</span></span>|<span data-ttu-id="2f99f-163">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-163">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-164">model</span><span class="sxs-lookup"><span data-stu-id="2f99f-164">model</span></span>|<span data-ttu-id="2f99f-165">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-165">String</span></span>|<span data-ttu-id="2f99f-166">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-166">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-167">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2f99f-167">enrollmentState</span></span>|[<span data-ttu-id="2f99f-168">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="2f99f-168">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2f99f-169">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-169">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="2f99f-170">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="2f99f-170">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2f99f-171">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="2f99f-171">lastContactedDateTime</span></span>|<span data-ttu-id="2f99f-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f99f-172">DateTimeOffset</span></span>|<span data-ttu-id="2f99f-173">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="2f99f-173">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="2f99f-174">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="2f99f-174">addressableUserName</span></span>|<span data-ttu-id="2f99f-175">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-175">String</span></span>|<span data-ttu-id="2f99f-176">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="2f99f-176">Addressable user name.</span></span>|
|<span data-ttu-id="2f99f-177">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2f99f-177">userPrincipalName</span></span>|<span data-ttu-id="2f99f-178">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-178">String</span></span>|<span data-ttu-id="2f99f-179">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="2f99f-179">User Principal Name.</span></span>|
|<span data-ttu-id="2f99f-180">resourceName</span><span class="sxs-lookup"><span data-stu-id="2f99f-180">resourceName</span></span>|<span data-ttu-id="2f99f-181">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-181">String</span></span>|<span data-ttu-id="2f99f-182">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="2f99f-182">Resource Name.</span></span>|
|<span data-ttu-id="2f99f-183">Скунумбер</span><span class="sxs-lookup"><span data-stu-id="2f99f-183">skuNumber</span></span>|<span data-ttu-id="2f99f-184">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-184">String</span></span>|<span data-ttu-id="2f99f-185">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="2f99f-185">SKU Number</span></span>|
|<span data-ttu-id="2f99f-186">Системфамили</span><span class="sxs-lookup"><span data-stu-id="2f99f-186">systemFamily</span></span>|<span data-ttu-id="2f99f-187">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-187">String</span></span>|<span data-ttu-id="2f99f-188">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="2f99f-188">System Family</span></span>|
|<span data-ttu-id="2f99f-189">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="2f99f-189">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="2f99f-190">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-190">String</span></span>|<span data-ttu-id="2f99f-191">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="2f99f-191">AAD Device ID</span></span>|
|<span data-ttu-id="2f99f-192">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="2f99f-192">managedDeviceId</span></span>|<span data-ttu-id="2f99f-193">String</span><span class="sxs-lookup"><span data-stu-id="2f99f-193">String</span></span>|<span data-ttu-id="2f99f-194">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="2f99f-194">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="2f99f-195">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f99f-195">Response</span></span>
<span data-ttu-id="2f99f-196">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2f99f-196">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f99f-197">Пример</span><span class="sxs-lookup"><span data-stu-id="2f99f-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f99f-198">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f99f-198">Request</span></span>
<span data-ttu-id="2f99f-199">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f99f-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
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

### <a name="response"></a><span data-ttu-id="2f99f-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f99f-200">Response</span></span>
<span data-ttu-id="2f99f-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2f99f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





