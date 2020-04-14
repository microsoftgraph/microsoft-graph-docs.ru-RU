---
title: Обновление Рестриктедаппсвиолатион
description: Обновление свойств объекта Рестриктедаппсвиолатион.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4055cbfd6a25d718e97c0fc874b7d450b19598a6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43431669"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="811c4-103">Обновление Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="811c4-103">Update restrictedAppsViolation</span></span>

<span data-ttu-id="811c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="811c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="811c4-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="811c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="811c4-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="811c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="811c4-107">Обновление свойств объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="811c4-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="811c4-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="811c4-108">Prerequisites</span></span>
<span data-ttu-id="811c4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="811c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="811c4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="811c4-111">Permission type</span></span>|<span data-ttu-id="811c4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="811c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="811c4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="811c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="811c4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="811c4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="811c4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="811c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="811c4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="811c4-116">Not supported.</span></span>|
|<span data-ttu-id="811c4-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="811c4-117">Application</span></span>|<span data-ttu-id="811c4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="811c4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="811c4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="811c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="811c4-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="811c4-120">Request headers</span></span>
|<span data-ttu-id="811c4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="811c4-121">Header</span></span>|<span data-ttu-id="811c4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="811c4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="811c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="811c4-123">Authorization</span></span>|<span data-ttu-id="811c4-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="811c4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="811c4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="811c4-125">Accept</span></span>|<span data-ttu-id="811c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="811c4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="811c4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="811c4-127">Request body</span></span>
<span data-ttu-id="811c4-128">В тексте запроса добавьте представление объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="811c4-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="811c4-129">В следующей таблице приведены свойства, необходимые при создании [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="811c4-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="811c4-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="811c4-130">Property</span></span>|<span data-ttu-id="811c4-131">Тип</span><span class="sxs-lookup"><span data-stu-id="811c4-131">Type</span></span>|<span data-ttu-id="811c4-132">Описание</span><span class="sxs-lookup"><span data-stu-id="811c4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="811c4-133">id</span><span class="sxs-lookup"><span data-stu-id="811c4-133">id</span></span>|<span data-ttu-id="811c4-134">Строка</span><span class="sxs-lookup"><span data-stu-id="811c4-134">String</span></span>|<span data-ttu-id="811c4-135">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="811c4-135">Unique identifier for the object.</span></span> <span data-ttu-id="811c4-136">Состоит из accountId, deviceId, Полициид и userId</span><span class="sxs-lookup"><span data-stu-id="811c4-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="811c4-137">userId</span><span class="sxs-lookup"><span data-stu-id="811c4-137">userId</span></span>|<span data-ttu-id="811c4-138">String</span><span class="sxs-lookup"><span data-stu-id="811c4-138">String</span></span>|<span data-ttu-id="811c4-139">Уникальный идентификатор пользователя, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="811c4-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="811c4-140">userName</span><span class="sxs-lookup"><span data-stu-id="811c4-140">userName</span></span>|<span data-ttu-id="811c4-141">String</span><span class="sxs-lookup"><span data-stu-id="811c4-141">String</span></span>|<span data-ttu-id="811c4-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="811c4-142">User name</span></span>|
|<span data-ttu-id="811c4-143">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="811c4-143">managedDeviceId</span></span>|<span data-ttu-id="811c4-144">String</span><span class="sxs-lookup"><span data-stu-id="811c4-144">String</span></span>|<span data-ttu-id="811c4-145">Уникальный идентификатор управляемого устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="811c4-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="811c4-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="811c4-146">deviceName</span></span>|<span data-ttu-id="811c4-147">String</span><span class="sxs-lookup"><span data-stu-id="811c4-147">String</span></span>|<span data-ttu-id="811c4-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="811c4-148">Device name</span></span>|
|<span data-ttu-id="811c4-149">девицеконфигуратионид</span><span class="sxs-lookup"><span data-stu-id="811c4-149">deviceConfigurationId</span></span>|<span data-ttu-id="811c4-150">String</span><span class="sxs-lookup"><span data-stu-id="811c4-150">String</span></span>|<span data-ttu-id="811c4-151">Уникальный идентификатор профиля конфигурации устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="811c4-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="811c4-152">девицеконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="811c4-152">deviceConfigurationName</span></span>|<span data-ttu-id="811c4-153">String</span><span class="sxs-lookup"><span data-stu-id="811c4-153">String</span></span>|<span data-ttu-id="811c4-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="811c4-154">Device configuration profile name</span></span>|
|<span data-ttu-id="811c4-155">platformType</span><span class="sxs-lookup"><span data-stu-id="811c4-155">platformType</span></span>|[<span data-ttu-id="811c4-156">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="811c4-156">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="811c4-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="811c4-157">Platform type.</span></span> <span data-ttu-id="811c4-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="811c4-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.</span></span>|
|<span data-ttu-id="811c4-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="811c4-159">restrictedAppsState</span></span>|[<span data-ttu-id="811c4-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="811c4-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="811c4-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="811c4-161">Restricted apps state.</span></span> <span data-ttu-id="811c4-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="811c4-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="811c4-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="811c4-163">restrictedApps</span></span>|<span data-ttu-id="811c4-164">Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="811c4-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="811c4-165">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="811c4-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="811c4-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="811c4-166">Response</span></span>
<span data-ttu-id="811c4-167">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="811c4-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="811c4-168">Пример</span><span class="sxs-lookup"><span data-stu-id="811c4-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="811c4-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="811c4-169">Request</span></span>
<span data-ttu-id="811c4-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="811c4-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="811c4-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="811c4-171">Response</span></span>
<span data-ttu-id="811c4-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="811c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



