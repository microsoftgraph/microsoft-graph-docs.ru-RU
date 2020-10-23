---
title: Создание Рестриктедаппсвиолатион
description: Создание нового объекта Рестриктедаппсвиолатион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cf4e7e67fb77afea84281dc586e65e195f2165ea
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48732981"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="e4421-103">Создание Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="e4421-103">Create restrictedAppsViolation</span></span>

<span data-ttu-id="e4421-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4421-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4421-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4421-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4421-107">Создание нового объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="e4421-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4421-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e4421-108">Prerequisites</span></span>
<span data-ttu-id="e4421-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4421-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4421-111">Permission type</span></span>|<span data-ttu-id="e4421-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4421-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4421-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4421-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4421-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4421-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4421-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4421-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4421-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4421-116">Not supported.</span></span>|
|<span data-ttu-id="e4421-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4421-117">Application</span></span>|<span data-ttu-id="e4421-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4421-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4421-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4421-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="e4421-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e4421-120">Request headers</span></span>
|<span data-ttu-id="e4421-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4421-121">Header</span></span>|<span data-ttu-id="e4421-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e4421-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4421-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4421-123">Authorization</span></span>|<span data-ttu-id="e4421-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4421-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4421-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4421-125">Accept</span></span>|<span data-ttu-id="e4421-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4421-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4421-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e4421-127">Request body</span></span>
<span data-ttu-id="e4421-128">В тексте запроса добавьте представление объекта Рестриктедаппсвиолатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4421-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="e4421-129">В следующей таблице приведены свойства, необходимые при создании Рестриктедаппсвиолатион.</span><span class="sxs-lookup"><span data-stu-id="e4421-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="e4421-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4421-130">Property</span></span>|<span data-ttu-id="e4421-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4421-131">Type</span></span>|<span data-ttu-id="e4421-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4421-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4421-133">id</span><span class="sxs-lookup"><span data-stu-id="e4421-133">id</span></span>|<span data-ttu-id="e4421-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e4421-134">String</span></span>|<span data-ttu-id="e4421-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="e4421-135">Unique identifier for the object.</span></span> <span data-ttu-id="e4421-136">Состоит из accountId, deviceId, Полициид и userId</span><span class="sxs-lookup"><span data-stu-id="e4421-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="e4421-137">userId</span><span class="sxs-lookup"><span data-stu-id="e4421-137">userId</span></span>|<span data-ttu-id="e4421-138">String</span><span class="sxs-lookup"><span data-stu-id="e4421-138">String</span></span>|<span data-ttu-id="e4421-139">Уникальный идентификатор пользователя, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="e4421-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e4421-140">userName</span><span class="sxs-lookup"><span data-stu-id="e4421-140">userName</span></span>|<span data-ttu-id="e4421-141">String</span><span class="sxs-lookup"><span data-stu-id="e4421-141">String</span></span>|<span data-ttu-id="e4421-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="e4421-142">User name</span></span>|
|<span data-ttu-id="e4421-143">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="e4421-143">managedDeviceId</span></span>|<span data-ttu-id="e4421-144">Строка</span><span class="sxs-lookup"><span data-stu-id="e4421-144">String</span></span>|<span data-ttu-id="e4421-145">Уникальный идентификатор управляемого устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="e4421-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e4421-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="e4421-146">deviceName</span></span>|<span data-ttu-id="e4421-147">String</span><span class="sxs-lookup"><span data-stu-id="e4421-147">String</span></span>|<span data-ttu-id="e4421-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="e4421-148">Device name</span></span>|
|<span data-ttu-id="e4421-149">девицеконфигуратионид</span><span class="sxs-lookup"><span data-stu-id="e4421-149">deviceConfigurationId</span></span>|<span data-ttu-id="e4421-150">Строка</span><span class="sxs-lookup"><span data-stu-id="e4421-150">String</span></span>|<span data-ttu-id="e4421-151">Уникальный идентификатор профиля конфигурации устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="e4421-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="e4421-152">девицеконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="e4421-152">deviceConfigurationName</span></span>|<span data-ttu-id="e4421-153">Строка</span><span class="sxs-lookup"><span data-stu-id="e4421-153">String</span></span>|<span data-ttu-id="e4421-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="e4421-154">Device configuration profile name</span></span>|
|<span data-ttu-id="e4421-155">platformType</span><span class="sxs-lookup"><span data-stu-id="e4421-155">platformType</span></span>|[<span data-ttu-id="e4421-156">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="e4421-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="e4421-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="e4421-157">Platform type.</span></span> <span data-ttu-id="e4421-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="e4421-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="e4421-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e4421-159">restrictedAppsState</span></span>|[<span data-ttu-id="e4421-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="e4421-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="e4421-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="e4421-161">Restricted apps state.</span></span> <span data-ttu-id="e4421-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="e4421-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="e4421-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="e4421-163">restrictedApps</span></span>|<span data-ttu-id="e4421-164">Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e4421-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="e4421-165">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="e4421-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="e4421-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4421-166">Response</span></span>
<span data-ttu-id="e4421-167">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4421-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4421-168">Пример</span><span class="sxs-lookup"><span data-stu-id="e4421-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4421-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4421-169">Request</span></span>
<span data-ttu-id="e4421-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4421-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4421-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4421-171">Response</span></span>
<span data-ttu-id="e4421-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4421-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





