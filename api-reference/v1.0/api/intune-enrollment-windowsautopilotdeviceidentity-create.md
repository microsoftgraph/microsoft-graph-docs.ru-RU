---
title: Создание объекта windowsAutopilotDeviceIdentity
description: Создание нового объекта windowsAutopilotDeviceIdentity.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7ee59ca45db337f85f1c4f0f01443c2c0965e1c0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753394"
---
# <a name="create-windowsautopilotdeviceidentity"></a><span data-ttu-id="dd32a-103">Создание объекта windowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="dd32a-103">Create windowsAutopilotDeviceIdentity</span></span>

<span data-ttu-id="dd32a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd32a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd32a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dd32a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd32a-106">Создание нового [объекта windowsAutopilotDeviceIdentity.](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="dd32a-106">Create a new [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd32a-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dd32a-107">Prerequisites</span></span>
<span data-ttu-id="dd32a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd32a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd32a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dd32a-110">Permission type</span></span>|<span data-ttu-id="dd32a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dd32a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd32a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dd32a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dd32a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd32a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dd32a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dd32a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd32a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dd32a-115">Not supported.</span></span>|
|<span data-ttu-id="dd32a-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="dd32a-116">Application</span></span>|<span data-ttu-id="dd32a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd32a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd32a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dd32a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="dd32a-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dd32a-119">Request headers</span></span>
|<span data-ttu-id="dd32a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dd32a-120">Header</span></span>|<span data-ttu-id="dd32a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dd32a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd32a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd32a-122">Authorization</span></span>|<span data-ttu-id="dd32a-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dd32a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd32a-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dd32a-124">Accept</span></span>|<span data-ttu-id="dd32a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dd32a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd32a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dd32a-126">Request body</span></span>
<span data-ttu-id="dd32a-127">В теле запроса поставляем представление JSON для объекта windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="dd32a-127">In the request body, supply a JSON representation for the windowsAutopilotDeviceIdentity object.</span></span>

<span data-ttu-id="dd32a-128">В следующей таблице показаны свойства, необходимые при создании объекта windowsAutopilotDeviceIdentity.</span><span class="sxs-lookup"><span data-stu-id="dd32a-128">The following table shows the properties that are required when you create the windowsAutopilotDeviceIdentity.</span></span>

|<span data-ttu-id="dd32a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd32a-129">Property</span></span>|<span data-ttu-id="dd32a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dd32a-130">Type</span></span>|<span data-ttu-id="dd32a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dd32a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd32a-132">id</span><span class="sxs-lookup"><span data-stu-id="dd32a-132">id</span></span>|<span data-ttu-id="dd32a-133">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-133">String</span></span>|<span data-ttu-id="dd32a-134">GUID объекта</span><span class="sxs-lookup"><span data-stu-id="dd32a-134">The GUID for the object</span></span>|
|<span data-ttu-id="dd32a-135">groupTag</span><span class="sxs-lookup"><span data-stu-id="dd32a-135">groupTag</span></span>|<span data-ttu-id="dd32a-136">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-136">String</span></span>|<span data-ttu-id="dd32a-137">Тег группы устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-137">Group Tag of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-138">purchaseOrderIdentifier</span><span class="sxs-lookup"><span data-stu-id="dd32a-138">purchaseOrderIdentifier</span></span>|<span data-ttu-id="dd32a-139">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-139">String</span></span>|<span data-ttu-id="dd32a-140">Покупка идентификатора заказа устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-140">Purchase Order Identifier of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-141">serialNumber</span><span class="sxs-lookup"><span data-stu-id="dd32a-141">serialNumber</span></span>|<span data-ttu-id="dd32a-142">Строка</span><span class="sxs-lookup"><span data-stu-id="dd32a-142">String</span></span>|<span data-ttu-id="dd32a-143">Серийный номер устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="dd32a-143">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-144">productKey</span><span class="sxs-lookup"><span data-stu-id="dd32a-144">productKey</span></span>|<span data-ttu-id="dd32a-145">Строка</span><span class="sxs-lookup"><span data-stu-id="dd32a-145">String</span></span>|<span data-ttu-id="dd32a-146">Ключ продукта устройства Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="dd32a-146">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-147">manufacturer</span><span class="sxs-lookup"><span data-stu-id="dd32a-147">manufacturer</span></span>|<span data-ttu-id="dd32a-148">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-148">String</span></span>|<span data-ttu-id="dd32a-149">Oem производитель устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-149">Oem manufacturer of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-150">model</span><span class="sxs-lookup"><span data-stu-id="dd32a-150">model</span></span>|<span data-ttu-id="dd32a-151">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-151">String</span></span>|<span data-ttu-id="dd32a-152">Имя модели устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-152">Model name of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="dd32a-153">enrollmentState</span></span>|[<span data-ttu-id="dd32a-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="dd32a-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="dd32a-155">Состояние регистрации intune устройства Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-155">Intune enrollment state of the Windows autopilot device.</span></span> <span data-ttu-id="dd32a-156">Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.</span><span class="sxs-lookup"><span data-stu-id="dd32a-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`.</span></span>|
|<span data-ttu-id="dd32a-157">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd32a-157">lastContactedDateTime</span></span>|<span data-ttu-id="dd32a-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd32a-158">DateTimeOffset</span></span>|<span data-ttu-id="dd32a-159">Intune Last Contacted Date Time of the Windows автопилота.</span><span class="sxs-lookup"><span data-stu-id="dd32a-159">Intune Last Contacted Date Time of the Windows autopilot device.</span></span>|
|<span data-ttu-id="dd32a-160">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="dd32a-160">addressableUserName</span></span>|<span data-ttu-id="dd32a-161">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-161">String</span></span>|<span data-ttu-id="dd32a-162">Адресное имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd32a-162">Addressable user name.</span></span>|
|<span data-ttu-id="dd32a-163">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dd32a-163">userPrincipalName</span></span>|<span data-ttu-id="dd32a-164">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-164">String</span></span>|<span data-ttu-id="dd32a-165">Имя главного пользователя.</span><span class="sxs-lookup"><span data-stu-id="dd32a-165">User Principal Name.</span></span>|
|<span data-ttu-id="dd32a-166">resourceName</span><span class="sxs-lookup"><span data-stu-id="dd32a-166">resourceName</span></span>|<span data-ttu-id="dd32a-167">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-167">String</span></span>|<span data-ttu-id="dd32a-168">Имя ресурса.</span><span class="sxs-lookup"><span data-stu-id="dd32a-168">Resource Name.</span></span>|
|<span data-ttu-id="dd32a-169">skuNumber</span><span class="sxs-lookup"><span data-stu-id="dd32a-169">skuNumber</span></span>|<span data-ttu-id="dd32a-170">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-170">String</span></span>|<span data-ttu-id="dd32a-171">Номер SKU</span><span class="sxs-lookup"><span data-stu-id="dd32a-171">SKU Number</span></span>|
|<span data-ttu-id="dd32a-172">systemFamily</span><span class="sxs-lookup"><span data-stu-id="dd32a-172">systemFamily</span></span>|<span data-ttu-id="dd32a-173">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-173">String</span></span>|<span data-ttu-id="dd32a-174">Семейство system</span><span class="sxs-lookup"><span data-stu-id="dd32a-174">System Family</span></span>|
|<span data-ttu-id="dd32a-175">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="dd32a-175">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="dd32a-176">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-176">String</span></span>|<span data-ttu-id="dd32a-177">AAD Device ID - to be deprecated</span><span class="sxs-lookup"><span data-stu-id="dd32a-177">AAD Device ID - to be deprecated</span></span>|
|<span data-ttu-id="dd32a-178">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="dd32a-178">managedDeviceId</span></span>|<span data-ttu-id="dd32a-179">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-179">String</span></span>|<span data-ttu-id="dd32a-180">Управляемый ID устройства</span><span class="sxs-lookup"><span data-stu-id="dd32a-180">Managed Device ID</span></span>|
|<span data-ttu-id="dd32a-181">displayName</span><span class="sxs-lookup"><span data-stu-id="dd32a-181">displayName</span></span>|<span data-ttu-id="dd32a-182">String</span><span class="sxs-lookup"><span data-stu-id="dd32a-182">String</span></span>|<span data-ttu-id="dd32a-183">"Display Name" (Отображаемое имя);</span><span class="sxs-lookup"><span data-stu-id="dd32a-183">Display Name</span></span>|



## <a name="response"></a><span data-ttu-id="dd32a-184">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd32a-184">Response</span></span>
<span data-ttu-id="dd32a-185">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="dd32a-185">If successful, this method returns a `201 Created` response code and a [windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd32a-186">Пример</span><span class="sxs-lookup"><span data-stu-id="dd32a-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd32a-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="dd32a-187">Request</span></span>
<span data-ttu-id="dd32a-188">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dd32a-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
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
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="dd32a-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="dd32a-189">Response</span></span>
<span data-ttu-id="dd32a-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dd32a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "fac6f0b1-f0b1-fac6-b1f0-c6fab1f0c6fa",
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
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value"
}
```




