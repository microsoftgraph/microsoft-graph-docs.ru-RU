---
title: Обновление restrictedAppsViolation
description: Обновление свойства объекта restrictedAppsViolation.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 01509691e65410776ba57269c8a7cb9e804ee661
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403856"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="a7ae7-103">Обновление restrictedAppsViolation</span><span class="sxs-lookup"><span data-stu-id="a7ae7-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="a7ae7-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a7ae7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7ae7-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7ae7-107">Обновление свойства объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="a7ae7-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7ae7-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="a7ae7-108">Prerequisites</span></span>
<span data-ttu-id="a7ae7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a7ae7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a7ae7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7ae7-111">Permission type</span></span>|<span data-ttu-id="a7ae7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7ae7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7ae7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7ae7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7ae7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7ae7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7ae7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7ae7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-116">Not supported.</span></span>|
|<span data-ttu-id="a7ae7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7ae7-117">Application</span></span>|<span data-ttu-id="a7ae7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7ae7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7ae7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7ae7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7ae7-120">Request headers</span></span>
|<span data-ttu-id="a7ae7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7ae7-121">Header</span></span>|<span data-ttu-id="a7ae7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a7ae7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7ae7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7ae7-123">Authorization</span></span>|<span data-ttu-id="a7ae7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a7ae7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7ae7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7ae7-125">Accept</span></span>|<span data-ttu-id="a7ae7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7ae7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7ae7-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7ae7-127">Request body</span></span>
<span data-ttu-id="a7ae7-128">В тексте запроса укажите представление JSON для объекта [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="a7ae7-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="a7ae7-129">В следующей таблице показаны свойства, которые необходимы для создания [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span><span class="sxs-lookup"><span data-stu-id="a7ae7-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="a7ae7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7ae7-130">Property</span></span>|<span data-ttu-id="a7ae7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a7ae7-131">Type</span></span>|<span data-ttu-id="a7ae7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a7ae7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7ae7-133">id</span><span class="sxs-lookup"><span data-stu-id="a7ae7-133">id</span></span>|<span data-ttu-id="a7ae7-134">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-134">String</span></span>|<span data-ttu-id="a7ae7-135">Уникальный идентификатор для объекта.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-135">Unique identifier for the object.</span></span> <span data-ttu-id="a7ae7-136">Состоит из accountId, deviceId, policyId и идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="a7ae7-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="a7ae7-137">userId</span><span class="sxs-lookup"><span data-stu-id="a7ae7-137">userId</span></span>|<span data-ttu-id="a7ae7-138">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-138">String</span></span>|<span data-ttu-id="a7ae7-139">Уникальный идентификатор пользователя, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="a7ae7-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a7ae7-140">userName</span><span class="sxs-lookup"><span data-stu-id="a7ae7-140">userName</span></span>|<span data-ttu-id="a7ae7-141">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-141">String</span></span>|<span data-ttu-id="a7ae7-142">Имя пользователя</span><span class="sxs-lookup"><span data-stu-id="a7ae7-142">User name</span></span>|
|<span data-ttu-id="a7ae7-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="a7ae7-143">managedDeviceId</span></span>|<span data-ttu-id="a7ae7-144">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-144">String</span></span>|<span data-ttu-id="a7ae7-145">Уникальный идентификатор управляемого устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="a7ae7-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a7ae7-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="a7ae7-146">deviceName</span></span>|<span data-ttu-id="a7ae7-147">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-147">String</span></span>|<span data-ttu-id="a7ae7-148">Имя устройства</span><span class="sxs-lookup"><span data-stu-id="a7ae7-148">Device name</span></span>|
|<span data-ttu-id="a7ae7-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a7ae7-149">deviceConfigurationId</span></span>|<span data-ttu-id="a7ae7-150">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-150">String</span></span>|<span data-ttu-id="a7ae7-151">Конфигурация профиля уникальный идентификатор устройства, должен быть идентификатор Guid</span><span class="sxs-lookup"><span data-stu-id="a7ae7-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="a7ae7-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="a7ae7-152">deviceConfigurationName</span></span>|<span data-ttu-id="a7ae7-153">String</span><span class="sxs-lookup"><span data-stu-id="a7ae7-153">String</span></span>|<span data-ttu-id="a7ae7-154">Имя профиля конфигурации устройства</span><span class="sxs-lookup"><span data-stu-id="a7ae7-154">Device configuration profile name</span></span>|
|<span data-ttu-id="a7ae7-155">platformType</span><span class="sxs-lookup"><span data-stu-id="a7ae7-155">platformType</span></span>|[<span data-ttu-id="a7ae7-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="a7ae7-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="a7ae7-157">Тип платформы.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-157">Platform type.</span></span> <span data-ttu-id="a7ae7-158">Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="a7ae7-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="a7ae7-159">restrictedAppsState</span></span>|[<span data-ttu-id="a7ae7-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="a7ae7-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="a7ae7-161">Состояние ограниченных приложений.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-161">Restricted apps state.</span></span> <span data-ttu-id="a7ae7-162">Возможные значения: `prohibitedApps`, `notApprovedApps`.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="a7ae7-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="a7ae7-163">restrictedApps</span></span>|<span data-ttu-id="a7ae7-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a7ae7-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="a7ae7-165">Список нарушенных ограниченных приложений</span><span class="sxs-lookup"><span data-stu-id="a7ae7-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="a7ae7-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ae7-166">Response</span></span>
<span data-ttu-id="a7ae7-167">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7ae7-168">Пример</span><span class="sxs-lookup"><span data-stu-id="a7ae7-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7ae7-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7ae7-169">Request</span></span>
<span data-ttu-id="a7ae7-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a7ae7-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7ae7-171">Response</span></span>
<span data-ttu-id="a7ae7-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a7ae7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




