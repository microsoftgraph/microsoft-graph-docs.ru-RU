---
title: Обновление Рестриктедаппсвиолатион
description: Обновление свойств объекта Рестриктедаппсвиолатион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2acc4245d07ddffe90bc87c70c116c8666af98c2
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39947829"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="85a59-103">Обновление Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="85a59-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="85a59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85a59-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="85a59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85a59-106">Обновление свойств объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="85a59-106">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="85a59-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="85a59-107">Prerequisites</span></span>
<span data-ttu-id="85a59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85a59-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85a59-110">Permission type</span></span>|<span data-ttu-id="85a59-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="85a59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="85a59-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85a59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="85a59-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85a59-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="85a59-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85a59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="85a59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85a59-115">Not supported.</span></span>|
|<span data-ttu-id="85a59-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85a59-116">Application</span></span>|<span data-ttu-id="85a59-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85a59-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="85a59-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85a59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="85a59-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="85a59-119">Request headers</span></span>
|<span data-ttu-id="85a59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="85a59-120">Header</span></span>|<span data-ttu-id="85a59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="85a59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="85a59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85a59-122">Authorization</span></span>|<span data-ttu-id="85a59-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85a59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="85a59-124">Accept</span><span class="sxs-lookup"><span data-stu-id="85a59-124">Accept</span></span>|<span data-ttu-id="85a59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="85a59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="85a59-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85a59-126">Request body</span></span>
<span data-ttu-id="85a59-127">В тексте запроса добавьте представление объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85a59-127">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="85a59-128">В следующей таблице приведены свойства, необходимые при создании [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="85a59-128">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="85a59-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="85a59-129">Property</span></span>|<span data-ttu-id="85a59-130">Тип</span><span class="sxs-lookup"><span data-stu-id="85a59-130">Type</span></span>|<span data-ttu-id="85a59-131">Описание</span><span class="sxs-lookup"><span data-stu-id="85a59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85a59-132">id</span><span class="sxs-lookup"><span data-stu-id="85a59-132">id</span></span>|<span data-ttu-id="85a59-133">Строка</span><span class="sxs-lookup"><span data-stu-id="85a59-133">String</span></span>|<span data-ttu-id="85a59-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="85a59-134">Unique identifier for the object.</span></span> <span data-ttu-id="85a59-135">Состоит из accountId, deviceId, Полициид и userId</span><span class="sxs-lookup"><span data-stu-id="85a59-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="85a59-136">userId</span><span class="sxs-lookup"><span data-stu-id="85a59-136">userId</span></span>|<span data-ttu-id="85a59-137">String</span><span class="sxs-lookup"><span data-stu-id="85a59-137">String</span></span>|<span data-ttu-id="85a59-138">Уникальный идентификатор пользователя, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="85a59-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="85a59-139">userName</span><span class="sxs-lookup"><span data-stu-id="85a59-139">userName</span></span>|<span data-ttu-id="85a59-140">String</span><span class="sxs-lookup"><span data-stu-id="85a59-140">String</span></span>|<span data-ttu-id="85a59-141">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="85a59-141">User name</span></span>|
|<span data-ttu-id="85a59-142">манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="85a59-142">managedDeviceId</span></span>|<span data-ttu-id="85a59-143">Строка</span><span class="sxs-lookup"><span data-stu-id="85a59-143">String</span></span>|<span data-ttu-id="85a59-144">Уникальный идентификатор управляемого устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="85a59-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="85a59-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="85a59-145">deviceName</span></span>|<span data-ttu-id="85a59-146">Строка</span><span class="sxs-lookup"><span data-stu-id="85a59-146">String</span></span>|<span data-ttu-id="85a59-147">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="85a59-147">Device name</span></span>|
|<span data-ttu-id="85a59-148">девицеконфигуратионид</span><span class="sxs-lookup"><span data-stu-id="85a59-148">deviceConfigurationId</span></span>|<span data-ttu-id="85a59-149">Строка</span><span class="sxs-lookup"><span data-stu-id="85a59-149">String</span></span>|<span data-ttu-id="85a59-150">Уникальный идентификатор профиля конфигурации устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="85a59-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="85a59-151">девицеконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="85a59-151">deviceConfigurationName</span></span>|<span data-ttu-id="85a59-152">Строка</span><span class="sxs-lookup"><span data-stu-id="85a59-152">String</span></span>|<span data-ttu-id="85a59-153">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="85a59-153">Device configuration profile name</span></span>|
|<span data-ttu-id="85a59-154">platformType</span><span class="sxs-lookup"><span data-stu-id="85a59-154">platformType</span></span>|[<span data-ttu-id="85a59-155">полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="85a59-155">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="85a59-156">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="85a59-156">Platform type.</span></span> <span data-ttu-id="85a59-157">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="85a59-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="85a59-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="85a59-158">restrictedAppsState</span></span>|[<span data-ttu-id="85a59-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="85a59-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="85a59-160">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="85a59-160">Restricted apps state.</span></span> <span data-ttu-id="85a59-161">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="85a59-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="85a59-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="85a59-162">restrictedApps</span></span>|<span data-ttu-id="85a59-163">Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="85a59-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="85a59-164">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="85a59-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="85a59-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="85a59-165">Response</span></span>
<span data-ttu-id="85a59-166">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85a59-166">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85a59-167">Пример</span><span class="sxs-lookup"><span data-stu-id="85a59-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="85a59-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="85a59-168">Request</span></span>
<span data-ttu-id="85a59-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85a59-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="85a59-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="85a59-170">Response</span></span>
<span data-ttu-id="85a59-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85a59-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





