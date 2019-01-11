---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e9ee1f093ffefa01967e961401aebb479ad57372
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845929"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="858e5-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="858e5-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="858e5-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="858e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="858e5-105">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="858e5-105">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="858e5-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="858e5-106">Prerequisites</span></span>
<span data-ttu-id="858e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="858e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="858e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="858e5-109">Permission type</span></span>|<span data-ttu-id="858e5-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="858e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="858e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="858e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="858e5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="858e5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="858e5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="858e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="858e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858e5-114">Not supported.</span></span>|
|<span data-ttu-id="858e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="858e5-115">Application</span></span>|<span data-ttu-id="858e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="858e5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="858e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="858e5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="858e5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="858e5-118">Request headers</span></span>
|<span data-ttu-id="858e5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="858e5-119">Header</span></span>|<span data-ttu-id="858e5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="858e5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="858e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="858e5-121">Authorization</span></span>|<span data-ttu-id="858e5-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="858e5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="858e5-123">Accept</span><span class="sxs-lookup"><span data-stu-id="858e5-123">Accept</span></span>|<span data-ttu-id="858e5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="858e5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="858e5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="858e5-125">Request body</span></span>
<span data-ttu-id="858e5-126">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="858e5-126">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="858e5-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="858e5-127">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="858e5-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="858e5-128">Property</span></span>|<span data-ttu-id="858e5-129">Тип</span><span class="sxs-lookup"><span data-stu-id="858e5-129">Type</span></span>|<span data-ttu-id="858e5-130">Описание</span><span class="sxs-lookup"><span data-stu-id="858e5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="858e5-131">id</span><span class="sxs-lookup"><span data-stu-id="858e5-131">id</span></span>|<span data-ttu-id="858e5-132">Строка</span><span class="sxs-lookup"><span data-stu-id="858e5-132">String</span></span>|<span data-ttu-id="858e5-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="858e5-133">Key of the entity.</span></span>|
|<span data-ttu-id="858e5-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="858e5-134">deviceDisplayName</span></span>|<span data-ttu-id="858e5-135">String</span><span class="sxs-lookup"><span data-stu-id="858e5-135">String</span></span>|<span data-ttu-id="858e5-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="858e5-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="858e5-137">userName</span><span class="sxs-lookup"><span data-stu-id="858e5-137">userName</span></span>|<span data-ttu-id="858e5-138">String</span><span class="sxs-lookup"><span data-stu-id="858e5-138">String</span></span>|<span data-ttu-id="858e5-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="858e5-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="858e5-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="858e5-140">deviceModel</span></span>|<span data-ttu-id="858e5-141">String</span><span class="sxs-lookup"><span data-stu-id="858e5-141">String</span></span>|<span data-ttu-id="858e5-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="858e5-142">The device model that is being reported</span></span>|
|<span data-ttu-id="858e5-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="858e5-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="858e5-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="858e5-144">DateTimeOffset</span></span>|<span data-ttu-id="858e5-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="858e5-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="858e5-146">status</span><span class="sxs-lookup"><span data-stu-id="858e5-146">status</span></span>|[<span data-ttu-id="858e5-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="858e5-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="858e5-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="858e5-148">Compliance status of the policy report.</span></span> <span data-ttu-id="858e5-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="858e5-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="858e5-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="858e5-150">lastReportedDateTime</span></span>|<span data-ttu-id="858e5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="858e5-151">DateTimeOffset</span></span>|<span data-ttu-id="858e5-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="858e5-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="858e5-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="858e5-153">userPrincipalName</span></span>|<span data-ttu-id="858e5-154">String</span><span class="sxs-lookup"><span data-stu-id="858e5-154">String</span></span>|<span data-ttu-id="858e5-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="858e5-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="858e5-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="858e5-156">Response</span></span>
<span data-ttu-id="858e5-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="858e5-157">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="858e5-158">Пример</span><span class="sxs-lookup"><span data-stu-id="858e5-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="858e5-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="858e5-159">Request</span></span>
<span data-ttu-id="858e5-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="858e5-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="858e5-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="858e5-161">Response</span></span>
<span data-ttu-id="858e5-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="858e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



