---
title: Обновление deviceManagementAutopilotPolicyStatusDetail
description: Обновление свойств объекта deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99a2267deba02e1f253d64452436236d1ae8f49a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134146"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="382a1-103">Обновление deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="382a1-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="382a1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="382a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="382a1-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="382a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="382a1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="382a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="382a1-107">Обновление свойств объекта [deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="382a1-107">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="382a1-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="382a1-108">Prerequisites</span></span>
<span data-ttu-id="382a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="382a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="382a1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="382a1-111">Permission type</span></span>|<span data-ttu-id="382a1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="382a1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="382a1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="382a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="382a1-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382a1-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="382a1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="382a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="382a1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="382a1-116">Not supported.</span></span>|
|<span data-ttu-id="382a1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="382a1-117">Application</span></span>|<span data-ttu-id="382a1-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="382a1-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="382a1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="382a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="382a1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="382a1-120">Request headers</span></span>
|<span data-ttu-id="382a1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="382a1-121">Header</span></span>|<span data-ttu-id="382a1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="382a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="382a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="382a1-123">Authorization</span></span>|<span data-ttu-id="382a1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="382a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="382a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="382a1-125">Accept</span></span>|<span data-ttu-id="382a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="382a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="382a1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="382a1-127">Request body</span></span>
<span data-ttu-id="382a1-128">В корпусе запроса поставляем представление JSON для [объекта deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="382a1-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="382a1-129">В следующей таблице показаны свойства, необходимые при создании [устройстваManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="382a1-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="382a1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="382a1-130">Property</span></span>|<span data-ttu-id="382a1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="382a1-131">Type</span></span>|<span data-ttu-id="382a1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="382a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="382a1-133">id</span><span class="sxs-lookup"><span data-stu-id="382a1-133">id</span></span>|<span data-ttu-id="382a1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="382a1-134">String</span></span>|<span data-ttu-id="382a1-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="382a1-135">UUID for the object</span></span>|
|<span data-ttu-id="382a1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="382a1-136">displayName</span></span>|<span data-ttu-id="382a1-137">Строка</span><span class="sxs-lookup"><span data-stu-id="382a1-137">String</span></span>|<span data-ttu-id="382a1-138">Удобное имя политики.</span><span class="sxs-lookup"><span data-stu-id="382a1-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="382a1-139">policyType</span><span class="sxs-lookup"><span data-stu-id="382a1-139">policyType</span></span>|[<span data-ttu-id="382a1-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="382a1-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="382a1-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="382a1-141">The type of policy.</span></span> <span data-ttu-id="382a1-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="382a1-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="382a1-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="382a1-143">complianceStatus</span></span>|[<span data-ttu-id="382a1-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="382a1-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="382a1-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="382a1-145">The policy compliance status.</span></span> <span data-ttu-id="382a1-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="382a1-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="382a1-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="382a1-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="382a1-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="382a1-148">Boolean</span></span>|<span data-ttu-id="382a1-149">Указывает, отслеживалась ли эта пролиза в рамках сеанса синхронизации синхронизации с загрузкой автопилота.</span><span class="sxs-lookup"><span data-stu-id="382a1-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="382a1-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="382a1-150">lastReportedDateTime</span></span>|<span data-ttu-id="382a1-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="382a1-151">DateTimeOffset</span></span>|<span data-ttu-id="382a1-152">Timestamp состояния политик, о чем сообщалось</span><span class="sxs-lookup"><span data-stu-id="382a1-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="382a1-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="382a1-153">errorCode</span></span>|<span data-ttu-id="382a1-154">Int32</span><span class="sxs-lookup"><span data-stu-id="382a1-154">Int32</span></span>|<span data-ttu-id="382a1-155">Ошибка, связанная со статусом соответствия или правоприменения политики.</span><span class="sxs-lookup"><span data-stu-id="382a1-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="382a1-156">Код ошибки для состояния правоприменения имеет приоритет, если он существует.</span><span class="sxs-lookup"><span data-stu-id="382a1-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="382a1-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="382a1-157">Response</span></span>
<span data-ttu-id="382a1-158">В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="382a1-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="382a1-159">Пример</span><span class="sxs-lookup"><span data-stu-id="382a1-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="382a1-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="382a1-160">Request</span></span>
<span data-ttu-id="382a1-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="382a1-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="382a1-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="382a1-162">Response</span></span>
<span data-ttu-id="382a1-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="382a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




