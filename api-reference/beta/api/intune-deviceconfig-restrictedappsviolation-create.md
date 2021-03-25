---
title: Создание restrictedAppsViolation
description: Создайте новый объект restrictedAppsViolation.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e3c614e14193945c84fd60f46205d7803b91da55
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155059"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="1f2df-103">Создание restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="1f2df-103">Create restrictedAppsViolation</span></span>

<span data-ttu-id="1f2df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f2df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f2df-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f2df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f2df-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f2df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f2df-107">Создайте новый [объект restrictedAppsViolation.](../resources/intune-deviceconfig-restrictedappsviolation.md)</span><span class="sxs-lookup"><span data-stu-id="1f2df-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f2df-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="1f2df-108">Prerequisites</span></span>
<span data-ttu-id="1f2df-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f2df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f2df-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f2df-111">Permission type</span></span>|<span data-ttu-id="1f2df-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f2df-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f2df-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f2df-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f2df-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2df-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f2df-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f2df-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f2df-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f2df-116">Not supported.</span></span>|
|<span data-ttu-id="1f2df-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="1f2df-117">Application</span></span>|<span data-ttu-id="1f2df-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f2df-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f2df-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f2df-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="1f2df-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f2df-120">Request headers</span></span>
|<span data-ttu-id="1f2df-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f2df-121">Header</span></span>|<span data-ttu-id="1f2df-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1f2df-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f2df-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f2df-123">Authorization</span></span>|<span data-ttu-id="1f2df-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f2df-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f2df-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f2df-125">Accept</span></span>|<span data-ttu-id="1f2df-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f2df-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f2df-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f2df-127">Request body</span></span>
<span data-ttu-id="1f2df-128">В теле запроса поставляем представление JSON для объекта restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="1f2df-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="1f2df-129">В следующей таблице показаны свойства, необходимые при создании ограниченного доступа кAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="1f2df-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="1f2df-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f2df-130">Property</span></span>|<span data-ttu-id="1f2df-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1f2df-131">Type</span></span>|<span data-ttu-id="1f2df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1f2df-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f2df-133">id</span><span class="sxs-lookup"><span data-stu-id="1f2df-133">id</span></span>|<span data-ttu-id="1f2df-134">Строка</span><span class="sxs-lookup"><span data-stu-id="1f2df-134">String</span></span>|<span data-ttu-id="1f2df-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="1f2df-135">Unique identifier for the object.</span></span> <span data-ttu-id="1f2df-136">Составлено из accountId, deviceId, policyId и userId</span><span class="sxs-lookup"><span data-stu-id="1f2df-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="1f2df-137">userId</span><span class="sxs-lookup"><span data-stu-id="1f2df-137">userId</span></span>|<span data-ttu-id="1f2df-138">String</span><span class="sxs-lookup"><span data-stu-id="1f2df-138">String</span></span>|<span data-ttu-id="1f2df-139">Уникальный идентификатор пользователя должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="1f2df-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="1f2df-140">userName</span><span class="sxs-lookup"><span data-stu-id="1f2df-140">userName</span></span>|<span data-ttu-id="1f2df-141">String</span><span class="sxs-lookup"><span data-stu-id="1f2df-141">String</span></span>|<span data-ttu-id="1f2df-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="1f2df-142">User name</span></span>|
|<span data-ttu-id="1f2df-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f2df-143">managedDeviceId</span></span>|<span data-ttu-id="1f2df-144">Строка</span><span class="sxs-lookup"><span data-stu-id="1f2df-144">String</span></span>|<span data-ttu-id="1f2df-145">Уникальный идентификатор управляемого устройства должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="1f2df-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="1f2df-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="1f2df-146">deviceName</span></span>|<span data-ttu-id="1f2df-147">String</span><span class="sxs-lookup"><span data-stu-id="1f2df-147">String</span></span>|<span data-ttu-id="1f2df-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="1f2df-148">Device name</span></span>|
|<span data-ttu-id="1f2df-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1f2df-149">deviceConfigurationId</span></span>|<span data-ttu-id="1f2df-150">Строка</span><span class="sxs-lookup"><span data-stu-id="1f2df-150">String</span></span>|<span data-ttu-id="1f2df-151">Уникальный идентификатор конфигурации устройства должен быть Guid</span><span class="sxs-lookup"><span data-stu-id="1f2df-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="1f2df-152">DeviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="1f2df-152">deviceConfigurationName</span></span>|<span data-ttu-id="1f2df-153">Строка</span><span class="sxs-lookup"><span data-stu-id="1f2df-153">String</span></span>|<span data-ttu-id="1f2df-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="1f2df-154">Device configuration profile name</span></span>|
|<span data-ttu-id="1f2df-155">platformType</span><span class="sxs-lookup"><span data-stu-id="1f2df-155">platformType</span></span>|[<span data-ttu-id="1f2df-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="1f2df-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="1f2df-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="1f2df-157">Platform type.</span></span> <span data-ttu-id="1f2df-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="1f2df-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="1f2df-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="1f2df-159">restrictedAppsState</span></span>|[<span data-ttu-id="1f2df-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="1f2df-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="1f2df-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="1f2df-161">Restricted apps state.</span></span> <span data-ttu-id="1f2df-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="1f2df-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="1f2df-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="1f2df-163">restrictedApps</span></span>|<span data-ttu-id="1f2df-164">[коллекция managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1f2df-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="1f2df-165">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="1f2df-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="1f2df-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f2df-166">Response</span></span>
<span data-ttu-id="1f2df-167">В случае успешной работы этот метод возвращает код ответа и объект `201 Created` [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1f2df-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f2df-168">Пример</span><span class="sxs-lookup"><span data-stu-id="1f2df-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f2df-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f2df-169">Request</span></span>
<span data-ttu-id="1f2df-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f2df-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
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

### <a name="response"></a><span data-ttu-id="1f2df-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f2df-171">Response</span></span>
<span data-ttu-id="1f2df-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f2df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




