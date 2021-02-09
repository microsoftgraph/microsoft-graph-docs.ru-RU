---
title: Создание deviceManagementAutopilotPolicyStatusDetail
description: Создание объекта deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dabf8f2a81a01a696a0402f1cb23771e82c89ce0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154987"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="c8d04-103">Создание deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="c8d04-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="c8d04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d04-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8d04-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d04-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8d04-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8d04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d04-107">Создание объекта [deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="c8d04-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8d04-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c8d04-108">Prerequisites</span></span>
<span data-ttu-id="c8d04-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c8d04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8d04-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c8d04-111">Permission type</span></span>|<span data-ttu-id="c8d04-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c8d04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8d04-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c8d04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8d04-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d04-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8d04-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c8d04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8d04-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8d04-116">Not supported.</span></span>|
|<span data-ttu-id="c8d04-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c8d04-117">Application</span></span>|<span data-ttu-id="c8d04-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8d04-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8d04-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c8d04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="c8d04-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c8d04-120">Request headers</span></span>
|<span data-ttu-id="c8d04-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c8d04-121">Header</span></span>|<span data-ttu-id="c8d04-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c8d04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8d04-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c8d04-123">Authorization</span></span>|<span data-ttu-id="c8d04-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c8d04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8d04-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8d04-125">Accept</span></span>|<span data-ttu-id="c8d04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8d04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8d04-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c8d04-127">Request body</span></span>
<span data-ttu-id="c8d04-128">В теле запроса предопределение представления объекта deviceManagementAutopilotPolicyStatusDetail в JSON.</span><span class="sxs-lookup"><span data-stu-id="c8d04-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="c8d04-129">В следующей таблице показаны свойства, необходимые при создании объекта deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="c8d04-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="c8d04-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8d04-130">Property</span></span>|<span data-ttu-id="c8d04-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c8d04-131">Type</span></span>|<span data-ttu-id="c8d04-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c8d04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d04-133">id</span><span class="sxs-lookup"><span data-stu-id="c8d04-133">id</span></span>|<span data-ttu-id="c8d04-134">String</span><span class="sxs-lookup"><span data-stu-id="c8d04-134">String</span></span>|<span data-ttu-id="c8d04-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="c8d04-135">UUID for the object</span></span>|
|<span data-ttu-id="c8d04-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c8d04-136">displayName</span></span>|<span data-ttu-id="c8d04-137">String</span><span class="sxs-lookup"><span data-stu-id="c8d04-137">String</span></span>|<span data-ttu-id="c8d04-138">Удобное имя политики.</span><span class="sxs-lookup"><span data-stu-id="c8d04-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="c8d04-139">policyType</span><span class="sxs-lookup"><span data-stu-id="c8d04-139">policyType</span></span>|[<span data-ttu-id="c8d04-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="c8d04-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="c8d04-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="c8d04-141">The type of policy.</span></span> <span data-ttu-id="c8d04-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="c8d04-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="c8d04-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c8d04-143">complianceStatus</span></span>|[<span data-ttu-id="c8d04-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="c8d04-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="c8d04-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="c8d04-145">The policy compliance status.</span></span> <span data-ttu-id="c8d04-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="c8d04-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="c8d04-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="c8d04-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="c8d04-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8d04-148">Boolean</span></span>|<span data-ttu-id="c8d04-149">Указывает, отслеживался ли этот выпуск в рамках сеанса синхронизации регистрации при загрузке Autopilot</span><span class="sxs-lookup"><span data-stu-id="c8d04-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="c8d04-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8d04-150">lastReportedDateTime</span></span>|<span data-ttu-id="c8d04-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8d04-151">DateTimeOffset</span></span>|<span data-ttu-id="c8d04-152">Timestamp of the reported policy status</span><span class="sxs-lookup"><span data-stu-id="c8d04-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="c8d04-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="c8d04-153">errorCode</span></span>|<span data-ttu-id="c8d04-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c8d04-154">Int32</span></span>|<span data-ttu-id="c8d04-155">Об ошибке, связанной с состоянием соответствия или выполнения политики.</span><span class="sxs-lookup"><span data-stu-id="c8d04-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="c8d04-156">Код ошибки для состояния принудения имеет приоритет, если он существует.</span><span class="sxs-lookup"><span data-stu-id="c8d04-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="c8d04-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d04-157">Response</span></span>
<span data-ttu-id="c8d04-158">В случае успешного выполнения этот метод возвращает код отклика и объект `201 Created` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c8d04-158">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8d04-159">Пример</span><span class="sxs-lookup"><span data-stu-id="c8d04-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8d04-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8d04-160">Request</span></span>
<span data-ttu-id="c8d04-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c8d04-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
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

### <a name="response"></a><span data-ttu-id="c8d04-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8d04-162">Response</span></span>
<span data-ttu-id="c8d04-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c8d04-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




