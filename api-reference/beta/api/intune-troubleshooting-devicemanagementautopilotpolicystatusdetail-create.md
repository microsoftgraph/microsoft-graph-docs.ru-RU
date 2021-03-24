---
title: Создание deviceManagementAutopilotPolicyStatusDetail
description: Создание нового объекта deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3f2b6614d980911c35babfa71425a2e5b0ac7e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134201"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="461ff-103">Создание deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="461ff-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="461ff-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="461ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="461ff-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="461ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="461ff-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="461ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="461ff-107">Создание нового [объекта deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="461ff-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="461ff-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="461ff-108">Prerequisites</span></span>
<span data-ttu-id="461ff-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="461ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="461ff-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="461ff-111">Permission type</span></span>|<span data-ttu-id="461ff-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="461ff-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="461ff-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="461ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="461ff-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461ff-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="461ff-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="461ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="461ff-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="461ff-116">Not supported.</span></span>|
|<span data-ttu-id="461ff-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="461ff-117">Application</span></span>|<span data-ttu-id="461ff-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="461ff-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="461ff-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="461ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="461ff-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="461ff-120">Request headers</span></span>
|<span data-ttu-id="461ff-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="461ff-121">Header</span></span>|<span data-ttu-id="461ff-122">Значение</span><span class="sxs-lookup"><span data-stu-id="461ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="461ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="461ff-123">Authorization</span></span>|<span data-ttu-id="461ff-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="461ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="461ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="461ff-125">Accept</span></span>|<span data-ttu-id="461ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="461ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="461ff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="461ff-127">Request body</span></span>
<span data-ttu-id="461ff-128">В корпусе запроса поставляем представление JSON для объекта deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="461ff-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="461ff-129">В следующей таблице показаны свойства, необходимые при создании устройстваManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="461ff-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="461ff-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="461ff-130">Property</span></span>|<span data-ttu-id="461ff-131">Тип</span><span class="sxs-lookup"><span data-stu-id="461ff-131">Type</span></span>|<span data-ttu-id="461ff-132">Описание</span><span class="sxs-lookup"><span data-stu-id="461ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="461ff-133">id</span><span class="sxs-lookup"><span data-stu-id="461ff-133">id</span></span>|<span data-ttu-id="461ff-134">Строка</span><span class="sxs-lookup"><span data-stu-id="461ff-134">String</span></span>|<span data-ttu-id="461ff-135">UUID объекта.</span><span class="sxs-lookup"><span data-stu-id="461ff-135">UUID for the object</span></span>|
|<span data-ttu-id="461ff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="461ff-136">displayName</span></span>|<span data-ttu-id="461ff-137">Строка</span><span class="sxs-lookup"><span data-stu-id="461ff-137">String</span></span>|<span data-ttu-id="461ff-138">Удобное имя политики.</span><span class="sxs-lookup"><span data-stu-id="461ff-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="461ff-139">policyType</span><span class="sxs-lookup"><span data-stu-id="461ff-139">policyType</span></span>|[<span data-ttu-id="461ff-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="461ff-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="461ff-141">Тип политики.</span><span class="sxs-lookup"><span data-stu-id="461ff-141">The type of policy.</span></span> <span data-ttu-id="461ff-142">Возможные значения: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="461ff-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="461ff-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="461ff-143">complianceStatus</span></span>|[<span data-ttu-id="461ff-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="461ff-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="461ff-145">Состояние соответствия политике.</span><span class="sxs-lookup"><span data-stu-id="461ff-145">The policy compliance status.</span></span> <span data-ttu-id="461ff-146">Возможные значения: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="461ff-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="461ff-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="461ff-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="461ff-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="461ff-148">Boolean</span></span>|<span data-ttu-id="461ff-149">Указывает, отслеживалась ли эта пролиза в рамках сеанса синхронизации синхронизации с загрузкой автопилота.</span><span class="sxs-lookup"><span data-stu-id="461ff-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="461ff-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="461ff-150">lastReportedDateTime</span></span>|<span data-ttu-id="461ff-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461ff-151">DateTimeOffset</span></span>|<span data-ttu-id="461ff-152">Timestamp состояния политик, о чем сообщалось</span><span class="sxs-lookup"><span data-stu-id="461ff-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="461ff-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="461ff-153">errorCode</span></span>|<span data-ttu-id="461ff-154">Int32</span><span class="sxs-lookup"><span data-stu-id="461ff-154">Int32</span></span>|<span data-ttu-id="461ff-155">Ошибка, связанная со статусом соответствия или правоприменения политики.</span><span class="sxs-lookup"><span data-stu-id="461ff-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="461ff-156">Код ошибки для состояния правоприменения имеет приоритет, если он существует.</span><span class="sxs-lookup"><span data-stu-id="461ff-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="461ff-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="461ff-157">Response</span></span>
<span data-ttu-id="461ff-158">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="461ff-158">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="461ff-159">Пример</span><span class="sxs-lookup"><span data-stu-id="461ff-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="461ff-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="461ff-160">Request</span></span>
<span data-ttu-id="461ff-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="461ff-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="461ff-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="461ff-162">Response</span></span>
<span data-ttu-id="461ff-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="461ff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




