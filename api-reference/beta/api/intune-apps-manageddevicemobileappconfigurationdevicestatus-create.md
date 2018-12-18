---
title: Создание managedDeviceMobileAppConfigurationDeviceStatus
description: Создание нового объекта managedDeviceMobileAppConfigurationDeviceStatus.
author: tfitzmac
ms.openlocfilehash: c98ee7ebbade4f5b32edf51f860b55c8de5db391
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309214"
---
# <a name="create-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="14b60-103">Создание managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="14b60-103">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>

> <span data-ttu-id="14b60-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="14b60-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14b60-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14b60-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="14b60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14b60-107">Создание нового объекта [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) .</span><span class="sxs-lookup"><span data-stu-id="14b60-107">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14b60-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="14b60-108">Prerequisites</span></span>
<span data-ttu-id="14b60-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14b60-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14b60-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14b60-111">Permission type</span></span>|<span data-ttu-id="14b60-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="14b60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14b60-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14b60-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14b60-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14b60-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="14b60-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14b60-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14b60-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b60-116">Not supported.</span></span>|
|<span data-ttu-id="14b60-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14b60-117">Application</span></span>|<span data-ttu-id="14b60-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14b60-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14b60-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14b60-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses
POST /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="14b60-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14b60-120">Request headers</span></span>
|<span data-ttu-id="14b60-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="14b60-121">Header</span></span>|<span data-ttu-id="14b60-122">Значение</span><span class="sxs-lookup"><span data-stu-id="14b60-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14b60-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14b60-123">Authorization</span></span>|<span data-ttu-id="14b60-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="14b60-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14b60-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14b60-125">Accept</span></span>|<span data-ttu-id="14b60-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14b60-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14b60-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14b60-127">Request body</span></span>
<span data-ttu-id="14b60-128">В тексте запроса укажите представление JSON для объекта managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="14b60-128">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="14b60-129">В следующей таблице показаны свойства, которые необходимы для создания managedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="14b60-129">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="14b60-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="14b60-130">Property</span></span>|<span data-ttu-id="14b60-131">Тип</span><span class="sxs-lookup"><span data-stu-id="14b60-131">Type</span></span>|<span data-ttu-id="14b60-132">Описание</span><span class="sxs-lookup"><span data-stu-id="14b60-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14b60-133">id</span><span class="sxs-lookup"><span data-stu-id="14b60-133">id</span></span>|<span data-ttu-id="14b60-134">Строка</span><span class="sxs-lookup"><span data-stu-id="14b60-134">String</span></span>|<span data-ttu-id="14b60-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="14b60-135">Key of the entity.</span></span>|
|<span data-ttu-id="14b60-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="14b60-136">deviceDisplayName</span></span>|<span data-ttu-id="14b60-137">String</span><span class="sxs-lookup"><span data-stu-id="14b60-137">String</span></span>|<span data-ttu-id="14b60-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="14b60-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="14b60-139">userName</span><span class="sxs-lookup"><span data-stu-id="14b60-139">userName</span></span>|<span data-ttu-id="14b60-140">String</span><span class="sxs-lookup"><span data-stu-id="14b60-140">String</span></span>|<span data-ttu-id="14b60-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="14b60-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="14b60-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="14b60-142">deviceModel</span></span>|<span data-ttu-id="14b60-143">String</span><span class="sxs-lookup"><span data-stu-id="14b60-143">String</span></span>|<span data-ttu-id="14b60-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="14b60-144">The device model that is being reported</span></span>|
|<span data-ttu-id="14b60-145">platform</span><span class="sxs-lookup"><span data-stu-id="14b60-145">platform</span></span>|<span data-ttu-id="14b60-146">Int32</span><span class="sxs-lookup"><span data-stu-id="14b60-146">Int32</span></span>|<span data-ttu-id="14b60-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="14b60-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="14b60-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="14b60-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="14b60-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14b60-149">DateTimeOffset</span></span>|<span data-ttu-id="14b60-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="14b60-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="14b60-151">status</span><span class="sxs-lookup"><span data-stu-id="14b60-151">status</span></span>|[<span data-ttu-id="14b60-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="14b60-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="14b60-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="14b60-153">Compliance status of the policy report.</span></span> <span data-ttu-id="14b60-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="14b60-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="14b60-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="14b60-155">lastReportedDateTime</span></span>|<span data-ttu-id="14b60-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14b60-156">DateTimeOffset</span></span>|<span data-ttu-id="14b60-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="14b60-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="14b60-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="14b60-158">userPrincipalName</span></span>|<span data-ttu-id="14b60-159">String</span><span class="sxs-lookup"><span data-stu-id="14b60-159">String</span></span>|<span data-ttu-id="14b60-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="14b60-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="14b60-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="14b60-161">Response</span></span>
<span data-ttu-id="14b60-162">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="14b60-162">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14b60-163">Пример</span><span class="sxs-lookup"><span data-stu-id="14b60-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="14b60-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="14b60-164">Request</span></span>
<span data-ttu-id="14b60-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14b60-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14b60-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="14b60-166">Response</span></span>
<span data-ttu-id="14b60-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="14b60-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





