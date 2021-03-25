---
title: Обновление userExperienceAnalyticsNotAutopilotReadyDevice
description: Обновление свойств объекта userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f65af4455834540609854708078bd8b62cbb6a1d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159488"
---
# <a name="update-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="ffb36-103">Обновление userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="ffb36-103">Update userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="ffb36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffb36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ffb36-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb36-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ffb36-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ffb36-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ffb36-107">Обновление свойств объекта [userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="ffb36-107">Update the properties of a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ffb36-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ffb36-108">Prerequisites</span></span>
<span data-ttu-id="ffb36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffb36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb36-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb36-111">Permission type</span></span>|<span data-ttu-id="ffb36-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffb36-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffb36-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffb36-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ffb36-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb36-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ffb36-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffb36-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffb36-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb36-116">Not supported.</span></span>|
|<span data-ttu-id="ffb36-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ffb36-117">Application</span></span>|<span data-ttu-id="ffb36-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb36-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffb36-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffb36-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="ffb36-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ffb36-120">Request headers</span></span>
|<span data-ttu-id="ffb36-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffb36-121">Header</span></span>|<span data-ttu-id="ffb36-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ffb36-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffb36-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffb36-123">Authorization</span></span>|<span data-ttu-id="ffb36-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffb36-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffb36-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ffb36-125">Accept</span></span>|<span data-ttu-id="ffb36-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb36-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb36-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffb36-127">Request body</span></span>
<span data-ttu-id="ffb36-128">В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="ffb36-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

<span data-ttu-id="ffb36-129">В следующей таблице показаны свойства, необходимые при создании [пользователяExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="ffb36-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md).</span></span>

|<span data-ttu-id="ffb36-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffb36-130">Property</span></span>|<span data-ttu-id="ffb36-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ffb36-131">Type</span></span>|<span data-ttu-id="ffb36-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ffb36-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffb36-133">id</span><span class="sxs-lookup"><span data-stu-id="ffb36-133">id</span></span>|<span data-ttu-id="ffb36-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ffb36-134">String</span></span>|<span data-ttu-id="ffb36-135">Уникальный идентификатор устройства intune аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ffb36-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="ffb36-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="ffb36-136">deviceName</span></span>|<span data-ttu-id="ffb36-137">String</span><span class="sxs-lookup"><span data-stu-id="ffb36-137">String</span></span>|<span data-ttu-id="ffb36-138">Имя устройства intune.</span><span class="sxs-lookup"><span data-stu-id="ffb36-138">The intune device's name.</span></span>|
|<span data-ttu-id="ffb36-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ffb36-139">serialNumber</span></span>|<span data-ttu-id="ffb36-140">String</span><span class="sxs-lookup"><span data-stu-id="ffb36-140">String</span></span>|<span data-ttu-id="ffb36-141">Серийный номер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="ffb36-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="ffb36-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ffb36-142">manufacturer</span></span>|<span data-ttu-id="ffb36-143">String</span><span class="sxs-lookup"><span data-stu-id="ffb36-143">String</span></span>|<span data-ttu-id="ffb36-144">Производитель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="ffb36-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="ffb36-145">model</span><span class="sxs-lookup"><span data-stu-id="ffb36-145">model</span></span>|<span data-ttu-id="ffb36-146">String</span><span class="sxs-lookup"><span data-stu-id="ffb36-146">String</span></span>|<span data-ttu-id="ffb36-147">Модель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="ffb36-147">The intune device's model.</span></span>|
|<span data-ttu-id="ffb36-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="ffb36-148">managedBy</span></span>|<span data-ttu-id="ffb36-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ffb36-149">String</span></span>|<span data-ttu-id="ffb36-150">Устройство intune управляется.</span><span class="sxs-lookup"><span data-stu-id="ffb36-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="ffb36-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="ffb36-151">autoPilotRegistered</span></span>|<span data-ttu-id="ffb36-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffb36-152">Boolean</span></span>|<span data-ttu-id="ffb36-153">Автопилотрегистер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="ffb36-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="ffb36-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="ffb36-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="ffb36-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="ffb36-155">Boolean</span></span>|<span data-ttu-id="ffb36-156">Автопилот Устройства intuneProfileAssigned.</span><span class="sxs-lookup"><span data-stu-id="ffb36-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="ffb36-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="ffb36-157">azureAdRegistered</span></span>|[<span data-ttu-id="ffb36-158">azureAdRegisteredState</span><span class="sxs-lookup"><span data-stu-id="ffb36-158">azureAdRegisteredState</span></span>](../resources/intune-devices-azureadregisteredstate.md)|<span data-ttu-id="ffb36-159">Устройство intune azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="ffb36-159">The intune device's azureAdRegistered.</span></span> <span data-ttu-id="ffb36-160">Возможные значения: `no`, `yes`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="ffb36-160">Possible values are: `no`, `yes`, `unknown`.</span></span>|
|<span data-ttu-id="ffb36-161">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="ffb36-161">azureAdJoinType</span></span>|<span data-ttu-id="ffb36-162">Строка</span><span class="sxs-lookup"><span data-stu-id="ffb36-162">String</span></span>|<span data-ttu-id="ffb36-163">Azure Ad ad для устройства intune присоединяется кType.</span><span class="sxs-lookup"><span data-stu-id="ffb36-163">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="ffb36-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffb36-164">Response</span></span>
<span data-ttu-id="ffb36-165">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ffb36-165">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb36-166">Пример</span><span class="sxs-lookup"><span data-stu-id="ffb36-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb36-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffb36-167">Request</span></span>
<span data-ttu-id="ffb36-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffb36-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
Content-type: application/json
Content-length: 422

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="ffb36-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffb36-169">Response</span></span>
<span data-ttu-id="ffb36-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffb36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "11c3ffd7-ffd7-11c3-d7ff-c311d7ffc311",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": "yes",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




