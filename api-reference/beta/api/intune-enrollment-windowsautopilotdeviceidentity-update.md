---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойств объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8d1afaa0b810d2559daa358c9d7af0895e5ac2d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159523"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="a7189-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="a7189-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="a7189-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7189-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7189-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7189-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7189-106">Обновление свойств объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="a7189-106">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7189-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a7189-107">Prerequisites</span></span>
<span data-ttu-id="a7189-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7189-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7189-110">Permission type</span></span>|<span data-ttu-id="a7189-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7189-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7189-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7189-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a7189-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7189-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a7189-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7189-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7189-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7189-115">Not supported.</span></span>|
|<span data-ttu-id="a7189-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7189-116">Application</span></span>|<span data-ttu-id="a7189-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7189-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7189-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7189-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="a7189-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7189-119">Request headers</span></span>
|<span data-ttu-id="a7189-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7189-120">Header</span></span>|<span data-ttu-id="a7189-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a7189-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7189-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7189-122">Authorization</span></span>|<span data-ttu-id="a7189-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7189-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7189-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a7189-124">Accept</span></span>|<span data-ttu-id="a7189-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a7189-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7189-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7189-126">Request body</span></span>
<span data-ttu-id="a7189-127">В тексте запроса добавьте представление объекта [WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7189-127">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="a7189-128">В следующей таблице приведены свойства, необходимые при создании [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="a7189-128">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="a7189-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7189-129">Property</span></span>|<span data-ttu-id="a7189-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a7189-130">Type</span></span>|<span data-ttu-id="a7189-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a7189-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7189-132">id</span><span class="sxs-lookup"><span data-stu-id="a7189-132">id</span></span>|<span data-ttu-id="a7189-133">String</span><span class="sxs-lookup"><span data-stu-id="a7189-133">String</span></span>|<span data-ttu-id="a7189-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="a7189-134">The GUID for the object</span></span>|
|<span data-ttu-id="a7189-135">Деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="a7189-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="a7189-136">Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="a7189-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="a7189-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="a7189-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="a7189-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="a7189-139">Деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="a7189-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="a7189-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="a7189-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="a7189-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="a7189-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="a7189-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="a7189-143">Деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a7189-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="a7189-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7189-144">DateTimeOffset</span></span>|<span data-ttu-id="a7189-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="a7189-146">orderIdentifier</span></span>|<span data-ttu-id="a7189-147">String</span><span class="sxs-lookup"><span data-stu-id="a7189-147">String</span></span>|<span data-ttu-id="a7189-148">Идентификатор заказа устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-149">Пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="a7189-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="a7189-150">String</span><span class="sxs-lookup"><span data-stu-id="a7189-150">String</span></span>|<span data-ttu-id="a7189-151">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a7189-152">serialNumber</span></span>|<span data-ttu-id="a7189-153">String</span><span class="sxs-lookup"><span data-stu-id="a7189-153">String</span></span>|<span data-ttu-id="a7189-154">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a7189-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-155">productKey</span><span class="sxs-lookup"><span data-stu-id="a7189-155">productKey</span></span>|<span data-ttu-id="a7189-156">Строка</span><span class="sxs-lookup"><span data-stu-id="a7189-156">String</span></span>|<span data-ttu-id="a7189-157">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="a7189-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a7189-158">manufacturer</span></span>|<span data-ttu-id="a7189-159">String</span><span class="sxs-lookup"><span data-stu-id="a7189-159">String</span></span>|<span data-ttu-id="a7189-160">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-161">model</span><span class="sxs-lookup"><span data-stu-id="a7189-161">model</span></span>|<span data-ttu-id="a7189-162">String</span><span class="sxs-lookup"><span data-stu-id="a7189-162">String</span></span>|<span data-ttu-id="a7189-163">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-164">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="a7189-164">enrollmentState</span></span>|[<span data-ttu-id="a7189-165">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="a7189-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="a7189-166">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="a7189-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="a7189-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="a7189-168">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a7189-168">lastContactedDateTime</span></span>|<span data-ttu-id="a7189-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7189-169">DateTimeOffset</span></span>|<span data-ttu-id="a7189-170">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="a7189-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="a7189-171">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="a7189-171">addressableUserName</span></span>|<span data-ttu-id="a7189-172">String</span><span class="sxs-lookup"><span data-stu-id="a7189-172">String</span></span>|<span data-ttu-id="a7189-173">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="a7189-173">Addressable user name.</span></span>|
|<span data-ttu-id="a7189-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a7189-174">userPrincipalName</span></span>|<span data-ttu-id="a7189-175">String</span><span class="sxs-lookup"><span data-stu-id="a7189-175">String</span></span>|<span data-ttu-id="a7189-176">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="a7189-176">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="a7189-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7189-177">Response</span></span>
<span data-ttu-id="a7189-178">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7189-178">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7189-179">Пример</span><span class="sxs-lookup"><span data-stu-id="a7189-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7189-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7189-180">Request</span></span>
<span data-ttu-id="a7189-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7189-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
Content-type: application/json
Content-length: 755

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
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a7189-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7189-182">Response</span></span>
<span data-ttu-id="a7189-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7189-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 804

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
  "userPrincipalName": "User Principal Name value"
}
```




