---
title: Обновление объекта deviceConfigurationDeviceStatus
description: Обновление свойств объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e12d6a531f032ba422c4b080878106a97eb44562
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450672"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="86af4-103">Обновление объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="86af4-103">Update deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="86af4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86af4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86af4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="86af4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86af4-106">Обновление свойств объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="86af4-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86af4-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="86af4-107">Prerequisites</span></span>
<span data-ttu-id="86af4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86af4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86af4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86af4-110">Permission type</span></span>|<span data-ttu-id="86af4-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="86af4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86af4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86af4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86af4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86af4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="86af4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86af4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86af4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86af4-115">Not supported.</span></span>|
|<span data-ttu-id="86af4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86af4-116">Application</span></span>|<span data-ttu-id="86af4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86af4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86af4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86af4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="86af4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="86af4-119">Request headers</span></span>
|<span data-ttu-id="86af4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86af4-120">Header</span></span>|<span data-ttu-id="86af4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="86af4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86af4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86af4-122">Authorization</span></span>|<span data-ttu-id="86af4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86af4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86af4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="86af4-124">Accept</span></span>|<span data-ttu-id="86af4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86af4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86af4-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="86af4-126">Request body</span></span>
<span data-ttu-id="86af4-127">В теле запроса добавьте представление объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86af4-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="86af4-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="86af4-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="86af4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="86af4-129">Property</span></span>|<span data-ttu-id="86af4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="86af4-130">Type</span></span>|<span data-ttu-id="86af4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="86af4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86af4-132">id</span><span class="sxs-lookup"><span data-stu-id="86af4-132">id</span></span>|<span data-ttu-id="86af4-133">Строка</span><span class="sxs-lookup"><span data-stu-id="86af4-133">String</span></span>|<span data-ttu-id="86af4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="86af4-134">Key of the entity.</span></span>|
|<span data-ttu-id="86af4-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="86af4-135">deviceDisplayName</span></span>|<span data-ttu-id="86af4-136">String</span><span class="sxs-lookup"><span data-stu-id="86af4-136">String</span></span>|<span data-ttu-id="86af4-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="86af4-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="86af4-138">userName</span><span class="sxs-lookup"><span data-stu-id="86af4-138">userName</span></span>|<span data-ttu-id="86af4-139">String</span><span class="sxs-lookup"><span data-stu-id="86af4-139">String</span></span>|<span data-ttu-id="86af4-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="86af4-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="86af4-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="86af4-141">deviceModel</span></span>|<span data-ttu-id="86af4-142">String</span><span class="sxs-lookup"><span data-stu-id="86af4-142">String</span></span>|<span data-ttu-id="86af4-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="86af4-143">The device model that is being reported</span></span>|
|<span data-ttu-id="86af4-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="86af4-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="86af4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86af4-145">DateTimeOffset</span></span>|<span data-ttu-id="86af4-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="86af4-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="86af4-147">status</span><span class="sxs-lookup"><span data-stu-id="86af4-147">status</span></span>|[<span data-ttu-id="86af4-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="86af4-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="86af4-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="86af4-149">Compliance status of the policy report.</span></span> <span data-ttu-id="86af4-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="86af4-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="86af4-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="86af4-151">lastReportedDateTime</span></span>|<span data-ttu-id="86af4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86af4-152">DateTimeOffset</span></span>|<span data-ttu-id="86af4-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="86af4-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="86af4-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="86af4-154">userPrincipalName</span></span>|<span data-ttu-id="86af4-155">String</span><span class="sxs-lookup"><span data-stu-id="86af4-155">String</span></span>|<span data-ttu-id="86af4-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="86af4-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="86af4-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="86af4-157">Response</span></span>
<span data-ttu-id="86af4-158">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="86af4-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86af4-159">Пример</span><span class="sxs-lookup"><span data-stu-id="86af4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="86af4-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="86af4-160">Request</span></span>
<span data-ttu-id="86af4-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86af4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 429

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="86af4-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="86af4-162">Response</span></span>
<span data-ttu-id="86af4-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86af4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```






