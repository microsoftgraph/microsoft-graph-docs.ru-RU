---
title: Обновление объекта deviceComplianceDeviceStatus
description: Обновление свойств объекта deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 8a19eb26870f41d1a84b977af79feb0947b54073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325335"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="41835-103">Обновление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="41835-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="41835-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41835-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41835-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41835-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="41835-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41835-107">Обновление свойств объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="41835-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41835-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="41835-108">Prerequisites</span></span>
<span data-ttu-id="41835-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41835-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41835-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41835-111">Permission type</span></span>|<span data-ttu-id="41835-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41835-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41835-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41835-113">Delegated (work or school account)</span></span>|<span data-ttu-id="41835-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41835-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41835-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41835-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41835-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41835-116">Not supported.</span></span>|
|<span data-ttu-id="41835-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41835-117">Application</span></span>|<span data-ttu-id="41835-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41835-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41835-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41835-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="41835-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41835-120">Request headers</span></span>
|<span data-ttu-id="41835-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41835-121">Header</span></span>|<span data-ttu-id="41835-122">Значение</span><span class="sxs-lookup"><span data-stu-id="41835-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41835-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41835-123">Authorization</span></span>|<span data-ttu-id="41835-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="41835-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41835-125">Accept</span><span class="sxs-lookup"><span data-stu-id="41835-125">Accept</span></span>|<span data-ttu-id="41835-126">application/json</span><span class="sxs-lookup"><span data-stu-id="41835-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41835-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41835-127">Request body</span></span>
<span data-ttu-id="41835-128">В тексте запроса добавьте представление объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41835-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="41835-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="41835-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="41835-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="41835-130">Property</span></span>|<span data-ttu-id="41835-131">Тип</span><span class="sxs-lookup"><span data-stu-id="41835-131">Type</span></span>|<span data-ttu-id="41835-132">Описание</span><span class="sxs-lookup"><span data-stu-id="41835-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41835-133">id</span><span class="sxs-lookup"><span data-stu-id="41835-133">id</span></span>|<span data-ttu-id="41835-134">Строка</span><span class="sxs-lookup"><span data-stu-id="41835-134">String</span></span>|<span data-ttu-id="41835-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41835-135">Key of the entity.</span></span>|
|<span data-ttu-id="41835-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="41835-136">deviceDisplayName</span></span>|<span data-ttu-id="41835-137">String</span><span class="sxs-lookup"><span data-stu-id="41835-137">String</span></span>|<span data-ttu-id="41835-138">Имя устройства в объекте DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="41835-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="41835-139">userName</span><span class="sxs-lookup"><span data-stu-id="41835-139">userName</span></span>|<span data-ttu-id="41835-140">String</span><span class="sxs-lookup"><span data-stu-id="41835-140">String</span></span>|<span data-ttu-id="41835-141">Имя пользователя в отчете.</span><span class="sxs-lookup"><span data-stu-id="41835-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="41835-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="41835-142">deviceModel</span></span>|<span data-ttu-id="41835-143">String</span><span class="sxs-lookup"><span data-stu-id="41835-143">String</span></span>|<span data-ttu-id="41835-144">Модель устройства в отчете.</span><span class="sxs-lookup"><span data-stu-id="41835-144">The device model that is being reported</span></span>|
|<span data-ttu-id="41835-145">platform</span><span class="sxs-lookup"><span data-stu-id="41835-145">platform</span></span>|<span data-ttu-id="41835-146">Int32</span><span class="sxs-lookup"><span data-stu-id="41835-146">Int32</span></span>|<span data-ttu-id="41835-147">Платформа устройства, предоставленные</span><span class="sxs-lookup"><span data-stu-id="41835-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="41835-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="41835-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="41835-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41835-149">DateTimeOffset</span></span>|<span data-ttu-id="41835-150">Дата и время, когда истекает период отсрочки применения политик на устройстве.</span><span class="sxs-lookup"><span data-stu-id="41835-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="41835-151">status</span><span class="sxs-lookup"><span data-stu-id="41835-151">status</span></span>|[<span data-ttu-id="41835-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="41835-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="41835-153">Состояние соответствия требованиям для отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="41835-153">Compliance status of the policy report.</span></span> <span data-ttu-id="41835-154">Возможные значения: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="41835-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="41835-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="41835-155">lastReportedDateTime</span></span>|<span data-ttu-id="41835-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41835-156">DateTimeOffset</span></span>|<span data-ttu-id="41835-157">Дата и время последнего изменения отчета о политике.</span><span class="sxs-lookup"><span data-stu-id="41835-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="41835-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41835-158">userPrincipalName</span></span>|<span data-ttu-id="41835-159">String</span><span class="sxs-lookup"><span data-stu-id="41835-159">String</span></span>|<span data-ttu-id="41835-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="41835-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="41835-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="41835-161">Response</span></span>
<span data-ttu-id="41835-162">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41835-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41835-163">Пример</span><span class="sxs-lookup"><span data-stu-id="41835-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="41835-164">Запрос</span><span class="sxs-lookup"><span data-stu-id="41835-164">Request</span></span>
<span data-ttu-id="41835-165">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41835-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 377

{
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

### <a name="response"></a><span data-ttu-id="41835-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="41835-166">Response</span></span>
<span data-ttu-id="41835-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41835-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





