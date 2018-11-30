---
title: Создание restrictedAppsViolation
description: Создание нового объекта restrictedAppsViolation.
ms.openlocfilehash: 2d43ddf5ae6c5965f67fdb32c4b242fd0a3f82e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078052"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="9619d-103">Создание restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="9619d-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="9619d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9619d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9619d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9619d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9619d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9619d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9619d-107">Создание нового объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="9619d-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9619d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9619d-108">Prerequisites</span></span>
<span data-ttu-id="9619d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9619d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9619d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9619d-111">Permission type</span></span>|<span data-ttu-id="9619d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9619d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9619d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9619d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9619d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9619d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9619d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9619d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9619d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9619d-116">Not supported.</span></span>|
|<span data-ttu-id="9619d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9619d-117">Application</span></span>|<span data-ttu-id="9619d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9619d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9619d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9619d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="9619d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9619d-120">Request headers</span></span>
|<span data-ttu-id="9619d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9619d-121">Header</span></span>|<span data-ttu-id="9619d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9619d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9619d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9619d-123">Authorization</span></span>|<span data-ttu-id="9619d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9619d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9619d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9619d-125">Accept</span></span>|<span data-ttu-id="9619d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9619d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9619d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9619d-127">Request body</span></span>
<span data-ttu-id="9619d-128">В тексте запроса укажите представление JSON для объекта restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="9619d-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="9619d-129">В следующей таблице показаны свойства, которые необходимы для создания restrictedAppsViolation.</span><span class="sxs-lookup"><span data-stu-id="9619d-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="9619d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9619d-130">Property</span></span>|<span data-ttu-id="9619d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9619d-131">Type</span></span>|<span data-ttu-id="9619d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9619d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9619d-133">id</span><span class="sxs-lookup"><span data-stu-id="9619d-133">id</span></span>|<span data-ttu-id="9619d-134">String</span><span class="sxs-lookup"><span data-stu-id="9619d-134">String</span></span>|<span data-ttu-id="9619d-135">Уникальный идентификатор для объекта.</span><span class="sxs-lookup"><span data-stu-id="9619d-135">Unique identifier for the object.</span></span> <span data-ttu-id="9619d-136">Состоит из accountId, deviceId, policyId и идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="9619d-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="9619d-137">userId</span><span class="sxs-lookup"><span data-stu-id="9619d-137">userId</span></span>|<span data-ttu-id="9619d-138">String</span><span class="sxs-lookup"><span data-stu-id="9619d-138">String</span></span>|<span data-ttu-id="9619d-139">Уникальный идентификатор пользователя, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="9619d-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9619d-140">userName</span><span class="sxs-lookup"><span data-stu-id="9619d-140">userName</span></span>|<span data-ttu-id="9619d-141">String</span><span class="sxs-lookup"><span data-stu-id="9619d-141">String</span></span>|<span data-ttu-id="9619d-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="9619d-142">User name</span></span>|
|<span data-ttu-id="9619d-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9619d-143">managedDeviceId</span></span>|<span data-ttu-id="9619d-144">String</span><span class="sxs-lookup"><span data-stu-id="9619d-144">String</span></span>|<span data-ttu-id="9619d-145">Уникальный идентификатор управляемого устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="9619d-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9619d-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="9619d-146">deviceName</span></span>|<span data-ttu-id="9619d-147">String</span><span class="sxs-lookup"><span data-stu-id="9619d-147">String</span></span>|<span data-ttu-id="9619d-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="9619d-148">Device name</span></span>|
|<span data-ttu-id="9619d-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9619d-149">deviceConfigurationId</span></span>|<span data-ttu-id="9619d-150">String</span><span class="sxs-lookup"><span data-stu-id="9619d-150">String</span></span>|<span data-ttu-id="9619d-151">Конфигурация профиля уникальный идентификатор устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="9619d-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9619d-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="9619d-152">deviceConfigurationName</span></span>|<span data-ttu-id="9619d-153">String</span><span class="sxs-lookup"><span data-stu-id="9619d-153">String</span></span>|<span data-ttu-id="9619d-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="9619d-154">Device configuration profile name</span></span>|
|<span data-ttu-id="9619d-155">platformType</span><span class="sxs-lookup"><span data-stu-id="9619d-155">platformType</span></span>|[<span data-ttu-id="9619d-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9619d-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="9619d-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="9619d-157">Platform type.</span></span> <span data-ttu-id="9619d-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="9619d-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="9619d-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9619d-159">restrictedAppsState</span></span>|[<span data-ttu-id="9619d-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9619d-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="9619d-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="9619d-161">Restricted apps state.</span></span> <span data-ttu-id="9619d-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="9619d-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="9619d-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="9619d-163">restrictedApps</span></span>|<span data-ttu-id="9619d-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9619d-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="9619d-165">Список нарушенных ограниченных приложений</span><span class="sxs-lookup"><span data-stu-id="9619d-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="9619d-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="9619d-166">Response</span></span>
<span data-ttu-id="9619d-167">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9619d-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9619d-168">Пример</span><span class="sxs-lookup"><span data-stu-id="9619d-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="9619d-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="9619d-169">Request</span></span>
<span data-ttu-id="9619d-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9619d-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9619d-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="9619d-171">Response</span></span>
<span data-ttu-id="9619d-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9619d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





