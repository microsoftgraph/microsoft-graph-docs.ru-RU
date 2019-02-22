---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d87a27c120f4866725e2f91828e8c267f655e69c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175306"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="46b25-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="46b25-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="46b25-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46b25-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46b25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46b25-106">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="46b25-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46b25-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46b25-107">Prerequisites</span></span>
<span data-ttu-id="46b25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="46b25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46b25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46b25-110">Permission type</span></span>|<span data-ttu-id="46b25-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46b25-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46b25-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46b25-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46b25-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46b25-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="46b25-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46b25-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46b25-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b25-115">Not supported.</span></span>|
|<span data-ttu-id="46b25-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46b25-116">Application</span></span>|<span data-ttu-id="46b25-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46b25-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46b25-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46b25-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="46b25-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46b25-119">Request headers</span></span>
|<span data-ttu-id="46b25-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46b25-120">Header</span></span>|<span data-ttu-id="46b25-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46b25-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46b25-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46b25-122">Authorization</span></span>|<span data-ttu-id="46b25-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="46b25-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46b25-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46b25-124">Accept</span></span>|<span data-ttu-id="46b25-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46b25-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46b25-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46b25-126">Request body</span></span>
<span data-ttu-id="46b25-127">В тексте запроса добавьте представление объекта windowsAutopilotDeviceIdentity в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46b25-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="46b25-128">В следующей таблице приведены свойства, необходимые при создании windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="46b25-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="46b25-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46b25-129">Property</span></span>|<span data-ttu-id="46b25-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46b25-130">Type</span></span>|<span data-ttu-id="46b25-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46b25-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46b25-132">id</span><span class="sxs-lookup"><span data-stu-id="46b25-132">id</span></span>|<span data-ttu-id="46b25-133">String</span><span class="sxs-lookup"><span data-stu-id="46b25-133">String</span></span>|<span data-ttu-id="46b25-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="46b25-134">The GUID for the object</span></span>|
|<span data-ttu-id="46b25-135">Деплойментпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="46b25-135">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="46b25-136">Виндовсаутопилотпрофилеассигнментстатус</span><span class="sxs-lookup"><span data-stu-id="46b25-136">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="46b25-137">Состояние назначения профиля устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-137">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="46b25-138">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="46b25-138">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="46b25-139">Деплойментпрофилеассигнментдетаиледстатус</span><span class="sxs-lookup"><span data-stu-id="46b25-139">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="46b25-140">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="46b25-140">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="46b25-141">Подробное состояние назначения профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-141">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="46b25-142">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="46b25-142">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="46b25-143">Деплойментпрофилеассигнеддатетиме</span><span class="sxs-lookup"><span data-stu-id="46b25-143">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="46b25-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46b25-144">DateTimeOffset</span></span>|<span data-ttu-id="46b25-145">Время настройки профиля для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-145">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-146">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="46b25-146">orderIdentifier</span></span>|<span data-ttu-id="46b25-147">String</span><span class="sxs-lookup"><span data-stu-id="46b25-147">String</span></span>|<span data-ttu-id="46b25-148">Идентификатор заказа устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-148">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-149">Пурчасеордеридентифиер</span><span class="sxs-lookup"><span data-stu-id="46b25-149">purchaseOrderIdentifier</span></span>|<span data-ttu-id="46b25-150">String</span><span class="sxs-lookup"><span data-stu-id="46b25-150">String</span></span>|<span data-ttu-id="46b25-151">Идентификатор заказа на покупку для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-151">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-152">serialNumber</span><span class="sxs-lookup"><span data-stu-id="46b25-152">serialNumber</span></span>|<span data-ttu-id="46b25-153">String</span><span class="sxs-lookup"><span data-stu-id="46b25-153">String</span></span>|<span data-ttu-id="46b25-154">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="46b25-154">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-155">productKey</span><span class="sxs-lookup"><span data-stu-id="46b25-155">productKey</span></span>|<span data-ttu-id="46b25-156">Строка</span><span class="sxs-lookup"><span data-stu-id="46b25-156">String</span></span>|<span data-ttu-id="46b25-157">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="46b25-157">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-158">manufacturer</span><span class="sxs-lookup"><span data-stu-id="46b25-158">manufacturer</span></span>|<span data-ttu-id="46b25-159">String</span><span class="sxs-lookup"><span data-stu-id="46b25-159">String</span></span>|<span data-ttu-id="46b25-160">OEM-производитель устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-160">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-161">model</span><span class="sxs-lookup"><span data-stu-id="46b25-161">model</span></span>|<span data-ttu-id="46b25-162">String</span><span class="sxs-lookup"><span data-stu-id="46b25-162">String</span></span>|<span data-ttu-id="46b25-163">Имя модели для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-163">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-164">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="46b25-164">enrollmentState</span></span>|[<span data-ttu-id="46b25-165">Енроллментстате</span><span class="sxs-lookup"><span data-stu-id="46b25-165">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="46b25-166">Состояние регистрации в Intune для устройства автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-166">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="46b25-167">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="46b25-167">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="46b25-168">Ластконтактеддатетиме</span><span class="sxs-lookup"><span data-stu-id="46b25-168">lastContactedDateTime</span></span>|<span data-ttu-id="46b25-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46b25-169">DateTimeOffset</span></span>|<span data-ttu-id="46b25-170">Дата и время последнего обращения в Intune к устройству автопилота Windows.</span><span class="sxs-lookup"><span data-stu-id="46b25-170">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="46b25-171">Аддрессаблеусернаме</span><span class="sxs-lookup"><span data-stu-id="46b25-171">addressableUserName</span></span>|<span data-ttu-id="46b25-172">String</span><span class="sxs-lookup"><span data-stu-id="46b25-172">String</span></span>|<span data-ttu-id="46b25-173">Имя пользователя с адресом.</span><span class="sxs-lookup"><span data-stu-id="46b25-173">Addressable user name.</span></span>|
|<span data-ttu-id="46b25-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46b25-174">userPrincipalName</span></span>|<span data-ttu-id="46b25-175">String</span><span class="sxs-lookup"><span data-stu-id="46b25-175">String</span></span>|<span data-ttu-id="46b25-176">Имя участника пользователя.</span><span class="sxs-lookup"><span data-stu-id="46b25-176">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="46b25-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="46b25-177">Response</span></span>
<span data-ttu-id="46b25-178">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46b25-178">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b25-179">Пример</span><span class="sxs-lookup"><span data-stu-id="46b25-179">Example</span></span>

### <a name="request"></a><span data-ttu-id="46b25-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="46b25-180">Request</span></span>
<span data-ttu-id="46b25-181">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46b25-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities
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

### <a name="response"></a><span data-ttu-id="46b25-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="46b25-182">Response</span></span>
<span data-ttu-id="46b25-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46b25-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




