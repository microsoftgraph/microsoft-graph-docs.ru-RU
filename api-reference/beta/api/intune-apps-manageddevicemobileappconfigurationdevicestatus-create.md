---
title: Создание managedDeviceMobileAppConfigurationDeviceStatus
description: Создание нового объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae574c44c4cf9cc3d40ce4dbe9b03667a6cbc376
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34974834"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="bf9e5-103">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="bf9e5-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="bf9e5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf9e5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf9e5-106">Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="bf9e5-106">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf9e5-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="bf9e5-107">Prerequisites</span></span>
<span data-ttu-id="bf9e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf9e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf9e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf9e5-110">Permission type</span></span>|<span data-ttu-id="bf9e5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf9e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf9e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf9e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bf9e5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf9e5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bf9e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf9e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf9e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-115">Not supported.</span></span>|
|<span data-ttu-id="bf9e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf9e5-116">Application</span></span>|<span data-ttu-id="bf9e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf9e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf9e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bf9e5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf9e5-119">Request headers</span></span>
|<span data-ttu-id="bf9e5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf9e5-120">Header</span></span>|<span data-ttu-id="bf9e5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bf9e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf9e5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf9e5-122">Authorization</span></span>|<span data-ttu-id="bf9e5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf9e5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bf9e5-124">Accept</span></span>|<span data-ttu-id="bf9e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf9e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf9e5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf9e5-126">Request body</span></span>
<span data-ttu-id="bf9e5-127">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="bf9e5-128">В следующей таблице приведены свойства, необходимые при создании managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="bf9e5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf9e5-129">Property</span></span>|<span data-ttu-id="bf9e5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bf9e5-130">Type</span></span>|<span data-ttu-id="bf9e5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bf9e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf9e5-132">id</span><span class="sxs-lookup"><span data-stu-id="bf9e5-132">id</span></span>|<span data-ttu-id="bf9e5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="bf9e5-133">String</span></span>|<span data-ttu-id="bf9e5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-134">Key of the entity.</span></span>|
|<span data-ttu-id="bf9e5-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf9e5-135">deviceDisplayName</span></span>|<span data-ttu-id="bf9e5-136">String</span><span class="sxs-lookup"><span data-stu-id="bf9e5-136">String</span></span>|<span data-ttu-id="bf9e5-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="bf9e5-138">userName</span><span class="sxs-lookup"><span data-stu-id="bf9e5-138">userName</span></span>|<span data-ttu-id="bf9e5-139">String</span><span class="sxs-lookup"><span data-stu-id="bf9e5-139">String</span></span>|<span data-ttu-id="bf9e5-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="bf9e5-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="bf9e5-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bf9e5-141">deviceModel</span></span>|<span data-ttu-id="bf9e5-142">String</span><span class="sxs-lookup"><span data-stu-id="bf9e5-142">String</span></span>|<span data-ttu-id="bf9e5-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="bf9e5-143">The device model that is being reported</span></span>|
|<span data-ttu-id="bf9e5-144">platform</span><span class="sxs-lookup"><span data-stu-id="bf9e5-144">platform</span></span>|<span data-ttu-id="bf9e5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="bf9e5-145">Int32</span></span>|<span data-ttu-id="bf9e5-146">Платформа для устройства, о котором сообщается</span><span class="sxs-lookup"><span data-stu-id="bf9e5-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="bf9e5-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9e5-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bf9e5-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9e5-148">DateTimeOffset</span></span>|<span data-ttu-id="bf9e5-149">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bf9e5-150">status</span><span class="sxs-lookup"><span data-stu-id="bf9e5-150">status</span></span>|[<span data-ttu-id="bf9e5-151">Комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="bf9e5-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bf9e5-152">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-152">Compliance status of the policy report.</span></span> <span data-ttu-id="bf9e5-153">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bf9e5-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf9e5-154">lastReportedDateTime</span></span>|<span data-ttu-id="bf9e5-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf9e5-155">DateTimeOffset</span></span>|<span data-ttu-id="bf9e5-156">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="bf9e5-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bf9e5-157">userPrincipalName</span></span>|<span data-ttu-id="bf9e5-158">String</span><span class="sxs-lookup"><span data-stu-id="bf9e5-158">String</span></span>|<span data-ttu-id="bf9e5-159">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="bf9e5-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="bf9e5-160">Response</span></span>
<span data-ttu-id="bf9e5-161">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-161">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf9e5-162">Пример</span><span class="sxs-lookup"><span data-stu-id="bf9e5-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf9e5-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf9e5-163">Request</span></span>
<span data-ttu-id="bf9e5-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="bf9e5-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf9e5-165">Response</span></span>
<span data-ttu-id="bf9e5-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf9e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```





