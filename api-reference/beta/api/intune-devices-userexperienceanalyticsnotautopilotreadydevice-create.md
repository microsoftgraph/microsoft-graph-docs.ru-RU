---
title: Создание userExperienceAnalyticsNotAutopilotReadyDevice
description: Создание нового объекта userExperienceAnalyticsNotAutopilotReadyDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3842a478ab89e03366a111a52aed901613959dce
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159472"
---
# <a name="create-userexperienceanalyticsnotautopilotreadydevice"></a><span data-ttu-id="b614b-103">Создание userExperienceAnalyticsNotAutopilotReadyDevice</span><span class="sxs-lookup"><span data-stu-id="b614b-103">Create userExperienceAnalyticsNotAutopilotReadyDevice</span></span>

<span data-ttu-id="b614b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b614b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b614b-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b614b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b614b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b614b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b614b-107">Создание нового [объекта userExperienceAnalyticsNotAutopilotReadyDevice.](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md)</span><span class="sxs-lookup"><span data-stu-id="b614b-107">Create a new [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b614b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="b614b-108">Prerequisites</span></span>
<span data-ttu-id="b614b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b614b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b614b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b614b-111">Permission type</span></span>|<span data-ttu-id="b614b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b614b-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b614b-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b614b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b614b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b614b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b614b-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b614b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b614b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b614b-116">Not supported.</span></span>|
|<span data-ttu-id="b614b-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="b614b-117">Application</span></span>|<span data-ttu-id="b614b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b614b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b614b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b614b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
```

## <a name="request-headers"></a><span data-ttu-id="b614b-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b614b-120">Request headers</span></span>
|<span data-ttu-id="b614b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b614b-121">Header</span></span>|<span data-ttu-id="b614b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b614b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b614b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b614b-123">Authorization</span></span>|<span data-ttu-id="b614b-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b614b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b614b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b614b-125">Accept</span></span>|<span data-ttu-id="b614b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b614b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b614b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b614b-127">Request body</span></span>
<span data-ttu-id="b614b-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="b614b-128">In the request body, supply a JSON representation for the userExperienceAnalyticsNotAutopilotReadyDevice object.</span></span>

<span data-ttu-id="b614b-129">В следующей таблице показаны свойства, необходимые при создании пользователяExperienceAnalyticsNotAutopilotReadyDevice.</span><span class="sxs-lookup"><span data-stu-id="b614b-129">The following table shows the properties that are required when you create the userExperienceAnalyticsNotAutopilotReadyDevice.</span></span>

|<span data-ttu-id="b614b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="b614b-130">Property</span></span>|<span data-ttu-id="b614b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="b614b-131">Type</span></span>|<span data-ttu-id="b614b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="b614b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b614b-133">id</span><span class="sxs-lookup"><span data-stu-id="b614b-133">id</span></span>|<span data-ttu-id="b614b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="b614b-134">String</span></span>|<span data-ttu-id="b614b-135">Уникальный идентификатор устройства intune аналитики пользовательского интерфейса.</span><span class="sxs-lookup"><span data-stu-id="b614b-135">The unique identifier of the user experience analytics intune device.</span></span>|
|<span data-ttu-id="b614b-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="b614b-136">deviceName</span></span>|<span data-ttu-id="b614b-137">String</span><span class="sxs-lookup"><span data-stu-id="b614b-137">String</span></span>|<span data-ttu-id="b614b-138">Имя устройства intune.</span><span class="sxs-lookup"><span data-stu-id="b614b-138">The intune device's name.</span></span>|
|<span data-ttu-id="b614b-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b614b-139">serialNumber</span></span>|<span data-ttu-id="b614b-140">String</span><span class="sxs-lookup"><span data-stu-id="b614b-140">String</span></span>|<span data-ttu-id="b614b-141">Серийный номер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="b614b-141">The intune device's serial number.</span></span>|
|<span data-ttu-id="b614b-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b614b-142">manufacturer</span></span>|<span data-ttu-id="b614b-143">String</span><span class="sxs-lookup"><span data-stu-id="b614b-143">String</span></span>|<span data-ttu-id="b614b-144">Производитель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="b614b-144">The intune device's manufacturer.</span></span>|
|<span data-ttu-id="b614b-145">model</span><span class="sxs-lookup"><span data-stu-id="b614b-145">model</span></span>|<span data-ttu-id="b614b-146">String</span><span class="sxs-lookup"><span data-stu-id="b614b-146">String</span></span>|<span data-ttu-id="b614b-147">Модель устройства intune.</span><span class="sxs-lookup"><span data-stu-id="b614b-147">The intune device's model.</span></span>|
|<span data-ttu-id="b614b-148">managedBy</span><span class="sxs-lookup"><span data-stu-id="b614b-148">managedBy</span></span>|<span data-ttu-id="b614b-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b614b-149">String</span></span>|<span data-ttu-id="b614b-150">Устройство intune управляется.</span><span class="sxs-lookup"><span data-stu-id="b614b-150">The intune device's managed by.</span></span>|
|<span data-ttu-id="b614b-151">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="b614b-151">autoPilotRegistered</span></span>|<span data-ttu-id="b614b-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="b614b-152">Boolean</span></span>|<span data-ttu-id="b614b-153">Автопилотрегистер устройства intune.</span><span class="sxs-lookup"><span data-stu-id="b614b-153">The intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="b614b-154">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="b614b-154">autoPilotProfileAssigned</span></span>|<span data-ttu-id="b614b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="b614b-155">Boolean</span></span>|<span data-ttu-id="b614b-156">Автопилот Устройства intuneProfileAssigned.</span><span class="sxs-lookup"><span data-stu-id="b614b-156">The intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="b614b-157">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="b614b-157">azureAdRegistered</span></span>|[<span data-ttu-id="b614b-158">azureAdRegisteredState</span><span class="sxs-lookup"><span data-stu-id="b614b-158">azureAdRegisteredState</span></span>](../resources/intune-devices-azureadregisteredstate.md)|<span data-ttu-id="b614b-159">Устройство intune azureAdRegistered.</span><span class="sxs-lookup"><span data-stu-id="b614b-159">The intune device's azureAdRegistered.</span></span> <span data-ttu-id="b614b-160">Возможные значения: `no`, `yes`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="b614b-160">Possible values are: `no`, `yes`, `unknown`.</span></span>|
|<span data-ttu-id="b614b-161">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="b614b-161">azureAdJoinType</span></span>|<span data-ttu-id="b614b-162">Строка</span><span class="sxs-lookup"><span data-stu-id="b614b-162">String</span></span>|<span data-ttu-id="b614b-163">Azure Ad ad для устройства intune присоединяется кType.</span><span class="sxs-lookup"><span data-stu-id="b614b-163">The intune device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="b614b-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="b614b-164">Response</span></span>
<span data-ttu-id="b614b-165">В случае успеха этот метод возвращает код ответа и `201 Created` [объект userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b614b-165">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/intune-devices-userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b614b-166">Пример</span><span class="sxs-lookup"><span data-stu-id="b614b-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="b614b-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="b614b-167">Request</span></span>
<span data-ttu-id="b614b-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b614b-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice
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

### <a name="response"></a><span data-ttu-id="b614b-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="b614b-169">Response</span></span>
<span data-ttu-id="b614b-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b614b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




