---
title: Обновление Девицеманажементаутопилотполицистатусдетаил
description: Обновление свойств объекта Девицеманажементаутопилотполицистатусдетаил.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c3c94dcde401fb4917171e97b18995bf2c6cf07
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800202"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="d6b8d-103">Обновление Девицеманажементаутопилотполицистатусдетаил</span><span class="sxs-lookup"><span data-stu-id="d6b8d-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

> <span data-ttu-id="d6b8d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6b8d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b8d-106">Обновление свойств объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="d6b8d-106">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6b8d-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d6b8d-107">Prerequisites</span></span>
<span data-ttu-id="d6b8d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6b8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b8d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6b8d-110">Permission type</span></span>|<span data-ttu-id="d6b8d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6b8d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b8d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6b8d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b8d-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b8d-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d6b8d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6b8d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-115">Not supported.</span></span>|
|<span data-ttu-id="d6b8d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d6b8d-116">Application</span></span>|<span data-ttu-id="d6b8d-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b8d-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b8d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6b8d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="d6b8d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d6b8d-119">Request headers</span></span>
|<span data-ttu-id="d6b8d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6b8d-120">Header</span></span>|<span data-ttu-id="d6b8d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d6b8d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b8d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b8d-122">Authorization</span></span>|<span data-ttu-id="d6b8d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6b8d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d6b8d-124">Accept</span></span>|<span data-ttu-id="d6b8d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b8d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b8d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d6b8d-126">Request body</span></span>
<span data-ttu-id="d6b8d-127">В тексте запроса добавьте представление объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-127">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="d6b8d-128">В следующей таблице приведены свойства, необходимые при создании [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span><span class="sxs-lookup"><span data-stu-id="d6b8d-128">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="d6b8d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6b8d-129">Property</span></span>|<span data-ttu-id="d6b8d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b8d-130">Type</span></span>|<span data-ttu-id="d6b8d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b8d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b8d-132">id</span><span class="sxs-lookup"><span data-stu-id="d6b8d-132">id</span></span>|<span data-ttu-id="d6b8d-133">String</span><span class="sxs-lookup"><span data-stu-id="d6b8d-133">String</span></span>|<span data-ttu-id="d6b8d-134">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-134">UUID for the object</span></span>|
|<span data-ttu-id="d6b8d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d6b8d-135">displayName</span></span>|<span data-ttu-id="d6b8d-136">Строка</span><span class="sxs-lookup"><span data-stu-id="d6b8d-136">String</span></span>|<span data-ttu-id="d6b8d-137">Понятное имя политики.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-137">The friendly name of the policy.</span></span>|
|<span data-ttu-id="d6b8d-138">полицитипе</span><span class="sxs-lookup"><span data-stu-id="d6b8d-138">policyType</span></span>|[<span data-ttu-id="d6b8d-139">девицеманажементаутопилотполицитипе</span><span class="sxs-lookup"><span data-stu-id="d6b8d-139">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="d6b8d-140">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-140">The type of policy.</span></span> <span data-ttu-id="d6b8d-141">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-141">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="d6b8d-142">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="d6b8d-142">complianceStatus</span></span>|[<span data-ttu-id="d6b8d-143">девицеманажементаутопилотполицикомплианцестатус</span><span class="sxs-lookup"><span data-stu-id="d6b8d-143">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="d6b8d-144">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-144">The policy compliance status.</span></span> <span data-ttu-id="d6b8d-145">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-145">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="d6b8d-146">траккедоненроллментстатус</span><span class="sxs-lookup"><span data-stu-id="d6b8d-146">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="d6b8d-147">Логический</span><span class="sxs-lookup"><span data-stu-id="d6b8d-147">Boolean</span></span>|<span data-ttu-id="d6b8d-148">Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="d6b8d-148">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="d6b8d-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b8d-149">lastReportedDateTime</span></span>|<span data-ttu-id="d6b8d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b8d-150">DateTimeOffset</span></span>|<span data-ttu-id="d6b8d-151">Метка времени для отчета о состоянии политики</span><span class="sxs-lookup"><span data-stu-id="d6b8d-151">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="d6b8d-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b8d-152">Response</span></span>
<span data-ttu-id="d6b8d-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b8d-154">Пример</span><span class="sxs-lookup"><span data-stu-id="d6b8d-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6b8d-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6b8d-155">Request</span></span>
<span data-ttu-id="d6b8d-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="d6b8d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6b8d-157">Response</span></span>
<span data-ttu-id="d6b8d-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6b8d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```




