---
title: Создание managedDeviceMobileAppConfigurationDeviceStatus
description: Создание нового объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff1f335fcc439578fc97aa9884c470a5fb97c9b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516309"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="a4095-103">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a4095-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="a4095-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a4095-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a4095-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4095-106">Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="a4095-106">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4095-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4095-107">Prerequisites</span></span>
<span data-ttu-id="a4095-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4095-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4095-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4095-110">Permission type</span></span>|<span data-ttu-id="a4095-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4095-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4095-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4095-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a4095-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4095-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4095-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4095-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4095-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4095-115">Not supported.</span></span>|
|<span data-ttu-id="a4095-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4095-116">Application</span></span>|<span data-ttu-id="a4095-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4095-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4095-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4095-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a4095-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a4095-119">Request headers</span></span>
|<span data-ttu-id="a4095-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4095-120">Header</span></span>|<span data-ttu-id="a4095-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a4095-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4095-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4095-122">Authorization</span></span>|<span data-ttu-id="a4095-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4095-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4095-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a4095-124">Accept</span></span>|<span data-ttu-id="a4095-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a4095-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4095-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a4095-126">Request body</span></span>
<span data-ttu-id="a4095-127">В тексте запроса добавьте представление объекта managedDeviceMobileAppConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4095-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="a4095-128">В следующей таблице приведены свойства, необходимые при создании managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="a4095-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="a4095-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4095-129">Property</span></span>|<span data-ttu-id="a4095-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a4095-130">Type</span></span>|<span data-ttu-id="a4095-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a4095-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4095-132">id</span><span class="sxs-lookup"><span data-stu-id="a4095-132">id</span></span>|<span data-ttu-id="a4095-133">Строка</span><span class="sxs-lookup"><span data-stu-id="a4095-133">String</span></span>|<span data-ttu-id="a4095-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a4095-134">Key of the entity.</span></span>|
|<span data-ttu-id="a4095-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a4095-135">deviceDisplayName</span></span>|<span data-ttu-id="a4095-136">Строка</span><span class="sxs-lookup"><span data-stu-id="a4095-136">String</span></span>|<span data-ttu-id="a4095-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a4095-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a4095-138">userName</span><span class="sxs-lookup"><span data-stu-id="a4095-138">userName</span></span>|<span data-ttu-id="a4095-139">Строка</span><span class="sxs-lookup"><span data-stu-id="a4095-139">String</span></span>|<span data-ttu-id="a4095-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="a4095-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="a4095-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a4095-141">deviceModel</span></span>|<span data-ttu-id="a4095-142">String</span><span class="sxs-lookup"><span data-stu-id="a4095-142">String</span></span>|<span data-ttu-id="a4095-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="a4095-143">The device model that is being reported</span></span>|
|<span data-ttu-id="a4095-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a4095-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a4095-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4095-145">DateTimeOffset</span></span>|<span data-ttu-id="a4095-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="a4095-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a4095-147">status</span><span class="sxs-lookup"><span data-stu-id="a4095-147">status</span></span>|[<span data-ttu-id="a4095-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="a4095-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a4095-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a4095-149">Compliance status of the policy report.</span></span> <span data-ttu-id="a4095-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a4095-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a4095-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4095-151">lastReportedDateTime</span></span>|<span data-ttu-id="a4095-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4095-152">DateTimeOffset</span></span>|<span data-ttu-id="a4095-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="a4095-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a4095-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a4095-154">userPrincipalName</span></span>|<span data-ttu-id="a4095-155">String</span><span class="sxs-lookup"><span data-stu-id="a4095-155">String</span></span>|<span data-ttu-id="a4095-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="a4095-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a4095-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4095-157">Response</span></span>
<span data-ttu-id="a4095-158">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a4095-158">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4095-159">Пример</span><span class="sxs-lookup"><span data-stu-id="a4095-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4095-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4095-160">Request</span></span>
<span data-ttu-id="a4095-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4095-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="a4095-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4095-162">Response</span></span>
<span data-ttu-id="a4095-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4095-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




