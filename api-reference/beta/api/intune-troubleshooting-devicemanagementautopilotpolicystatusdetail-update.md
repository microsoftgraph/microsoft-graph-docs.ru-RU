---
title: Обновление Девицеманажементаутопилотполицистатусдетаил
description: Обновление свойств объекта Девицеманажементаутопилотполицистатусдетаил.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6131ec1b4fb52cce0c3af969d48473780efdb8ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49223488"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="c8ad6-103">Обновление Девицеманажементаутопилотполицистатусдетаил</span><span class="sxs-lookup"><span data-stu-id="c8ad6-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="c8ad6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8ad6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8ad6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8ad6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8ad6-107">Обновление свойств объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="c8ad6-107">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8ad6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8ad6-108">Prerequisites</span></span>
<span data-ttu-id="c8ad6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8ad6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8ad6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8ad6-111">Permission type</span></span>|<span data-ttu-id="c8ad6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8ad6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8ad6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ad6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8ad6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8ad6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8ad6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-116">Not supported.</span></span>|
|<span data-ttu-id="c8ad6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="c8ad6-117">Application</span></span>|<span data-ttu-id="c8ad6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8ad6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8ad6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8ad6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="c8ad6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8ad6-120">Request headers</span></span>
|<span data-ttu-id="c8ad6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8ad6-121">Header</span></span>|<span data-ttu-id="c8ad6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8ad6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8ad6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8ad6-123">Authorization</span></span>|<span data-ttu-id="c8ad6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8ad6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8ad6-125">Accept</span></span>|<span data-ttu-id="c8ad6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8ad6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8ad6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8ad6-127">Request body</span></span>
<span data-ttu-id="c8ad6-128">В тексте запроса добавьте представление объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="c8ad6-129">В следующей таблице приведены свойства, необходимые при создании [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span><span class="sxs-lookup"><span data-stu-id="c8ad6-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="c8ad6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8ad6-130">Property</span></span>|<span data-ttu-id="c8ad6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8ad6-131">Type</span></span>|<span data-ttu-id="c8ad6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8ad6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8ad6-133">id</span><span class="sxs-lookup"><span data-stu-id="c8ad6-133">id</span></span>|<span data-ttu-id="c8ad6-134">String</span><span class="sxs-lookup"><span data-stu-id="c8ad6-134">String</span></span>|<span data-ttu-id="c8ad6-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-135">UUID for the object</span></span>|
|<span data-ttu-id="c8ad6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8ad6-136">displayName</span></span>|<span data-ttu-id="c8ad6-137">String</span><span class="sxs-lookup"><span data-stu-id="c8ad6-137">String</span></span>|<span data-ttu-id="c8ad6-138">Понятное имя политики.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="c8ad6-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="c8ad6-139">policyType</span></span>|[<span data-ttu-id="c8ad6-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="c8ad6-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="c8ad6-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-141">The type of policy.</span></span> <span data-ttu-id="c8ad6-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="c8ad6-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="c8ad6-143">complianceStatus</span></span>|[<span data-ttu-id="c8ad6-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="c8ad6-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="c8ad6-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-145">The policy compliance status.</span></span> <span data-ttu-id="c8ad6-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="c8ad6-147">траккедоненроллментстатус</span><span class="sxs-lookup"><span data-stu-id="c8ad6-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="c8ad6-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8ad6-148">Boolean</span></span>|<span data-ttu-id="c8ad6-149">Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="c8ad6-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="c8ad6-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8ad6-150">lastReportedDateTime</span></span>|<span data-ttu-id="c8ad6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8ad6-151">DateTimeOffset</span></span>|<span data-ttu-id="c8ad6-152">Метка времени для отчета о состоянии политики</span><span class="sxs-lookup"><span data-stu-id="c8ad6-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="c8ad6-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8ad6-153">Response</span></span>
<span data-ttu-id="c8ad6-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8ad6-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c8ad6-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8ad6-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8ad6-156">Request</span></span>
<span data-ttu-id="c8ad6-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8ad6-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8ad6-158">Response</span></span>
<span data-ttu-id="c8ad6-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8ad6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




