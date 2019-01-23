---
title: Обновление объекта deviceComplianceDeviceStatus
description: Обновление свойств объекта deviceComplianceDeviceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35273f196231912f8343130e5a58ff62949579ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425493"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="c2d21-103">Обновление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="c2d21-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="c2d21-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2d21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c2d21-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2d21-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2d21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2d21-107">Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c2d21-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2d21-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2d21-108">Prerequisites</span></span>
<span data-ttu-id="c2d21-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c2d21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c2d21-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2d21-111">Permission type</span></span>|<span data-ttu-id="c2d21-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2d21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2d21-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2d21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2d21-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2d21-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2d21-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2d21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2d21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d21-116">Not supported.</span></span>|
|<span data-ttu-id="c2d21-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2d21-117">Application</span></span>|<span data-ttu-id="c2d21-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2d21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2d21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c2d21-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2d21-120">Request headers</span></span>
|<span data-ttu-id="c2d21-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2d21-121">Header</span></span>|<span data-ttu-id="c2d21-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2d21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2d21-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2d21-123">Authorization</span></span>|<span data-ttu-id="c2d21-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2d21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2d21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2d21-125">Accept</span></span>|<span data-ttu-id="c2d21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2d21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2d21-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2d21-127">Request body</span></span>
<span data-ttu-id="c2d21-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d21-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="c2d21-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c2d21-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="c2d21-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d21-130">Property</span></span>|<span data-ttu-id="c2d21-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d21-131">Type</span></span>|<span data-ttu-id="c2d21-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d21-133">id</span><span class="sxs-lookup"><span data-stu-id="c2d21-133">id</span></span>|<span data-ttu-id="c2d21-134">String</span><span class="sxs-lookup"><span data-stu-id="c2d21-134">String</span></span>|<span data-ttu-id="c2d21-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2d21-135">Key of the entity.</span></span>|
|<span data-ttu-id="c2d21-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2d21-136">deviceDisplayName</span></span>|<span data-ttu-id="c2d21-137">String</span><span class="sxs-lookup"><span data-stu-id="c2d21-137">String</span></span>|<span data-ttu-id="c2d21-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c2d21-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c2d21-139">userName</span><span class="sxs-lookup"><span data-stu-id="c2d21-139">userName</span></span>|<span data-ttu-id="c2d21-140">String</span><span class="sxs-lookup"><span data-stu-id="c2d21-140">String</span></span>|<span data-ttu-id="c2d21-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="c2d21-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="c2d21-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c2d21-142">deviceModel</span></span>|<span data-ttu-id="c2d21-143">String</span><span class="sxs-lookup"><span data-stu-id="c2d21-143">String</span></span>|<span data-ttu-id="c2d21-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="c2d21-144">The device model that is being reported</span></span>|
|<span data-ttu-id="c2d21-145">platform</span><span class="sxs-lookup"><span data-stu-id="c2d21-145">platform</span></span>|<span data-ttu-id="c2d21-146">Int32</span><span class="sxs-lookup"><span data-stu-id="c2d21-146">Int32</span></span>|<span data-ttu-id="c2d21-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="c2d21-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="c2d21-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d21-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c2d21-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d21-149">DateTimeOffset</span></span>|<span data-ttu-id="c2d21-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="c2d21-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="c2d21-151">status</span><span class="sxs-lookup"><span data-stu-id="c2d21-151">status</span></span>|[<span data-ttu-id="c2d21-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c2d21-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c2d21-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="c2d21-153">Compliance status of the policy report.</span></span> <span data-ttu-id="c2d21-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c2d21-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c2d21-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2d21-155">lastReportedDateTime</span></span>|<span data-ttu-id="c2d21-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2d21-156">DateTimeOffset</span></span>|<span data-ttu-id="c2d21-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="c2d21-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c2d21-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2d21-158">userPrincipalName</span></span>|<span data-ttu-id="c2d21-159">String</span><span class="sxs-lookup"><span data-stu-id="c2d21-159">String</span></span>|<span data-ttu-id="c2d21-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c2d21-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c2d21-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2d21-161">Response</span></span>
<span data-ttu-id="c2d21-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2d21-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2d21-163">Пример</span><span class="sxs-lookup"><span data-stu-id="c2d21-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2d21-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2d21-164">Request</span></span>
<span data-ttu-id="c2d21-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2d21-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="c2d21-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2d21-166">Response</span></span>
<span data-ttu-id="c2d21-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2d21-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
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




