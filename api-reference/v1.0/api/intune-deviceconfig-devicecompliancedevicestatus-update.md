---
title: Обновление объекта deviceComplianceDeviceStatus
description: Обновление свойств объекта deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f35f353cca2eca8f1284bcd998087920f3f47a72
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929587"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="4c4a7-103">Обновление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="4c4a7-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="4c4a7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c4a7-105">Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c4a7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c4a7-106">Prerequisites</span></span>
<span data-ttu-id="4c4a7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4a7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c4a7-109">Permission type</span></span>|<span data-ttu-id="4c4a7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c4a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c4a7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c4a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c4a7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4a7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c4a7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c4a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c4a7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-114">Not supported.</span></span>|
|<span data-ttu-id="4c4a7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c4a7-115">Application</span></span>|<span data-ttu-id="4c4a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c4a7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c4a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="4c4a7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c4a7-118">Request headers</span></span>
|<span data-ttu-id="4c4a7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c4a7-119">Header</span></span>|<span data-ttu-id="4c4a7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="4c4a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c4a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4a7-121">Authorization</span></span>|<span data-ttu-id="4c4a7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c4a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c4a7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4c4a7-123">Accept</span></span>|<span data-ttu-id="4c4a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c4a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c4a7-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c4a7-125">Request body</span></span>
<span data-ttu-id="4c4a7-126">В тексте запроса добавьте представление объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="4c4a7-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="4c4a7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c4a7-128">Property</span></span>|<span data-ttu-id="4c4a7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="4c4a7-129">Type</span></span>|<span data-ttu-id="4c4a7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="4c4a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c4a7-131">id</span><span class="sxs-lookup"><span data-stu-id="4c4a7-131">id</span></span>|<span data-ttu-id="4c4a7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="4c4a7-132">String</span></span>|<span data-ttu-id="4c4a7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-133">Key of the entity.</span></span>|
|<span data-ttu-id="4c4a7-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4c4a7-134">deviceDisplayName</span></span>|<span data-ttu-id="4c4a7-135">String</span><span class="sxs-lookup"><span data-stu-id="4c4a7-135">String</span></span>|<span data-ttu-id="4c4a7-136">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="4c4a7-137">userName</span><span class="sxs-lookup"><span data-stu-id="4c4a7-137">userName</span></span>|<span data-ttu-id="4c4a7-138">String</span><span class="sxs-lookup"><span data-stu-id="4c4a7-138">String</span></span>|<span data-ttu-id="4c4a7-139">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="4c4a7-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4c4a7-140">deviceModel</span></span>|<span data-ttu-id="4c4a7-141">String</span><span class="sxs-lookup"><span data-stu-id="4c4a7-141">String</span></span>|<span data-ttu-id="4c4a7-142">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-142">The device model that is being reported</span></span>|
|<span data-ttu-id="4c4a7-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4c4a7-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4c4a7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c4a7-144">DateTimeOffset</span></span>|<span data-ttu-id="4c4a7-145">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="4c4a7-146">status</span><span class="sxs-lookup"><span data-stu-id="4c4a7-146">status</span></span>|[<span data-ttu-id="4c4a7-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4c4a7-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4c4a7-148">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-148">Compliance status of the policy report.</span></span> <span data-ttu-id="4c4a7-149">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4c4a7-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c4a7-150">lastReportedDateTime</span></span>|<span data-ttu-id="4c4a7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c4a7-151">DateTimeOffset</span></span>|<span data-ttu-id="4c4a7-152">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="4c4a7-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4c4a7-153">userPrincipalName</span></span>|<span data-ttu-id="4c4a7-154">String</span><span class="sxs-lookup"><span data-stu-id="4c4a7-154">String</span></span>|<span data-ttu-id="4c4a7-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="4c4a7-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c4a7-156">Response</span></span>
<span data-ttu-id="4c4a7-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c4a7-158">Пример</span><span class="sxs-lookup"><span data-stu-id="4c4a7-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c4a7-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c4a7-159">Request</span></span>
<span data-ttu-id="4c4a7-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="4c4a7-161">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c4a7-161">Response</span></span>
<span data-ttu-id="4c4a7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



