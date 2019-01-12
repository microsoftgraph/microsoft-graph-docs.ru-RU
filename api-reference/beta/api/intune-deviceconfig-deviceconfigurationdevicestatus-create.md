---
title: Создание объекта deviceConfigurationDeviceStatus
description: Создание объекта deviceConfigurationDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18f2875409f2eb9ae56639c2a1944c99ffe537a6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921985"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="f3cac-103">Создание объекта deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f3cac-103">Create deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="f3cac-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f3cac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3cac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3cac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3cac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f3cac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3cac-107">Создание объекта [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f3cac-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f3cac-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f3cac-108">Prerequisites</span></span>
<span data-ttu-id="f3cac-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3cac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3cac-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f3cac-111">Permission type</span></span>|<span data-ttu-id="f3cac-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f3cac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3cac-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f3cac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3cac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3cac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3cac-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f3cac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3cac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3cac-116">Not supported.</span></span>|
|<span data-ttu-id="f3cac-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f3cac-117">Application</span></span>|<span data-ttu-id="f3cac-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f3cac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3cac-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f3cac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f3cac-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f3cac-120">Request headers</span></span>
|<span data-ttu-id="f3cac-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f3cac-121">Header</span></span>|<span data-ttu-id="f3cac-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f3cac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3cac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3cac-123">Authorization</span></span>|<span data-ttu-id="f3cac-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f3cac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3cac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f3cac-125">Accept</span></span>|<span data-ttu-id="f3cac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3cac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3cac-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f3cac-127">Request body</span></span>
<span data-ttu-id="f3cac-128">В теле запроса добавьте представление объекта deviceConfigurationDeviceStatus в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3cac-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="f3cac-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="f3cac-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="f3cac-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3cac-130">Property</span></span>|<span data-ttu-id="f3cac-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f3cac-131">Type</span></span>|<span data-ttu-id="f3cac-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f3cac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cac-133">id</span><span class="sxs-lookup"><span data-stu-id="f3cac-133">id</span></span>|<span data-ttu-id="f3cac-134">String</span><span class="sxs-lookup"><span data-stu-id="f3cac-134">String</span></span>|<span data-ttu-id="f3cac-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f3cac-135">Key of the entity.</span></span>|
|<span data-ttu-id="f3cac-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f3cac-136">deviceDisplayName</span></span>|<span data-ttu-id="f3cac-137">String</span><span class="sxs-lookup"><span data-stu-id="f3cac-137">String</span></span>|<span data-ttu-id="f3cac-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f3cac-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f3cac-139">userName</span><span class="sxs-lookup"><span data-stu-id="f3cac-139">userName</span></span>|<span data-ttu-id="f3cac-140">String</span><span class="sxs-lookup"><span data-stu-id="f3cac-140">String</span></span>|<span data-ttu-id="f3cac-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="f3cac-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="f3cac-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f3cac-142">deviceModel</span></span>|<span data-ttu-id="f3cac-143">String</span><span class="sxs-lookup"><span data-stu-id="f3cac-143">String</span></span>|<span data-ttu-id="f3cac-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="f3cac-144">The device model that is being reported</span></span>|
|<span data-ttu-id="f3cac-145">platform</span><span class="sxs-lookup"><span data-stu-id="f3cac-145">platform</span></span>|<span data-ttu-id="f3cac-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f3cac-146">Int32</span></span>|<span data-ttu-id="f3cac-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="f3cac-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f3cac-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f3cac-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f3cac-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3cac-149">DateTimeOffset</span></span>|<span data-ttu-id="f3cac-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="f3cac-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f3cac-151">status</span><span class="sxs-lookup"><span data-stu-id="f3cac-151">status</span></span>|[<span data-ttu-id="f3cac-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f3cac-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f3cac-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f3cac-153">Compliance status of the policy report.</span></span> <span data-ttu-id="f3cac-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f3cac-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f3cac-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3cac-155">lastReportedDateTime</span></span>|<span data-ttu-id="f3cac-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3cac-156">DateTimeOffset</span></span>|<span data-ttu-id="f3cac-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="f3cac-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f3cac-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f3cac-158">userPrincipalName</span></span>|<span data-ttu-id="f3cac-159">String</span><span class="sxs-lookup"><span data-stu-id="f3cac-159">String</span></span>|<span data-ttu-id="f3cac-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f3cac-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f3cac-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="f3cac-161">Response</span></span>
<span data-ttu-id="f3cac-162">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f3cac-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3cac-163">Пример</span><span class="sxs-lookup"><span data-stu-id="f3cac-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="f3cac-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="f3cac-164">Request</span></span>
<span data-ttu-id="f3cac-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f3cac-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="f3cac-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="f3cac-166">Response</span></span>
<span data-ttu-id="f3cac-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f3cac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
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





