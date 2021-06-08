---
title: Создание managedDeviceMobileAppConfigurationDeviceStatus
description: Создание нового объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f7075b3946fbad099f11bed2df109815ac6ffd82
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759877"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="1c59f-103">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="1c59f-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="1c59f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c59f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c59f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c59f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c59f-106">Создание нового [объекта managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="1c59f-106">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c59f-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1c59f-107">Prerequisites</span></span>
<span data-ttu-id="1c59f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1c59f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c59f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1c59f-110">Permission type</span></span>|<span data-ttu-id="1c59f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1c59f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c59f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1c59f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c59f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c59f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1c59f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1c59f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c59f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c59f-115">Not supported.</span></span>|
|<span data-ttu-id="1c59f-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1c59f-116">Application</span></span>|<span data-ttu-id="1c59f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1c59f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c59f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1c59f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1c59f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1c59f-119">Request headers</span></span>
|<span data-ttu-id="1c59f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1c59f-120">Header</span></span>|<span data-ttu-id="1c59f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1c59f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c59f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c59f-122">Authorization</span></span>|<span data-ttu-id="1c59f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1c59f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c59f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1c59f-124">Accept</span></span>|<span data-ttu-id="1c59f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1c59f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c59f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1c59f-126">Request body</span></span>
<span data-ttu-id="1c59f-127">В теле запроса поставляем представление JSON для объекта managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="1c59f-127">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="1c59f-128">В следующей таблице показаны свойства, необходимые при создании управляемогоDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="1c59f-128">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="1c59f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c59f-129">Property</span></span>|<span data-ttu-id="1c59f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1c59f-130">Type</span></span>|<span data-ttu-id="1c59f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1c59f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c59f-132">id</span><span class="sxs-lookup"><span data-stu-id="1c59f-132">id</span></span>|<span data-ttu-id="1c59f-133">String</span><span class="sxs-lookup"><span data-stu-id="1c59f-133">String</span></span>|<span data-ttu-id="1c59f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1c59f-134">Key of the entity.</span></span>|
|<span data-ttu-id="1c59f-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="1c59f-135">deviceDisplayName</span></span>|<span data-ttu-id="1c59f-136">String</span><span class="sxs-lookup"><span data-stu-id="1c59f-136">String</span></span>|<span data-ttu-id="1c59f-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="1c59f-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="1c59f-138">userName</span><span class="sxs-lookup"><span data-stu-id="1c59f-138">userName</span></span>|<span data-ttu-id="1c59f-139">String</span><span class="sxs-lookup"><span data-stu-id="1c59f-139">String</span></span>|<span data-ttu-id="1c59f-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="1c59f-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="1c59f-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1c59f-141">deviceModel</span></span>|<span data-ttu-id="1c59f-142">String</span><span class="sxs-lookup"><span data-stu-id="1c59f-142">String</span></span>|<span data-ttu-id="1c59f-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="1c59f-143">The device model that is being reported</span></span>|
|<span data-ttu-id="1c59f-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1c59f-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1c59f-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c59f-145">DateTimeOffset</span></span>|<span data-ttu-id="1c59f-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="1c59f-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1c59f-147">status</span><span class="sxs-lookup"><span data-stu-id="1c59f-147">status</span></span>|[<span data-ttu-id="1c59f-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1c59f-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1c59f-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="1c59f-149">Compliance status of the policy report.</span></span> <span data-ttu-id="1c59f-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="1c59f-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1c59f-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="1c59f-151">lastReportedDateTime</span></span>|<span data-ttu-id="1c59f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1c59f-152">DateTimeOffset</span></span>|<span data-ttu-id="1c59f-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="1c59f-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="1c59f-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1c59f-154">userPrincipalName</span></span>|<span data-ttu-id="1c59f-155">String</span><span class="sxs-lookup"><span data-stu-id="1c59f-155">String</span></span>|<span data-ttu-id="1c59f-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c59f-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="1c59f-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="1c59f-157">Response</span></span>
<span data-ttu-id="1c59f-158">В случае успешной работы этот метод возвращает код отклика и объект `201 Created` [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1c59f-158">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c59f-159">Пример</span><span class="sxs-lookup"><span data-stu-id="1c59f-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c59f-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="1c59f-160">Request</span></span>
<span data-ttu-id="1c59f-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1c59f-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1c59f-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1c59f-162">Response</span></span>
<span data-ttu-id="1c59f-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1c59f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




