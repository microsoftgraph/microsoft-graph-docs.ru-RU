---
title: Создание Девицеманажементаутопилотполицистатусдетаил
description: Создание нового объекта Девицеманажементаутопилотполицистатусдетаил.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db4e90778d137b23d6e34d5503df15e137297814
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443426"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="3b930-103">Создание Девицеманажементаутопилотполицистатусдетаил</span><span class="sxs-lookup"><span data-stu-id="3b930-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="3b930-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b930-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b930-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3b930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b930-107">Создание нового объекта [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="3b930-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b930-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="3b930-108">Prerequisites</span></span>
<span data-ttu-id="3b930-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b930-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b930-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3b930-111">Permission type</span></span>|<span data-ttu-id="3b930-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3b930-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b930-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3b930-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b930-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b930-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b930-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3b930-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b930-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3b930-116">Not supported.</span></span>|
|<span data-ttu-id="3b930-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3b930-117">Application</span></span>|<span data-ttu-id="3b930-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b930-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b930-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3b930-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="3b930-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3b930-120">Request headers</span></span>
|<span data-ttu-id="3b930-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3b930-121">Header</span></span>|<span data-ttu-id="3b930-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3b930-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b930-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b930-123">Authorization</span></span>|<span data-ttu-id="3b930-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3b930-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b930-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3b930-125">Accept</span></span>|<span data-ttu-id="3b930-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b930-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b930-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3b930-127">Request body</span></span>
<span data-ttu-id="3b930-128">В тексте запроса добавьте представление объекта Девицеманажементаутопилотполицистатусдетаил в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b930-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="3b930-129">В следующей таблице приведены свойства, необходимые при создании Девицеманажементаутопилотполицистатусдетаил.</span><span class="sxs-lookup"><span data-stu-id="3b930-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="3b930-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b930-130">Property</span></span>|<span data-ttu-id="3b930-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3b930-131">Type</span></span>|<span data-ttu-id="3b930-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3b930-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b930-133">id</span><span class="sxs-lookup"><span data-stu-id="3b930-133">id</span></span>|<span data-ttu-id="3b930-134">String</span><span class="sxs-lookup"><span data-stu-id="3b930-134">String</span></span>|<span data-ttu-id="3b930-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="3b930-135">UUID for the object</span></span>|
|<span data-ttu-id="3b930-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3b930-136">displayName</span></span>|<span data-ttu-id="3b930-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3b930-137">String</span></span>|<span data-ttu-id="3b930-138">Понятное имя политики.</span><span class="sxs-lookup"><span data-stu-id="3b930-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="3b930-139">полицитипе</span><span class="sxs-lookup"><span data-stu-id="3b930-139">policyType</span></span>|[<span data-ttu-id="3b930-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="3b930-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="3b930-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="3b930-141">The type of policy.</span></span> <span data-ttu-id="3b930-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="3b930-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="3b930-143">комплианцестатус</span><span class="sxs-lookup"><span data-stu-id="3b930-143">complianceStatus</span></span>|[<span data-ttu-id="3b930-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="3b930-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="3b930-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="3b930-145">The policy compliance status.</span></span> <span data-ttu-id="3b930-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="3b930-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="3b930-147">траккедоненроллментстатус</span><span class="sxs-lookup"><span data-stu-id="3b930-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="3b930-148">Логическое</span><span class="sxs-lookup"><span data-stu-id="3b930-148">Boolean</span></span>|<span data-ttu-id="3b930-149">Указывает, была ли эта пролици зарегистрирована в рамках сеанса синхронизации автоматической загрузки для автоматической пилотной установки</span><span class="sxs-lookup"><span data-stu-id="3b930-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="3b930-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b930-150">lastReportedDateTime</span></span>|<span data-ttu-id="3b930-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b930-151">DateTimeOffset</span></span>|<span data-ttu-id="3b930-152">Метка времени для отчета о состоянии политики</span><span class="sxs-lookup"><span data-stu-id="3b930-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="3b930-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b930-153">Response</span></span>
<span data-ttu-id="3b930-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементаутопилотполицистатусдетаил](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3b930-154">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b930-155">Пример</span><span class="sxs-lookup"><span data-stu-id="3b930-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b930-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="3b930-156">Request</span></span>
<span data-ttu-id="3b930-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3b930-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
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

### <a name="response"></a><span data-ttu-id="3b930-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="3b930-158">Response</span></span>
<span data-ttu-id="3b930-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3b930-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



