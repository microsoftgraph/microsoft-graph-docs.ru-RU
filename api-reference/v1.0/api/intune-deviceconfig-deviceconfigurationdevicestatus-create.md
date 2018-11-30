---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
ms.openlocfilehash: b79a58ef701d22b35b1c2c19a0c166db02cada11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024787"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="4f2ef-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4f2ef-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="4f2ef-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f2ef-105">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4f2ef-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f2ef-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4f2ef-106">Prerequisites</span></span>
<span data-ttu-id="4f2ef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f2ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f2ef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4f2ef-109">Permission type</span></span>|<span data-ttu-id="4f2ef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4f2ef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f2ef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4f2ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f2ef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f2ef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f2ef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4f2ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f2ef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-114">Not supported.</span></span>|
|<span data-ttu-id="4f2ef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4f2ef-115">Application</span></span>|<span data-ttu-id="4f2ef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f2ef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4f2ef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4f2ef-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4f2ef-118">Request headers</span></span>
|<span data-ttu-id="4f2ef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4f2ef-119">Header</span></span>|<span data-ttu-id="4f2ef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4f2ef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f2ef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f2ef-121">Authorization</span></span>|<span data-ttu-id="4f2ef-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4f2ef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f2ef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4f2ef-123">Accept</span></span>|<span data-ttu-id="4f2ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f2ef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f2ef-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4f2ef-125">Request body</span></span>
<span data-ttu-id="4f2ef-126">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="4f2ef-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="4f2ef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f2ef-128">Property</span></span>|<span data-ttu-id="4f2ef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4f2ef-129">Type</span></span>|<span data-ttu-id="4f2ef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4f2ef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f2ef-131">id</span><span class="sxs-lookup"><span data-stu-id="4f2ef-131">id</span></span>|<span data-ttu-id="4f2ef-132">String</span><span class="sxs-lookup"><span data-stu-id="4f2ef-132">String</span></span>|<span data-ttu-id="4f2ef-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-133">Key of the entity.</span></span>|
|<span data-ttu-id="4f2ef-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4f2ef-134">deviceDisplayName</span></span>|<span data-ttu-id="4f2ef-135">String</span><span class="sxs-lookup"><span data-stu-id="4f2ef-135">String</span></span>|<span data-ttu-id="4f2ef-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4f2ef-137">userName</span><span class="sxs-lookup"><span data-stu-id="4f2ef-137">userName</span></span>|<span data-ttu-id="4f2ef-138">String</span><span class="sxs-lookup"><span data-stu-id="4f2ef-138">String</span></span>|<span data-ttu-id="4f2ef-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="4f2ef-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4f2ef-140">deviceModel</span></span>|<span data-ttu-id="4f2ef-141">String</span><span class="sxs-lookup"><span data-stu-id="4f2ef-141">String</span></span>|<span data-ttu-id="4f2ef-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-142">The device model that is being reported</span></span>|
|<span data-ttu-id="4f2ef-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2ef-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4f2ef-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2ef-144">DateTimeOffset</span></span>|<span data-ttu-id="4f2ef-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4f2ef-146">status</span><span class="sxs-lookup"><span data-stu-id="4f2ef-146">status</span></span>|[<span data-ttu-id="4f2ef-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4f2ef-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4f2ef-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-148">Compliance status of the policy report.</span></span> <span data-ttu-id="4f2ef-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4f2ef-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f2ef-150">lastReportedDateTime</span></span>|<span data-ttu-id="4f2ef-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f2ef-151">DateTimeOffset</span></span>|<span data-ttu-id="4f2ef-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4f2ef-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4f2ef-153">userPrincipalName</span></span>|<span data-ttu-id="4f2ef-154">String</span><span class="sxs-lookup"><span data-stu-id="4f2ef-154">String</span></span>|<span data-ttu-id="4f2ef-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4f2ef-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4f2ef-156">Response</span></span>
<span data-ttu-id="4f2ef-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f2ef-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4f2ef-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f2ef-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4f2ef-159">Request</span></span>
<span data-ttu-id="4f2ef-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4f2ef-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4f2ef-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="4f2ef-161">Response</span></span>
<span data-ttu-id="4f2ef-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="4f2ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



