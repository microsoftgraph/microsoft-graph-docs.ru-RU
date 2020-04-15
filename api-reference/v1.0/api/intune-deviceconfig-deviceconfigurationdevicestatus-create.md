---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 584b85ba203c4b37e2e35eedee5a1cbad213e70d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450702"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="41d76-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="41d76-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="41d76-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41d76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41d76-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41d76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d76-106">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="41d76-106">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41d76-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41d76-107">Prerequisites</span></span>
<span data-ttu-id="41d76-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41d76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41d76-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41d76-110">Permission type</span></span>|<span data-ttu-id="41d76-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41d76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41d76-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41d76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41d76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41d76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41d76-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41d76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41d76-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41d76-115">Not supported.</span></span>|
|<span data-ttu-id="41d76-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41d76-116">Application</span></span>|<span data-ttu-id="41d76-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41d76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41d76-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41d76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="41d76-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="41d76-119">Request headers</span></span>
|<span data-ttu-id="41d76-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41d76-120">Header</span></span>|<span data-ttu-id="41d76-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41d76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41d76-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41d76-122">Authorization</span></span>|<span data-ttu-id="41d76-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41d76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41d76-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41d76-124">Accept</span></span>|<span data-ttu-id="41d76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41d76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41d76-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41d76-126">Request body</span></span>
<span data-ttu-id="41d76-127">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41d76-127">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="41d76-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="41d76-128">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="41d76-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="41d76-129">Property</span></span>|<span data-ttu-id="41d76-130">Тип</span><span class="sxs-lookup"><span data-stu-id="41d76-130">Type</span></span>|<span data-ttu-id="41d76-131">Описание</span><span class="sxs-lookup"><span data-stu-id="41d76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d76-132">id</span><span class="sxs-lookup"><span data-stu-id="41d76-132">id</span></span>|<span data-ttu-id="41d76-133">Строка</span><span class="sxs-lookup"><span data-stu-id="41d76-133">String</span></span>|<span data-ttu-id="41d76-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41d76-134">Key of the entity.</span></span>|
|<span data-ttu-id="41d76-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="41d76-135">deviceDisplayName</span></span>|<span data-ttu-id="41d76-136">String</span><span class="sxs-lookup"><span data-stu-id="41d76-136">String</span></span>|<span data-ttu-id="41d76-137">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="41d76-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="41d76-138">userName</span><span class="sxs-lookup"><span data-stu-id="41d76-138">userName</span></span>|<span data-ttu-id="41d76-139">String</span><span class="sxs-lookup"><span data-stu-id="41d76-139">String</span></span>|<span data-ttu-id="41d76-140">Имя пользователя в отчете</span><span class="sxs-lookup"><span data-stu-id="41d76-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="41d76-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="41d76-141">deviceModel</span></span>|<span data-ttu-id="41d76-142">String</span><span class="sxs-lookup"><span data-stu-id="41d76-142">String</span></span>|<span data-ttu-id="41d76-143">Модель устройства в отчете</span><span class="sxs-lookup"><span data-stu-id="41d76-143">The device model that is being reported</span></span>|
|<span data-ttu-id="41d76-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="41d76-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="41d76-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41d76-145">DateTimeOffset</span></span>|<span data-ttu-id="41d76-146">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41d76-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="41d76-147">status</span><span class="sxs-lookup"><span data-stu-id="41d76-147">status</span></span>|[<span data-ttu-id="41d76-148">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="41d76-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="41d76-149">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="41d76-149">Compliance status of the policy report.</span></span> <span data-ttu-id="41d76-150">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="41d76-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="41d76-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="41d76-151">lastReportedDateTime</span></span>|<span data-ttu-id="41d76-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41d76-152">DateTimeOffset</span></span>|<span data-ttu-id="41d76-153">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="41d76-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="41d76-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41d76-154">userPrincipalName</span></span>|<span data-ttu-id="41d76-155">String</span><span class="sxs-lookup"><span data-stu-id="41d76-155">String</span></span>|<span data-ttu-id="41d76-156">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="41d76-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="41d76-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d76-157">Response</span></span>
<span data-ttu-id="41d76-158">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="41d76-158">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41d76-159">Пример</span><span class="sxs-lookup"><span data-stu-id="41d76-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="41d76-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="41d76-160">Request</span></span>
<span data-ttu-id="41d76-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41d76-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="41d76-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="41d76-162">Response</span></span>
<span data-ttu-id="41d76-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41d76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






