---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
ms.openlocfilehash: dcd89e79b2e3c3008a2ac03a3115e8d766d0f1e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026505"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="1f29c-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f29c-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="1f29c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1f29c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f29c-105">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f29c-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f29c-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="1f29c-106">Prerequisites</span></span>
<span data-ttu-id="1f29c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f29c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f29c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f29c-109">Permission type</span></span>|<span data-ttu-id="1f29c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f29c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f29c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f29c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f29c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f29c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f29c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f29c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f29c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f29c-114">Not supported.</span></span>|
|<span data-ttu-id="1f29c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f29c-115">Application</span></span>|<span data-ttu-id="1f29c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f29c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f29c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f29c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1f29c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1f29c-118">Request headers</span></span>
|<span data-ttu-id="1f29c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f29c-119">Header</span></span>|<span data-ttu-id="1f29c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1f29c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f29c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f29c-121">Authorization</span></span>|<span data-ttu-id="1f29c-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1f29c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f29c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1f29c-123">Accept</span></span>|<span data-ttu-id="1f29c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f29c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f29c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1f29c-125">Request body</span></span>
<span data-ttu-id="1f29c-126">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f29c-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="1f29c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f29c-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="1f29c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f29c-128">Property</span></span>|<span data-ttu-id="1f29c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1f29c-129">Type</span></span>|<span data-ttu-id="1f29c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1f29c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f29c-131">id</span><span class="sxs-lookup"><span data-stu-id="1f29c-131">id</span></span>|<span data-ttu-id="1f29c-132">String</span><span class="sxs-lookup"><span data-stu-id="1f29c-132">String</span></span>|<span data-ttu-id="1f29c-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f29c-133">Key of the entity.</span></span> <span data-ttu-id="1f29c-134">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="1f29c-135">targetedMobileApps</span></span>|<span data-ttu-id="1f29c-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1f29c-136">String collection</span></span>|<span data-ttu-id="1f29c-137">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="1f29c-137">the associated app.</span></span> <span data-ttu-id="1f29c-138">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f29c-139">createdDateTime</span></span>|<span data-ttu-id="1f29c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f29c-140">DateTimeOffset</span></span>|<span data-ttu-id="1f29c-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1f29c-141">DateTime the object was created.</span></span> <span data-ttu-id="1f29c-142">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-143">описание</span><span class="sxs-lookup"><span data-stu-id="1f29c-143">description</span></span>|<span data-ttu-id="1f29c-144">String</span><span class="sxs-lookup"><span data-stu-id="1f29c-144">String</span></span>|<span data-ttu-id="1f29c-145">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="1f29c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f29c-146">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f29c-147">lastModifiedDateTime</span></span>|<span data-ttu-id="1f29c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f29c-148">DateTimeOffset</span></span>|<span data-ttu-id="1f29c-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1f29c-149">DateTime the object was last modified.</span></span> <span data-ttu-id="1f29c-150">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-151">displayName</span><span class="sxs-lookup"><span data-stu-id="1f29c-151">displayName</span></span>|<span data-ttu-id="1f29c-152">String</span><span class="sxs-lookup"><span data-stu-id="1f29c-152">String</span></span>|<span data-ttu-id="1f29c-153">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f29c-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f29c-154">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-155">версия</span><span class="sxs-lookup"><span data-stu-id="1f29c-155">version</span></span>|<span data-ttu-id="1f29c-156">Int32</span><span class="sxs-lookup"><span data-stu-id="1f29c-156">Int32</span></span>|<span data-ttu-id="1f29c-157">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f29c-157">Version of the device configuration.</span></span> <span data-ttu-id="1f29c-158">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="1f29c-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="1f29c-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="1f29c-159">encodedSettingXml</span></span>|<span data-ttu-id="1f29c-160">Двоичный</span><span class="sxs-lookup"><span data-stu-id="1f29c-160">Binary</span></span>|<span data-ttu-id="1f29c-161">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="1f29c-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="1f29c-162">параметры</span><span class="sxs-lookup"><span data-stu-id="1f29c-162">settings</span></span>|<span data-ttu-id="1f29c-163">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="1f29c-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="1f29c-164">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="1f29c-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="1f29c-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f29c-165">Response</span></span>
<span data-ttu-id="1f29c-166">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="1f29c-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f29c-167">Пример</span><span class="sxs-lookup"><span data-stu-id="1f29c-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f29c-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f29c-168">Request</span></span>
<span data-ttu-id="1f29c-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f29c-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f29c-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="1f29c-170">Response</span></span>
<span data-ttu-id="1f29c-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="1f29c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



