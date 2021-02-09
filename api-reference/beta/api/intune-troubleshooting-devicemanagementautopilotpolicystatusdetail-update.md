---
title: Обновление deviceManagementAutopilotPolicyStatusDetail
description: Обновление свойств объекта deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8e38d9ae11c0eb34d92681725fcd3173e2d9a9b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155631"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="3a66d-103">Обновление deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="3a66d-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="3a66d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a66d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a66d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a66d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a66d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3a66d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a66d-107">Обновление свойств объекта [deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="3a66d-107">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a66d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3a66d-108">Prerequisites</span></span>
<span data-ttu-id="3a66d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a66d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a66d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a66d-111">Permission type</span></span>|<span data-ttu-id="3a66d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a66d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a66d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a66d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a66d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a66d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3a66d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a66d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a66d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a66d-116">Not supported.</span></span>|
|<span data-ttu-id="3a66d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3a66d-117">Application</span></span>|<span data-ttu-id="3a66d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a66d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a66d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a66d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="3a66d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3a66d-120">Request headers</span></span>
|<span data-ttu-id="3a66d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a66d-121">Header</span></span>|<span data-ttu-id="3a66d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3a66d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a66d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a66d-123">Authorization</span></span>|<span data-ttu-id="3a66d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a66d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a66d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3a66d-125">Accept</span></span>|<span data-ttu-id="3a66d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a66d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a66d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a66d-127">Request body</span></span>
<span data-ttu-id="3a66d-128">В теле запроса предопределение представления объекта [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="3a66d-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="3a66d-129">В следующей таблице показаны свойства, необходимые при создании [объекта deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="3a66d-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="3a66d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a66d-130">Property</span></span>|<span data-ttu-id="3a66d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3a66d-131">Type</span></span>|<span data-ttu-id="3a66d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3a66d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a66d-133">id</span><span class="sxs-lookup"><span data-stu-id="3a66d-133">id</span></span>|<span data-ttu-id="3a66d-134">String</span><span class="sxs-lookup"><span data-stu-id="3a66d-134">String</span></span>|<span data-ttu-id="3a66d-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="3a66d-135">UUID for the object</span></span>|
|<span data-ttu-id="3a66d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3a66d-136">displayName</span></span>|<span data-ttu-id="3a66d-137">String</span><span class="sxs-lookup"><span data-stu-id="3a66d-137">String</span></span>|<span data-ttu-id="3a66d-138">Удобное имя политики.</span><span class="sxs-lookup"><span data-stu-id="3a66d-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="3a66d-139">policyType</span><span class="sxs-lookup"><span data-stu-id="3a66d-139">policyType</span></span>|[<span data-ttu-id="3a66d-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="3a66d-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="3a66d-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="3a66d-141">The type of policy.</span></span> <span data-ttu-id="3a66d-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="3a66d-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="3a66d-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3a66d-143">complianceStatus</span></span>|[<span data-ttu-id="3a66d-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="3a66d-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="3a66d-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="3a66d-145">The policy compliance status.</span></span> <span data-ttu-id="3a66d-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="3a66d-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="3a66d-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="3a66d-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="3a66d-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="3a66d-148">Boolean</span></span>|<span data-ttu-id="3a66d-149">Указывает, отслеживался ли этот выпуск в рамках сеанса синхронизации регистрации при загрузке Autopilot</span><span class="sxs-lookup"><span data-stu-id="3a66d-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="3a66d-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a66d-150">lastReportedDateTime</span></span>|<span data-ttu-id="3a66d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a66d-151">DateTimeOffset</span></span>|<span data-ttu-id="3a66d-152">Timestamp of the reported policy status</span><span class="sxs-lookup"><span data-stu-id="3a66d-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="3a66d-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="3a66d-153">errorCode</span></span>|<span data-ttu-id="3a66d-154">Int32</span><span class="sxs-lookup"><span data-stu-id="3a66d-154">Int32</span></span>|<span data-ttu-id="3a66d-155">Errorode, связанный с состоянием соответствия или выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="3a66d-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="3a66d-156">Код ошибки для состояния принудения имеет приоритет, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3a66d-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="3a66d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a66d-157">Response</span></span>
<span data-ttu-id="3a66d-158">В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a66d-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a66d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="3a66d-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a66d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a66d-160">Request</span></span>
<span data-ttu-id="3a66d-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a66d-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```

### <a name="response"></a><span data-ttu-id="3a66d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a66d-162">Response</span></span>
<span data-ttu-id="3a66d-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3a66d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```




