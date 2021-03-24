---
title: Обновление deviceComplianceScriptRunSummary
description: Обновление свойств объекта deviceComplianceScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7bbd7d35373caaaf9a463955fa3de09025839e38
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130765"
---
# <a name="update-devicecompliancescriptrunsummary"></a><span data-ttu-id="e810d-103">Обновление deviceComplianceScriptRunSummary</span><span class="sxs-lookup"><span data-stu-id="e810d-103">Update deviceComplianceScriptRunSummary</span></span>

<span data-ttu-id="e810d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e810d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e810d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e810d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e810d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e810d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e810d-107">Обновление свойств объекта [deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="e810d-107">Update the properties of a [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e810d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e810d-108">Prerequisites</span></span>
<span data-ttu-id="e810d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e810d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e810d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e810d-111">Permission type</span></span>|<span data-ttu-id="e810d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e810d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e810d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e810d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e810d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e810d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e810d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e810d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e810d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e810d-116">Not supported.</span></span>|
|<span data-ttu-id="e810d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="e810d-117">Application</span></span>|<span data-ttu-id="e810d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e810d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e810d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e810d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="e810d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e810d-120">Request headers</span></span>
|<span data-ttu-id="e810d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e810d-121">Header</span></span>|<span data-ttu-id="e810d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e810d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e810d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e810d-123">Authorization</span></span>|<span data-ttu-id="e810d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e810d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e810d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e810d-125">Accept</span></span>|<span data-ttu-id="e810d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e810d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e810d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e810d-127">Request body</span></span>
<span data-ttu-id="e810d-128">В теле запроса поставляем представление JSON для [объекта deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="e810d-128">In the request body, supply a JSON representation for the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object.</span></span>

<span data-ttu-id="e810d-129">В следующей таблице показаны свойства, необходимые при создании [устройстваComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)</span><span class="sxs-lookup"><span data-stu-id="e810d-129">The following table shows the properties that are required when you create the [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md).</span></span>

|<span data-ttu-id="e810d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e810d-130">Property</span></span>|<span data-ttu-id="e810d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e810d-131">Type</span></span>|<span data-ttu-id="e810d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e810d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e810d-133">id</span><span class="sxs-lookup"><span data-stu-id="e810d-133">id</span></span>|<span data-ttu-id="e810d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e810d-134">String</span></span>|<span data-ttu-id="e810d-135">Клавиша скрипта соответствия устройству запускать сводную сущность.</span><span class="sxs-lookup"><span data-stu-id="e810d-135">Key of the device compliance script run summary entity.</span></span> <span data-ttu-id="e810d-136">Это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e810d-136">This property is read-only.</span></span>|
|<span data-ttu-id="e810d-137">noIssueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e810d-137">noIssueDetectedDeviceCount</span></span>|<span data-ttu-id="e810d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="e810d-138">Int32</span></span>|<span data-ttu-id="e810d-139">Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым.</span><span class="sxs-lookup"><span data-stu-id="e810d-139">Number of devices for which the detection script did not find an issue and the device is healthy.</span></span> <span data-ttu-id="e810d-140">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e810d-140">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e810d-141">issueDetectedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e810d-141">issueDetectedDeviceCount</span></span>|<span data-ttu-id="e810d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e810d-142">Int32</span></span>|<span data-ttu-id="e810d-143">Количество устройств, для которых скрипт обнаружения обнаружил проблему.</span><span class="sxs-lookup"><span data-stu-id="e810d-143">Number of devices for which the detection script found an issue.</span></span> <span data-ttu-id="e810d-144">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e810d-144">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e810d-145">detectionScriptErrorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e810d-145">detectionScriptErrorDeviceCount</span></span>|<span data-ttu-id="e810d-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e810d-146">Int32</span></span>|<span data-ttu-id="e810d-147">Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена.</span><span class="sxs-lookup"><span data-stu-id="e810d-147">Number of devices on which the detection script execution encountered an error and did not complete.</span></span> <span data-ttu-id="e810d-148">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e810d-148">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e810d-149">detectionScriptPendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e810d-149">detectionScriptPendingDeviceCount</span></span>|<span data-ttu-id="e810d-150">Int32</span><span class="sxs-lookup"><span data-stu-id="e810d-150">Int32</span></span>|<span data-ttu-id="e810d-151">Количество устройств, которые еще не запускают последнюю версию сценария соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="e810d-151">Number of devices which have not yet run the latest version of the device compliance script.</span></span> <span data-ttu-id="e810d-152">Допустимые значения -2147483648 до 2147483647</span><span class="sxs-lookup"><span data-stu-id="e810d-152">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="e810d-153">lastScriptRunDateTime</span><span class="sxs-lookup"><span data-stu-id="e810d-153">lastScriptRunDateTime</span></span>|<span data-ttu-id="e810d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e810d-154">DateTimeOffset</span></span>|<span data-ttu-id="e810d-155">Время последнего запуска сценария на всех устройствах</span><span class="sxs-lookup"><span data-stu-id="e810d-155">Last run time for the script across all devices</span></span>|



## <a name="response"></a><span data-ttu-id="e810d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="e810d-156">Response</span></span>
<span data-ttu-id="e810d-157">В случае успешного использования этот метод возвращает код ответа и обновленный объект `200 OK` [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e810d-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e810d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="e810d-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e810d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="e810d-159">Request</span></span>
<span data-ttu-id="e810d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e810d-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/runSummary
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e810d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="e810d-161">Response</span></span>
<span data-ttu-id="e810d-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e810d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "dad42f14-2f14-dad4-142f-d4da142fd4da",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00"
}
```




