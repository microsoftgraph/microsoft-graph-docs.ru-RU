---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойств объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e6aaba99e2526b139fd06fa047ec36828ef24a6
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570789"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="b8a86-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b8a86-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="b8a86-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8a86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8a86-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b8a86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8a86-106">Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="b8a86-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8a86-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b8a86-107">Prerequisites</span></span>
<span data-ttu-id="b8a86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8a86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b8a86-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8a86-110">Permission type</span></span>|<span data-ttu-id="b8a86-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8a86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8a86-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8a86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8a86-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8a86-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b8a86-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8a86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8a86-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8a86-115">Not supported.</span></span>|
|<span data-ttu-id="b8a86-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8a86-116">Application</span></span>|<span data-ttu-id="b8a86-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8a86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8a86-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8a86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b8a86-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8a86-119">Request headers</span></span>
|<span data-ttu-id="b8a86-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8a86-120">Header</span></span>|<span data-ttu-id="b8a86-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b8a86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8a86-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8a86-122">Authorization</span></span>|<span data-ttu-id="b8a86-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8a86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8a86-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b8a86-124">Accept</span></span>|<span data-ttu-id="b8a86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8a86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8a86-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8a86-126">Request body</span></span>
<span data-ttu-id="b8a86-127">В тексте запроса добавьте представление объекта [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8a86-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="b8a86-128">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b8a86-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="b8a86-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8a86-129">Property</span></span>|<span data-ttu-id="b8a86-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b8a86-130">Type</span></span>|<span data-ttu-id="b8a86-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b8a86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8a86-132">id</span><span class="sxs-lookup"><span data-stu-id="b8a86-132">id</span></span>|<span data-ttu-id="b8a86-133">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-133">String</span></span>|<span data-ttu-id="b8a86-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="b8a86-134">The GUID for the object</span></span>|
|<span data-ttu-id="b8a86-135">Деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="b8a86-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="b8a86-136">Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="b8a86-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="b8a86-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="b8a86-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="b8a86-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="b8a86-139">Деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="b8a86-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="b8a86-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="b8a86-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="b8a86-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="b8a86-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="b8a86-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="b8a86-143">Деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b8a86-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="b8a86-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8a86-144">DateTimeOffset</span></span>|<span data-ttu-id="b8a86-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="b8a86-146">orderIdentifier</span></span>|<span data-ttu-id="b8a86-147">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-147">String</span></span>|<span data-ttu-id="b8a86-148">Идентификатор заказа устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-149">Пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="b8a86-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="b8a86-150">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-150">String</span></span>|<span data-ttu-id="b8a86-151">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b8a86-152">serialNumber</span></span>|<span data-ttu-id="b8a86-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-153">String</span></span>|<span data-ttu-id="b8a86-154">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b8a86-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-155">productKey</span><span class="sxs-lookup"><span data-stu-id="b8a86-155">productKey</span></span>|<span data-ttu-id="b8a86-156">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-156">String</span></span>|<span data-ttu-id="b8a86-157">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="b8a86-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b8a86-158">manufacturer</span></span>|<span data-ttu-id="b8a86-159">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-159">String</span></span>|<span data-ttu-id="b8a86-160">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-161">model</span><span class="sxs-lookup"><span data-stu-id="b8a86-161">model</span></span>|<span data-ttu-id="b8a86-162">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-162">String</span></span>|<span data-ttu-id="b8a86-163">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-164">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b8a86-164">enrollmentState</span></span>|[<span data-ttu-id="b8a86-165">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="b8a86-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="b8a86-166">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="b8a86-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="b8a86-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="b8a86-168">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="b8a86-168">lastContactedDateTime</span></span>|<span data-ttu-id="b8a86-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8a86-169">DateTimeOffset</span></span>|<span data-ttu-id="b8a86-170">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="b8a86-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="b8a86-171">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="b8a86-171">addressableUserName</span></span>|<span data-ttu-id="b8a86-172">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-172">String</span></span>|<span data-ttu-id="b8a86-173">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="b8a86-173">Addressable user name.</span></span>|
|<span data-ttu-id="b8a86-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b8a86-174">userPrincipalName</span></span>|<span data-ttu-id="b8a86-175">String</span><span class="sxs-lookup"><span data-stu-id="b8a86-175">String</span></span>|<span data-ttu-id="b8a86-176">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="b8a86-176">User Principal Name.</span></span>|
|<span data-ttu-id="b8a86-177">resourceName</span><span class="sxs-lookup"><span data-stu-id="b8a86-177">resourceName</span></span>|<span data-ttu-id="b8a86-178">String</span><span class="sxs-lookup"><span data-stu-id="b8a86-178">String</span></span>|<span data-ttu-id="b8a86-179">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="b8a86-179">Resource Name.</span></span>|
|<span data-ttu-id="b8a86-180">Скунумбер</span><span class="sxs-lookup"><span data-stu-id="b8a86-180">skuNumber</span></span>|<span data-ttu-id="b8a86-181">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-181">String</span></span>|<span data-ttu-id="b8a86-182">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="b8a86-182">SKU Number</span></span>|
|<span data-ttu-id="b8a86-183">Системфамили</span><span class="sxs-lookup"><span data-stu-id="b8a86-183">systemFamily</span></span>|<span data-ttu-id="b8a86-184">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-184">String</span></span>|<span data-ttu-id="b8a86-185">Семейство системы</span><span class="sxs-lookup"><span data-stu-id="b8a86-185">System Family</span></span>|
|<span data-ttu-id="b8a86-186">Свойства azureactivedirectorydeviceid</span><span class="sxs-lookup"><span data-stu-id="b8a86-186">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="b8a86-187">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-187">String</span></span>|<span data-ttu-id="b8a86-188">ИДЕНТИФИКАТОР устройства AAD</span><span class="sxs-lookup"><span data-stu-id="b8a86-188">AAD Device ID</span></span>|
|<span data-ttu-id="b8a86-189">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="b8a86-189">managedDeviceId</span></span>|<span data-ttu-id="b8a86-190">Строка</span><span class="sxs-lookup"><span data-stu-id="b8a86-190">String</span></span>|<span data-ttu-id="b8a86-191">Управляемый идентификатор устройства</span><span class="sxs-lookup"><span data-stu-id="b8a86-191">Managed Device ID</span></span>|



## <a name="response"></a><span data-ttu-id="b8a86-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8a86-192">Response</span></span>
<span data-ttu-id="b8a86-193">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8a86-193">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8a86-194">Пример</span><span class="sxs-lookup"><span data-stu-id="b8a86-194">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8a86-195">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8a86-195">Request</span></span>
<span data-ttu-id="b8a86-196">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8a86-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 1001

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
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

### <a name="response"></a><span data-ttu-id="b8a86-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8a86-197">Response</span></span>
<span data-ttu-id="b8a86-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8a86-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1050

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
  "deploymentProfileAssignmentStatus": "assignedInSync",
  "deploymentProfileAssignmentDetailedStatus": "hardwareRequirementsNotMet",
  "deploymentProfileAssignedDateTime": "2016-12-31T23:58:26.2447023-08:00",
  "orderIdentifier": "Order Identifier value",
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




