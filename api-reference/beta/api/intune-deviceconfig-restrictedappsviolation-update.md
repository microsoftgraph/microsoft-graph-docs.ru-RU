---
title: Обновление restrictedAppsViolation
description: Обновление свойств объекта restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b0e600358463916219109b1123413d9f69b2d44
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132473"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="72aab-103">Обновление restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="72aab-103">Update restrictedAppsViolation</span></span>

<span data-ttu-id="72aab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72aab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72aab-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72aab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72aab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72aab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72aab-107">Обновление свойств объекта [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="72aab-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72aab-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="72aab-108">Prerequisites</span></span>
<span data-ttu-id="72aab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72aab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72aab-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72aab-111">Permission type</span></span>|<span data-ttu-id="72aab-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72aab-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72aab-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72aab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="72aab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72aab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72aab-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72aab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72aab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72aab-116">Not supported.</span></span>|
|<span data-ttu-id="72aab-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="72aab-117">Application</span></span>|<span data-ttu-id="72aab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72aab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72aab-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72aab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="72aab-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="72aab-120">Request headers</span></span>
|<span data-ttu-id="72aab-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="72aab-121">Header</span></span>|<span data-ttu-id="72aab-122">Значение</span><span class="sxs-lookup"><span data-stu-id="72aab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72aab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="72aab-123">Authorization</span></span>|<span data-ttu-id="72aab-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72aab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72aab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="72aab-125">Accept</span></span>|<span data-ttu-id="72aab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="72aab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72aab-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="72aab-127">Request body</span></span>
<span data-ttu-id="72aab-128">В теле запроса поставляем представление JSON для объекта [restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="72aab-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="72aab-129">В следующей таблице показаны свойства, необходимые при создании [ограниченного доступа кAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="72aab-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="72aab-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="72aab-130">Property</span></span>|<span data-ttu-id="72aab-131">Тип</span><span class="sxs-lookup"><span data-stu-id="72aab-131">Type</span></span>|<span data-ttu-id="72aab-132">Описание</span><span class="sxs-lookup"><span data-stu-id="72aab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72aab-133">id</span><span class="sxs-lookup"><span data-stu-id="72aab-133">id</span></span>|<span data-ttu-id="72aab-134">Строка</span><span class="sxs-lookup"><span data-stu-id="72aab-134">String</span></span>|<span data-ttu-id="72aab-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="72aab-135">Unique identifier for the object.</span></span> <span data-ttu-id="72aab-136">Составлено из accountId, deviceId, policyId и userId</span><span class="sxs-lookup"><span data-stu-id="72aab-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="72aab-137">userId</span><span class="sxs-lookup"><span data-stu-id="72aab-137">userId</span></span>|<span data-ttu-id="72aab-138">String</span><span class="sxs-lookup"><span data-stu-id="72aab-138">String</span></span>|<span data-ttu-id="72aab-139">Уникальный идентификатор пользователя должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="72aab-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="72aab-140">userName</span><span class="sxs-lookup"><span data-stu-id="72aab-140">userName</span></span>|<span data-ttu-id="72aab-141">String</span><span class="sxs-lookup"><span data-stu-id="72aab-141">String</span></span>|<span data-ttu-id="72aab-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="72aab-142">User name</span></span>|
|<span data-ttu-id="72aab-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="72aab-143">managedDeviceId</span></span>|<span data-ttu-id="72aab-144">Строка</span><span class="sxs-lookup"><span data-stu-id="72aab-144">String</span></span>|<span data-ttu-id="72aab-145">Уникальный идентификатор управляемого устройства должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="72aab-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="72aab-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="72aab-146">deviceName</span></span>|<span data-ttu-id="72aab-147">String</span><span class="sxs-lookup"><span data-stu-id="72aab-147">String</span></span>|<span data-ttu-id="72aab-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="72aab-148">Device name</span></span>|
|<span data-ttu-id="72aab-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="72aab-149">deviceConfigurationId</span></span>|<span data-ttu-id="72aab-150">Строка</span><span class="sxs-lookup"><span data-stu-id="72aab-150">String</span></span>|<span data-ttu-id="72aab-151">Уникальный идентификатор конфигурации устройства должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="72aab-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="72aab-152">DeviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="72aab-152">deviceConfigurationName</span></span>|<span data-ttu-id="72aab-153">Строка</span><span class="sxs-lookup"><span data-stu-id="72aab-153">String</span></span>|<span data-ttu-id="72aab-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="72aab-154">Device configuration profile name</span></span>|
|<span data-ttu-id="72aab-155">platformType</span><span class="sxs-lookup"><span data-stu-id="72aab-155">platformType</span></span>|[<span data-ttu-id="72aab-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="72aab-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="72aab-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="72aab-157">Platform type.</span></span> <span data-ttu-id="72aab-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="72aab-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="72aab-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="72aab-159">restrictedAppsState</span></span>|[<span data-ttu-id="72aab-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="72aab-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="72aab-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="72aab-161">Restricted apps state.</span></span> <span data-ttu-id="72aab-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="72aab-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="72aab-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="72aab-163">restrictedApps</span></span>|<span data-ttu-id="72aab-164">[коллекция managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="72aab-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="72aab-165">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="72aab-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="72aab-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="72aab-166">Response</span></span>
<span data-ttu-id="72aab-167">В случае успеха этот метод возвращает код ответа и обновленный объект `200 OK` [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="72aab-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72aab-168">Пример</span><span class="sxs-lookup"><span data-stu-id="72aab-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="72aab-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="72aab-169">Request</span></span>
<span data-ttu-id="72aab-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="72aab-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="72aab-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="72aab-171">Response</span></span>
<span data-ttu-id="72aab-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="72aab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```




