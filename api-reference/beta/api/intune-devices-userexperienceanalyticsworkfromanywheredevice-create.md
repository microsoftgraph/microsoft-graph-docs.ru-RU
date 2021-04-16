---
title: Создание userExperienceAnalyticsWorkFromAnywhereDevice
description: Создание нового объекта userExperienceAnalyticsWorkFromAnywhereDevice.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1cd4db22f691935d53b85eded268650ab0bc12b4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51869034"
---
# <a name="create-userexperienceanalyticsworkfromanywheredevice"></a><span data-ttu-id="15302-103">Создание userExperienceAnalyticsWorkFromAnywhereDevice</span><span class="sxs-lookup"><span data-stu-id="15302-103">Create userExperienceAnalyticsWorkFromAnywhereDevice</span></span>

<span data-ttu-id="15302-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15302-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15302-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15302-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15302-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15302-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15302-107">Создание нового [объекта userExperienceAnalyticsWorkFromAnywhereDevice.](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md)</span><span class="sxs-lookup"><span data-stu-id="15302-107">Create a new [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="15302-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="15302-108">Prerequisites</span></span>
<span data-ttu-id="15302-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="15302-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15302-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="15302-111">Permission type</span></span>|<span data-ttu-id="15302-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="15302-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="15302-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="15302-113">Delegated (work or school account)</span></span>|<span data-ttu-id="15302-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15302-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="15302-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="15302-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="15302-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15302-116">Not supported.</span></span>|
|<span data-ttu-id="15302-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="15302-117">Application</span></span>|<span data-ttu-id="15302-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15302-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="15302-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="15302-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
```

## <a name="request-headers"></a><span data-ttu-id="15302-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="15302-120">Request headers</span></span>
|<span data-ttu-id="15302-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="15302-121">Header</span></span>|<span data-ttu-id="15302-122">Значение</span><span class="sxs-lookup"><span data-stu-id="15302-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="15302-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="15302-123">Authorization</span></span>|<span data-ttu-id="15302-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="15302-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="15302-125">Accept</span><span class="sxs-lookup"><span data-stu-id="15302-125">Accept</span></span>|<span data-ttu-id="15302-126">application/json</span><span class="sxs-lookup"><span data-stu-id="15302-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="15302-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="15302-127">Request body</span></span>
<span data-ttu-id="15302-128">В теле запроса поставляем представление JSON для объекта userExperienceAnalyticsWorkFromAnywhereDevice.</span><span class="sxs-lookup"><span data-stu-id="15302-128">In the request body, supply a JSON representation for the userExperienceAnalyticsWorkFromAnywhereDevice object.</span></span>

<span data-ttu-id="15302-129">В следующей таблице показаны свойства, необходимые при создании userExperienceAnalyticsWorkFromAnywhereDevice.</span><span class="sxs-lookup"><span data-stu-id="15302-129">The following table shows the properties that are required when you create the userExperienceAnalyticsWorkFromAnywhereDevice.</span></span>

|<span data-ttu-id="15302-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="15302-130">Property</span></span>|<span data-ttu-id="15302-131">Тип</span><span class="sxs-lookup"><span data-stu-id="15302-131">Type</span></span>|<span data-ttu-id="15302-132">Описание</span><span class="sxs-lookup"><span data-stu-id="15302-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15302-133">id</span><span class="sxs-lookup"><span data-stu-id="15302-133">id</span></span>|<span data-ttu-id="15302-134">String</span><span class="sxs-lookup"><span data-stu-id="15302-134">String</span></span>|<span data-ttu-id="15302-135">Уникальный идентификатор аналитики пользовательских интерфейсов работает с любого устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-135">The unique identifier of the user experience analytics work from anywhere device.</span></span>|
|<span data-ttu-id="15302-136">deviceName</span><span class="sxs-lookup"><span data-stu-id="15302-136">deviceName</span></span>|<span data-ttu-id="15302-137">String</span><span class="sxs-lookup"><span data-stu-id="15302-137">String</span></span>|<span data-ttu-id="15302-138">Работа из любого имени устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-138">The work from anywhere device's name.</span></span>|
|<span data-ttu-id="15302-139">serialNumber</span><span class="sxs-lookup"><span data-stu-id="15302-139">serialNumber</span></span>|<span data-ttu-id="15302-140">String</span><span class="sxs-lookup"><span data-stu-id="15302-140">String</span></span>|<span data-ttu-id="15302-141">Пользовательский интерфейс работает с любого серийного номера устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-141">The user experience work from anywhere device's serial number.</span></span>|
|<span data-ttu-id="15302-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="15302-142">manufacturer</span></span>|<span data-ttu-id="15302-143">String</span><span class="sxs-lookup"><span data-stu-id="15302-143">String</span></span>|<span data-ttu-id="15302-144">Пользовательский интерфейс работает с любого производителя устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-144">The user experience work from anywhere device's manufacturer.</span></span>|
|<span data-ttu-id="15302-145">model</span><span class="sxs-lookup"><span data-stu-id="15302-145">model</span></span>|<span data-ttu-id="15302-146">String</span><span class="sxs-lookup"><span data-stu-id="15302-146">String</span></span>|<span data-ttu-id="15302-147">Пользовательский интерфейс работает из любой модели устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-147">The user experience work from anywhere device's model.</span></span>|
|<span data-ttu-id="15302-148">владение</span><span class="sxs-lookup"><span data-stu-id="15302-148">ownership</span></span>|<span data-ttu-id="15302-149">String</span><span class="sxs-lookup"><span data-stu-id="15302-149">String</span></span>|<span data-ttu-id="15302-150">Пользовательский интерфейс работает с любого владельца устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-150">The user experience work from anywhere device's ownership.</span></span>|
|<span data-ttu-id="15302-151">managedBy</span><span class="sxs-lookup"><span data-stu-id="15302-151">managedBy</span></span>|<span data-ttu-id="15302-152">String</span><span class="sxs-lookup"><span data-stu-id="15302-152">String</span></span>|<span data-ttu-id="15302-153">Пользовательский интерфейс работает из любого агента управления устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-153">The user experience work from anywhere management agent of the device.</span></span>|
|<span data-ttu-id="15302-154">autoPilotRegistered</span><span class="sxs-lookup"><span data-stu-id="15302-154">autoPilotRegistered</span></span>|<span data-ttu-id="15302-155">Логический</span><span class="sxs-lookup"><span data-stu-id="15302-155">Boolean</span></span>|<span data-ttu-id="15302-156">Пользовательский интерфейс работает с автопилотом устройства intune.</span><span class="sxs-lookup"><span data-stu-id="15302-156">The user experience work from anywhere intune device's autopilotRegistered.</span></span>|
|<span data-ttu-id="15302-157">autoPilotProfileAssigned</span><span class="sxs-lookup"><span data-stu-id="15302-157">autoPilotProfileAssigned</span></span>|<span data-ttu-id="15302-158">Логический</span><span class="sxs-lookup"><span data-stu-id="15302-158">Boolean</span></span>|<span data-ttu-id="15302-159">Аналитика пользовательских интерфейсов работает из любого автопилота устройства intuneProfileAssigned.</span><span class="sxs-lookup"><span data-stu-id="15302-159">The user experience analytics work from anywhere intune device's autopilotProfileAssigned.</span></span>|
|<span data-ttu-id="15302-160">azureAdRegistered</span><span class="sxs-lookup"><span data-stu-id="15302-160">azureAdRegistered</span></span>|<span data-ttu-id="15302-161">Логический</span><span class="sxs-lookup"><span data-stu-id="15302-161">Boolean</span></span>|<span data-ttu-id="15302-162">Пользовательский интерфейс работает с azureAdRegistered любого устройства.</span><span class="sxs-lookup"><span data-stu-id="15302-162">The user experience work from anywhere device's azureAdRegistered.</span></span>|
|<span data-ttu-id="15302-163">azureAdDeviceId</span><span class="sxs-lookup"><span data-stu-id="15302-163">azureAdDeviceId</span></span>|<span data-ttu-id="15302-164">String</span><span class="sxs-lookup"><span data-stu-id="15302-164">String</span></span>|<span data-ttu-id="15302-165">Пользовательский интерфейс работает из любого id-устройства Azure Ad.</span><span class="sxs-lookup"><span data-stu-id="15302-165">The user experience work from anywhere azure Ad device Id.</span></span>|
|<span data-ttu-id="15302-166">azureAdJoinType</span><span class="sxs-lookup"><span data-stu-id="15302-166">azureAdJoinType</span></span>|<span data-ttu-id="15302-167">String</span><span class="sxs-lookup"><span data-stu-id="15302-167">String</span></span>|<span data-ttu-id="15302-168">Пользовательский опыт работы из любого устройства azure Ad joinType.</span><span class="sxs-lookup"><span data-stu-id="15302-168">The user experience work from anywhere device's azure Ad joinType.</span></span>|



## <a name="response"></a><span data-ttu-id="15302-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="15302-169">Response</span></span>
<span data-ttu-id="15302-170">В случае успеха этот метод возвращает код отклика и `201 Created` [объект userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="15302-170">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15302-171">Пример</span><span class="sxs-lookup"><span data-stu-id="15302-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="15302-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="15302-172">Request</span></span>
<span data-ttu-id="15302-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="15302-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```

### <a name="response"></a><span data-ttu-id="15302-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="15302-174">Response</span></span>
<span data-ttu-id="15302-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="15302-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 554

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "83d5adfc-adfc-83d5-fcad-d583fcadd583",
  "deviceName": "Device Name value",
  "serialNumber": "Serial Number value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "ownership": "Ownership value",
  "managedBy": "Managed By value",
  "autoPilotRegistered": true,
  "autoPilotProfileAssigned": true,
  "azureAdRegistered": true,
  "azureAdDeviceId": "Azure Ad Device Id value",
  "azureAdJoinType": "Azure Ad Join Type value"
}
```




