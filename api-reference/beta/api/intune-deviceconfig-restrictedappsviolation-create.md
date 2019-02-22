---
title: Создание Рестриктедаппсвиолатион
description: Создание нового объекта Рестриктедаппсвиолатион.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbba9348e8b97125651951bdb4df424dc3b9fe47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146405"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="20373-103">Создание Рестриктедаппсвиолатион</span><span class="sxs-lookup"><span data-stu-id="20373-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="20373-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20373-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20373-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20373-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20373-106">Создание нового объекта [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="20373-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20373-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="20373-107">Prerequisites</span></span>
<span data-ttu-id="20373-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="20373-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="20373-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20373-110">Permission type</span></span>|<span data-ttu-id="20373-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20373-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20373-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20373-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20373-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20373-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20373-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20373-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20373-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20373-115">Not supported.</span></span>|
|<span data-ttu-id="20373-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20373-116">Application</span></span>|<span data-ttu-id="20373-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20373-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20373-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20373-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="20373-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20373-119">Request headers</span></span>
|<span data-ttu-id="20373-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20373-120">Header</span></span>|<span data-ttu-id="20373-121">Значение</span><span class="sxs-lookup"><span data-stu-id="20373-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20373-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20373-122">Authorization</span></span>|<span data-ttu-id="20373-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20373-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20373-124">Accept</span><span class="sxs-lookup"><span data-stu-id="20373-124">Accept</span></span>|<span data-ttu-id="20373-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20373-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20373-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20373-126">Request body</span></span>
<span data-ttu-id="20373-127">В тексте запроса добавьте представление объекта Рестриктедаппсвиолатион в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20373-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="20373-128">В следующей таблице приведены свойства, необходимые при создании Рестриктедаппсвиолатион.</span><span class="sxs-lookup"><span data-stu-id="20373-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="20373-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="20373-129">Property</span></span>|<span data-ttu-id="20373-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20373-130">Type</span></span>|<span data-ttu-id="20373-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20373-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20373-132">id</span><span class="sxs-lookup"><span data-stu-id="20373-132">id</span></span>|<span data-ttu-id="20373-133">Строка</span><span class="sxs-lookup"><span data-stu-id="20373-133">String</span></span>|<span data-ttu-id="20373-134">Уникальный идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="20373-134">Unique identifier for the object.</span></span> <span data-ttu-id="20373-135">Состоит из accountId, deviceId, Полициид и userId</span><span class="sxs-lookup"><span data-stu-id="20373-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="20373-136">userId</span><span class="sxs-lookup"><span data-stu-id="20373-136">userId</span></span>|<span data-ttu-id="20373-137">String</span><span class="sxs-lookup"><span data-stu-id="20373-137">String</span></span>|<span data-ttu-id="20373-138">Уникальный идентификатор пользователя, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="20373-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="20373-139">userName</span><span class="sxs-lookup"><span data-stu-id="20373-139">userName</span></span>|<span data-ttu-id="20373-140">String</span><span class="sxs-lookup"><span data-stu-id="20373-140">String</span></span>|<span data-ttu-id="20373-141">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="20373-141">User name</span></span>|
|<span data-ttu-id="20373-142">Манажеддевицеид</span><span class="sxs-lookup"><span data-stu-id="20373-142">managedDeviceId</span></span>|<span data-ttu-id="20373-143">String</span><span class="sxs-lookup"><span data-stu-id="20373-143">String</span></span>|<span data-ttu-id="20373-144">Уникальный идентификатор управляемого устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="20373-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="20373-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="20373-145">deviceName</span></span>|<span data-ttu-id="20373-146">String</span><span class="sxs-lookup"><span data-stu-id="20373-146">String</span></span>|<span data-ttu-id="20373-147">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="20373-147">Device name</span></span>|
|<span data-ttu-id="20373-148">Девицеконфигуратионид</span><span class="sxs-lookup"><span data-stu-id="20373-148">deviceConfigurationId</span></span>|<span data-ttu-id="20373-149">String</span><span class="sxs-lookup"><span data-stu-id="20373-149">String</span></span>|<span data-ttu-id="20373-150">Уникальный идентификатор профиля конфигурации устройства, должен быть GUID</span><span class="sxs-lookup"><span data-stu-id="20373-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="20373-151">Девицеконфигуратионнаме</span><span class="sxs-lookup"><span data-stu-id="20373-151">deviceConfigurationName</span></span>|<span data-ttu-id="20373-152">String</span><span class="sxs-lookup"><span data-stu-id="20373-152">String</span></span>|<span data-ttu-id="20373-153">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="20373-153">Device configuration profile name</span></span>|
|<span data-ttu-id="20373-154">platformType</span><span class="sxs-lookup"><span data-stu-id="20373-154">platformType</span></span>|[<span data-ttu-id="20373-155">Полициплатформтипе</span><span class="sxs-lookup"><span data-stu-id="20373-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="20373-156">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="20373-156">Platform type.</span></span> <span data-ttu-id="20373-157">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="20373-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="20373-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="20373-158">restrictedAppsState</span></span>|[<span data-ttu-id="20373-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="20373-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="20373-160">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="20373-160">Restricted apps state.</span></span> <span data-ttu-id="20373-161">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="20373-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="20373-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="20373-162">restrictedApps</span></span>|<span data-ttu-id="20373-163">Коллекция [манажеддевицерепортедапп](../resources/intune-deviceconfig-manageddevicereportedapp.md)</span><span class="sxs-lookup"><span data-stu-id="20373-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="20373-164">Список нарушенных приложений с ограниченным доступом</span><span class="sxs-lookup"><span data-stu-id="20373-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="20373-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="20373-165">Response</span></span>
<span data-ttu-id="20373-166">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [рестриктедаппсвиолатион](../resources/intune-deviceconfig-restrictedappsviolation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20373-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20373-167">Пример</span><span class="sxs-lookup"><span data-stu-id="20373-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="20373-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="20373-168">Request</span></span>
<span data-ttu-id="20373-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20373-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="20373-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="20373-170">Response</span></span>
<span data-ttu-id="20373-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20373-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




