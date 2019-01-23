---
title: Обновление windowsAutopilotDeviceIdentity
description: Обновление свойства объекта windowsAutopilotDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 018b45712ce7a35d2b7a19a09bca7ea7dd1650d7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423869"
---
# <a name="update-windowsautopilotdeviceidentity"></a><span data-ttu-id="07d86-103">Обновление windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="07d86-103">Update windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="07d86-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07d86-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07d86-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07d86-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07d86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d86-107">Обновление свойства объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="07d86-107">Update the properties of a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07d86-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="07d86-108">Prerequisites</span></span>
<span data-ttu-id="07d86-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="07d86-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07d86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07d86-111">Permission type</span></span>|<span data-ttu-id="07d86-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="07d86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07d86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07d86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07d86-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07d86-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="07d86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07d86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07d86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d86-116">Not supported.</span></span>|
|<span data-ttu-id="07d86-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="07d86-117">Application</span></span>|<span data-ttu-id="07d86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07d86-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07d86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07d86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}
PATCH /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="07d86-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="07d86-120">Request headers</span></span>
|<span data-ttu-id="07d86-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07d86-121">Header</span></span>|<span data-ttu-id="07d86-122">Значение</span><span class="sxs-lookup"><span data-stu-id="07d86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07d86-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="07d86-123">Authorization</span></span>|<span data-ttu-id="07d86-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="07d86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07d86-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07d86-125">Accept</span></span>|<span data-ttu-id="07d86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07d86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07d86-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07d86-127">Request body</span></span>
<span data-ttu-id="07d86-128">В тексте запроса укажите представление JSON для объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="07d86-128">In the request body, supply a JSON representation for the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

<span data-ttu-id="07d86-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="07d86-129">The following table shows the properties that are required when you create the [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md).</span></span>

|<span data-ttu-id="07d86-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="07d86-130">Property</span></span>|<span data-ttu-id="07d86-131">Тип</span><span class="sxs-lookup"><span data-stu-id="07d86-131">Type</span></span>|<span data-ttu-id="07d86-132">Описание</span><span class="sxs-lookup"><span data-stu-id="07d86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d86-133">id</span><span class="sxs-lookup"><span data-stu-id="07d86-133">id</span></span>|<span data-ttu-id="07d86-134">Строка</span><span class="sxs-lookup"><span data-stu-id="07d86-134">String</span></span>|<span data-ttu-id="07d86-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="07d86-135">The GUID for the object</span></span>|
|<span data-ttu-id="07d86-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="07d86-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="07d86-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="07d86-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="07d86-138">Состояние назначения профиля устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="07d86-139">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="07d86-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="07d86-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="07d86-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="07d86-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="07d86-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="07d86-142">Назначение профиля подробное описание состояния устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="07d86-143">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="07d86-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="07d86-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="07d86-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="07d86-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d86-145">DateTimeOffset</span></span>|<span data-ttu-id="07d86-146">Профиль задания времени автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="07d86-147">orderIdentifier</span></span>|<span data-ttu-id="07d86-148">Строка</span><span class="sxs-lookup"><span data-stu-id="07d86-148">String</span></span>|<span data-ttu-id="07d86-149">Порядок идентификатор устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="07d86-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="07d86-151">String</span><span class="sxs-lookup"><span data-stu-id="07d86-151">String</span></span>|<span data-ttu-id="07d86-152">Идентификатор заказа на покупку автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="07d86-153">serialNumber</span></span>|<span data-ttu-id="07d86-154">Строка</span><span class="sxs-lookup"><span data-stu-id="07d86-154">String</span></span>|<span data-ttu-id="07d86-155">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="07d86-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-156">productKey</span><span class="sxs-lookup"><span data-stu-id="07d86-156">productKey</span></span>|<span data-ttu-id="07d86-157">Строка</span><span class="sxs-lookup"><span data-stu-id="07d86-157">String</span></span>|<span data-ttu-id="07d86-158">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="07d86-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="07d86-159">manufacturer</span></span>|<span data-ttu-id="07d86-160">String</span><span class="sxs-lookup"><span data-stu-id="07d86-160">String</span></span>|<span data-ttu-id="07d86-161">Изготовителей автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-162">model</span><span class="sxs-lookup"><span data-stu-id="07d86-162">model</span></span>|<span data-ttu-id="07d86-163">String</span><span class="sxs-lookup"><span data-stu-id="07d86-163">String</span></span>|<span data-ttu-id="07d86-164">Имя модели устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="07d86-165">enrollmentState</span></span>|[<span data-ttu-id="07d86-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="07d86-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="07d86-167">Состояние регистрации автопилот устройства Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="07d86-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="07d86-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="07d86-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="07d86-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="07d86-169">lastContactedDateTime</span></span>|<span data-ttu-id="07d86-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07d86-170">DateTimeOffset</span></span>|<span data-ttu-id="07d86-171">Intune связаться с даты последнего устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="07d86-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="07d86-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="07d86-172">addressableUserName</span></span>|<span data-ttu-id="07d86-173">String</span><span class="sxs-lookup"><span data-stu-id="07d86-173">String</span></span>|<span data-ttu-id="07d86-174">Имя адресации пользователя.</span><span class="sxs-lookup"><span data-stu-id="07d86-174">Addressable user name.</span></span>|
|<span data-ttu-id="07d86-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="07d86-175">userPrincipalName</span></span>|<span data-ttu-id="07d86-176">String</span><span class="sxs-lookup"><span data-stu-id="07d86-176">String</span></span>|<span data-ttu-id="07d86-177">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="07d86-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="07d86-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d86-178">Response</span></span>
<span data-ttu-id="07d86-179">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="07d86-179">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07d86-180">Пример</span><span class="sxs-lookup"><span data-stu-id="07d86-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="07d86-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="07d86-181">Request</span></span>
<span data-ttu-id="07d86-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07d86-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07d86-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="07d86-183">Response</span></span>
<span data-ttu-id="07d86-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="07d86-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




