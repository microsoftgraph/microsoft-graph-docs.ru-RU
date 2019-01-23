---
title: Создание managedDeviceMobileAppConfigurationDeviceStatus
description: Создание нового объекта managedDeviceMobileAppConfigurationDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93d6ac158fc1196ce02c8e09ec997bc3827f8e08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408924"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="2f766-103">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2f766-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2f766-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f766-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f766-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f766-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f766-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f766-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f766-107">Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="2f766-107">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f766-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="2f766-108">Prerequisites</span></span>
<span data-ttu-id="2f766-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f766-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f766-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f766-111">Permission type</span></span>|<span data-ttu-id="2f766-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f766-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f766-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f766-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f766-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f766-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2f766-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f766-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f766-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f766-116">Not supported.</span></span>|
|<span data-ttu-id="2f766-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f766-117">Application</span></span>|<span data-ttu-id="2f766-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f766-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f766-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f766-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2f766-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f766-120">Request headers</span></span>
|<span data-ttu-id="2f766-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f766-121">Header</span></span>|<span data-ttu-id="2f766-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f766-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f766-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f766-123">Authorization</span></span>|<span data-ttu-id="2f766-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f766-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f766-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f766-125">Accept</span></span>|<span data-ttu-id="2f766-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f766-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f766-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f766-127">Request body</span></span>
<span data-ttu-id="2f766-128">В тексте запроса укажите представление JSON для объекта managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2f766-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="2f766-129">В следующей таблице показаны свойства, которые необходимы для создания managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="2f766-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="2f766-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f766-130">Property</span></span>|<span data-ttu-id="2f766-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f766-131">Type</span></span>|<span data-ttu-id="2f766-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f766-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f766-133">id</span><span class="sxs-lookup"><span data-stu-id="2f766-133">id</span></span>|<span data-ttu-id="2f766-134">String</span><span class="sxs-lookup"><span data-stu-id="2f766-134">String</span></span>|<span data-ttu-id="2f766-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2f766-135">Key of the entity.</span></span>|
|<span data-ttu-id="2f766-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2f766-136">deviceDisplayName</span></span>|<span data-ttu-id="2f766-137">String</span><span class="sxs-lookup"><span data-stu-id="2f766-137">String</span></span>|<span data-ttu-id="2f766-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="2f766-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2f766-139">userName</span><span class="sxs-lookup"><span data-stu-id="2f766-139">userName</span></span>|<span data-ttu-id="2f766-140">String</span><span class="sxs-lookup"><span data-stu-id="2f766-140">String</span></span>|<span data-ttu-id="2f766-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="2f766-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="2f766-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2f766-142">deviceModel</span></span>|<span data-ttu-id="2f766-143">String</span><span class="sxs-lookup"><span data-stu-id="2f766-143">String</span></span>|<span data-ttu-id="2f766-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="2f766-144">The device model that is being reported</span></span>|
|<span data-ttu-id="2f766-145">platform</span><span class="sxs-lookup"><span data-stu-id="2f766-145">platform</span></span>|<span data-ttu-id="2f766-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2f766-146">Int32</span></span>|<span data-ttu-id="2f766-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="2f766-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="2f766-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2f766-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2f766-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f766-149">DateTimeOffset</span></span>|<span data-ttu-id="2f766-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="2f766-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2f766-151">status</span><span class="sxs-lookup"><span data-stu-id="2f766-151">status</span></span>|[<span data-ttu-id="2f766-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2f766-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="2f766-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2f766-153">Compliance status of the policy report.</span></span> <span data-ttu-id="2f766-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="2f766-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="2f766-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f766-155">lastReportedDateTime</span></span>|<span data-ttu-id="2f766-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f766-156">DateTimeOffset</span></span>|<span data-ttu-id="2f766-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="2f766-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2f766-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2f766-158">userPrincipalName</span></span>|<span data-ttu-id="2f766-159">String</span><span class="sxs-lookup"><span data-stu-id="2f766-159">String</span></span>|<span data-ttu-id="2f766-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="2f766-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="2f766-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f766-161">Response</span></span>
<span data-ttu-id="2f766-162">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2f766-162">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f766-163">Пример</span><span class="sxs-lookup"><span data-stu-id="2f766-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f766-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f766-164">Request</span></span>
<span data-ttu-id="2f766-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f766-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f766-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f766-166">Response</span></span>
<span data-ttu-id="2f766-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f766-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




