---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2cb3576941a755cdf14ecf1b7dc4f198baa6183
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469631"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="dafbe-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="dafbe-103">Update iosMobileAppConfiguration</span></span>

<span data-ttu-id="dafbe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dafbe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dafbe-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dafbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dafbe-106">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dafbe-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dafbe-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="dafbe-107">Prerequisites</span></span>
<span data-ttu-id="dafbe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dafbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dafbe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dafbe-110">Permission type</span></span>|<span data-ttu-id="dafbe-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dafbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dafbe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dafbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dafbe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dafbe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dafbe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dafbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dafbe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dafbe-115">Not supported.</span></span>|
|<span data-ttu-id="dafbe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dafbe-116">Application</span></span>|<span data-ttu-id="dafbe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dafbe-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dafbe-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dafbe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dafbe-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dafbe-119">Request headers</span></span>
|<span data-ttu-id="dafbe-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dafbe-120">Header</span></span>|<span data-ttu-id="dafbe-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dafbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dafbe-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dafbe-122">Authorization</span></span>|<span data-ttu-id="dafbe-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dafbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dafbe-124">Accept</span><span class="sxs-lookup"><span data-stu-id="dafbe-124">Accept</span></span>|<span data-ttu-id="dafbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dafbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dafbe-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dafbe-126">Request body</span></span>
<span data-ttu-id="dafbe-127">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dafbe-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="dafbe-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="dafbe-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="dafbe-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="dafbe-129">Property</span></span>|<span data-ttu-id="dafbe-130">Тип</span><span class="sxs-lookup"><span data-stu-id="dafbe-130">Type</span></span>|<span data-ttu-id="dafbe-131">Описание</span><span class="sxs-lookup"><span data-stu-id="dafbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dafbe-132">id</span><span class="sxs-lookup"><span data-stu-id="dafbe-132">id</span></span>|<span data-ttu-id="dafbe-133">String</span><span class="sxs-lookup"><span data-stu-id="dafbe-133">String</span></span>|<span data-ttu-id="dafbe-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dafbe-134">Key of the entity.</span></span> <span data-ttu-id="dafbe-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="dafbe-136">targetedMobileApps</span></span>|<span data-ttu-id="dafbe-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="dafbe-137">String collection</span></span>|<span data-ttu-id="dafbe-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="dafbe-138">the associated app.</span></span> <span data-ttu-id="dafbe-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dafbe-140">createdDateTime</span></span>|<span data-ttu-id="dafbe-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dafbe-141">DateTimeOffset</span></span>|<span data-ttu-id="dafbe-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="dafbe-142">DateTime the object was created.</span></span> <span data-ttu-id="dafbe-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-144">description</span><span class="sxs-lookup"><span data-stu-id="dafbe-144">description</span></span>|<span data-ttu-id="dafbe-145">String</span><span class="sxs-lookup"><span data-stu-id="dafbe-145">String</span></span>|<span data-ttu-id="dafbe-146">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dafbe-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dafbe-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dafbe-148">lastModifiedDateTime</span></span>|<span data-ttu-id="dafbe-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dafbe-149">DateTimeOffset</span></span>|<span data-ttu-id="dafbe-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="dafbe-150">DateTime the object was last modified.</span></span> <span data-ttu-id="dafbe-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-152">displayName</span><span class="sxs-lookup"><span data-stu-id="dafbe-152">displayName</span></span>|<span data-ttu-id="dafbe-153">Строка</span><span class="sxs-lookup"><span data-stu-id="dafbe-153">String</span></span>|<span data-ttu-id="dafbe-154">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dafbe-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dafbe-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-156">версия</span><span class="sxs-lookup"><span data-stu-id="dafbe-156">version</span></span>|<span data-ttu-id="dafbe-157">Int32</span><span class="sxs-lookup"><span data-stu-id="dafbe-157">Int32</span></span>|<span data-ttu-id="dafbe-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="dafbe-158">Version of the device configuration.</span></span> <span data-ttu-id="dafbe-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="dafbe-160">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="dafbe-160">encodedSettingXml</span></span>|<span data-ttu-id="dafbe-161">Двоичный</span><span class="sxs-lookup"><span data-stu-id="dafbe-161">Binary</span></span>|<span data-ttu-id="dafbe-162">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="dafbe-162">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="dafbe-163">параметры</span><span class="sxs-lookup"><span data-stu-id="dafbe-163">settings</span></span>|<span data-ttu-id="dafbe-164">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="dafbe-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="dafbe-165">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="dafbe-165">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="dafbe-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="dafbe-166">Response</span></span>
<span data-ttu-id="dafbe-167">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="dafbe-167">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dafbe-168">Пример</span><span class="sxs-lookup"><span data-stu-id="dafbe-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="dafbe-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="dafbe-169">Request</span></span>
<span data-ttu-id="dafbe-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dafbe-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 534

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dafbe-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="dafbe-171">Response</span></span>
<span data-ttu-id="dafbe-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dafbe-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 706

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "App Config Key value",
      "appConfigKeyType": "integerType",
      "appConfigKeyValue": "App Config Key Value value"
    }
  ]
}
```






