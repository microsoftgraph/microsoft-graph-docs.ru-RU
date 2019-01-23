---
title: Создание windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9d9287738b33b1afe55a3f22c441b888ae7d77b4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406397"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="7f94f-103">Создание windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7f94f-103">Create windowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="7f94f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f94f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7f94f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f94f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f94f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f94f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f94f-107">Создание нового объекта [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="7f94f-107">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f94f-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="7f94f-108">Prerequisites</span></span>
<span data-ttu-id="7f94f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7f94f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f94f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f94f-111">Permission type</span></span>|<span data-ttu-id="7f94f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f94f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f94f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f94f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f94f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f94f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f94f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f94f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f94f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f94f-116">Not supported.</span></span>|
|<span data-ttu-id="7f94f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f94f-117">Application</span></span>|<span data-ttu-id="7f94f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f94f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f94f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f94f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices
```

## <a name="request-headers"></a><span data-ttu-id="7f94f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f94f-120">Request headers</span></span>
|<span data-ttu-id="7f94f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f94f-121">Header</span></span>|<span data-ttu-id="7f94f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f94f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f94f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f94f-123">Authorization</span></span>|<span data-ttu-id="7f94f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f94f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f94f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f94f-125">Accept</span></span>|<span data-ttu-id="7f94f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f94f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f94f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f94f-127">Request body</span></span>
<span data-ttu-id="7f94f-128">В тексте запроса укажите представление JSON для объекта windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="7f94f-128">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="7f94f-129">В следующей таблице показаны свойства, которые необходимы для создания windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="7f94f-129">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="7f94f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f94f-130">Property</span></span>|<span data-ttu-id="7f94f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f94f-131">Type</span></span>|<span data-ttu-id="7f94f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f94f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f94f-133">id</span><span class="sxs-lookup"><span data-stu-id="7f94f-133">id</span></span>|<span data-ttu-id="7f94f-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7f94f-134">String</span></span>|<span data-ttu-id="7f94f-135">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="7f94f-135">The GUID for the object</span></span>|
|<span data-ttu-id="7f94f-136">deploymentProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="7f94f-136">deploymentProfileAssignmentStatus</span></span>|[<span data-ttu-id="7f94f-137">windowsAutopilotProfileAssignmentStatus</span><span class="sxs-lookup"><span data-stu-id="7f94f-137">windowsAutopilotProfileAssignmentStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|<span data-ttu-id="7f94f-138">Состояние назначения профиля устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-138">Profile assignment status of the Windows autopilot device.</span></span> <span data-ttu-id="7f94f-139">Возможные значения: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="7f94f-139">Possible values are: `unknown`, `assignedInSync`, `assignedOutOfSync`, `assignedUnkownSyncState`, `notAssigned`, `pending`, `failed`.</span></span>|
|<span data-ttu-id="7f94f-140">deploymentProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="7f94f-140">deploymentProfileAssignmentDetailedStatus</span></span>|[<span data-ttu-id="7f94f-141">windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="7f94f-141">windowsAutopilotProfileAssignmentDetailedStatus</span></span>](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|<span data-ttu-id="7f94f-142">Назначение профиля подробное описание состояния устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-142">Profile assignment detailed status of the Windows autopilot device.</span></span> <span data-ttu-id="7f94f-143">Возможные значения: `none`, `hardwareRequirementsNotMet`.</span><span class="sxs-lookup"><span data-stu-id="7f94f-143">Possible values are: `none`, `hardwareRequirementsNotMet`.</span></span>|
|<span data-ttu-id="7f94f-144">deploymentProfileAssignedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f94f-144">deploymentProfileAssignedDateTime</span></span>|<span data-ttu-id="7f94f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f94f-145">DateTimeOffset</span></span>|<span data-ttu-id="7f94f-146">Профиль задания времени автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-146">Profile set time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-147">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f94f-147">orderIdentifier</span></span>|<span data-ttu-id="7f94f-148">Строка</span><span class="sxs-lookup"><span data-stu-id="7f94f-148">String</span></span>|<span data-ttu-id="7f94f-149">Порядок идентификатор устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-149">Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-150">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f94f-150">purchaseOrderIdentifier</span></span>|<span data-ttu-id="7f94f-151">String</span><span class="sxs-lookup"><span data-stu-id="7f94f-151">String</span></span>|<span data-ttu-id="7f94f-152">Идентификатор заказа на покупку автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-152">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-153">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7f94f-153">serialNumber</span></span>|<span data-ttu-id="7f94f-154">Строка</span><span class="sxs-lookup"><span data-stu-id="7f94f-154">String</span></span>|<span data-ttu-id="7f94f-155">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7f94f-155">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-156">productKey</span><span class="sxs-lookup"><span data-stu-id="7f94f-156">productKey</span></span>|<span data-ttu-id="7f94f-157">Строка</span><span class="sxs-lookup"><span data-stu-id="7f94f-157">String</span></span>|<span data-ttu-id="7f94f-158">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="7f94f-158">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-159">manufacturer</span><span class="sxs-lookup"><span data-stu-id="7f94f-159">manufacturer</span></span>|<span data-ttu-id="7f94f-160">String</span><span class="sxs-lookup"><span data-stu-id="7f94f-160">String</span></span>|<span data-ttu-id="7f94f-161">Изготовителей автопилот устройства Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-161">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-162">model</span><span class="sxs-lookup"><span data-stu-id="7f94f-162">model</span></span>|<span data-ttu-id="7f94f-163">String</span><span class="sxs-lookup"><span data-stu-id="7f94f-163">String</span></span>|<span data-ttu-id="7f94f-164">Имя модели устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-164">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-165">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7f94f-165">enrollmentState</span></span>|[<span data-ttu-id="7f94f-166">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7f94f-166">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7f94f-167">Состояние регистрации автопилот устройства Windows Intune.</span><span class="sxs-lookup"><span data-stu-id="7f94f-167">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="7f94f-168">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="7f94f-168">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7f94f-169">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f94f-169">lastContactedDateTime</span></span>|<span data-ttu-id="7f94f-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f94f-170">DateTimeOffset</span></span>|<span data-ttu-id="7f94f-171">Intune связаться с даты последнего устройства автопилот Windows.</span><span class="sxs-lookup"><span data-stu-id="7f94f-171">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f94f-172">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="7f94f-172">addressableUserName</span></span>|<span data-ttu-id="7f94f-173">String</span><span class="sxs-lookup"><span data-stu-id="7f94f-173">String</span></span>|<span data-ttu-id="7f94f-174">Имя адресации пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f94f-174">Addressable user name.</span></span>|
|<span data-ttu-id="7f94f-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f94f-175">userPrincipalName</span></span>|<span data-ttu-id="7f94f-176">String</span><span class="sxs-lookup"><span data-stu-id="7f94f-176">String</span></span>|<span data-ttu-id="7f94f-177">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f94f-177">User Principal Name.</span></span>|



## <a name="response"></a><span data-ttu-id="7f94f-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f94f-178">Response</span></span>
<span data-ttu-id="7f94f-179">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7f94f-179">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f94f-180">Пример</span><span class="sxs-lookup"><span data-stu-id="7f94f-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f94f-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f94f-181">Request</span></span>
<span data-ttu-id="7f94f-182">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f94f-182">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f94f-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f94f-183">Response</span></span>
<span data-ttu-id="7f94f-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f94f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




