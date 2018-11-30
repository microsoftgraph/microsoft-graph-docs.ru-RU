---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
ms.openlocfilehash: 24bd4b7a606ce95a146d0ce5273ba268766bb6c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025335"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="83b48-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="83b48-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="83b48-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="83b48-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83b48-105">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="83b48-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83b48-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="83b48-106">Prerequisites</span></span>
<span data-ttu-id="83b48-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83b48-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83b48-109">Permission type</span></span>|<span data-ttu-id="83b48-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83b48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83b48-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83b48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="83b48-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83b48-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83b48-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83b48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83b48-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83b48-114">Not supported.</span></span>|
|<span data-ttu-id="83b48-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="83b48-115">Application</span></span>|<span data-ttu-id="83b48-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83b48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83b48-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83b48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="83b48-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83b48-118">Request headers</span></span>
|<span data-ttu-id="83b48-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="83b48-119">Header</span></span>|<span data-ttu-id="83b48-120">Значение</span><span class="sxs-lookup"><span data-stu-id="83b48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83b48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="83b48-121">Authorization</span></span>|<span data-ttu-id="83b48-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="83b48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83b48-123">Accept</span><span class="sxs-lookup"><span data-stu-id="83b48-123">Accept</span></span>|<span data-ttu-id="83b48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="83b48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83b48-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83b48-125">Request body</span></span>
<span data-ttu-id="83b48-126">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83b48-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="83b48-127">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="83b48-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="83b48-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="83b48-128">Property</span></span>|<span data-ttu-id="83b48-129">Тип</span><span class="sxs-lookup"><span data-stu-id="83b48-129">Type</span></span>|<span data-ttu-id="83b48-130">Описание</span><span class="sxs-lookup"><span data-stu-id="83b48-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b48-131">id</span><span class="sxs-lookup"><span data-stu-id="83b48-131">id</span></span>|<span data-ttu-id="83b48-132">String</span><span class="sxs-lookup"><span data-stu-id="83b48-132">String</span></span>|<span data-ttu-id="83b48-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="83b48-133">Key of the entity.</span></span> <span data-ttu-id="83b48-134">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="83b48-135">targetedMobileApps</span></span>|<span data-ttu-id="83b48-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="83b48-136">String collection</span></span>|<span data-ttu-id="83b48-137">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="83b48-137">the associated app.</span></span> <span data-ttu-id="83b48-138">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83b48-139">createdDateTime</span></span>|<span data-ttu-id="83b48-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b48-140">DateTimeOffset</span></span>|<span data-ttu-id="83b48-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="83b48-141">DateTime the object was created.</span></span> <span data-ttu-id="83b48-142">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-143">описание</span><span class="sxs-lookup"><span data-stu-id="83b48-143">description</span></span>|<span data-ttu-id="83b48-144">String</span><span class="sxs-lookup"><span data-stu-id="83b48-144">String</span></span>|<span data-ttu-id="83b48-145">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="83b48-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="83b48-146">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83b48-147">lastModifiedDateTime</span></span>|<span data-ttu-id="83b48-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83b48-148">DateTimeOffset</span></span>|<span data-ttu-id="83b48-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="83b48-149">DateTime the object was last modified.</span></span> <span data-ttu-id="83b48-150">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-151">displayName</span><span class="sxs-lookup"><span data-stu-id="83b48-151">displayName</span></span>|<span data-ttu-id="83b48-152">String</span><span class="sxs-lookup"><span data-stu-id="83b48-152">String</span></span>|<span data-ttu-id="83b48-153">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83b48-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="83b48-154">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-155">версия</span><span class="sxs-lookup"><span data-stu-id="83b48-155">version</span></span>|<span data-ttu-id="83b48-156">Int32</span><span class="sxs-lookup"><span data-stu-id="83b48-156">Int32</span></span>|<span data-ttu-id="83b48-157">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="83b48-157">Version of the device configuration.</span></span> <span data-ttu-id="83b48-158">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="83b48-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="83b48-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="83b48-159">encodedSettingXml</span></span>|<span data-ttu-id="83b48-160">Двоичный</span><span class="sxs-lookup"><span data-stu-id="83b48-160">Binary</span></span>|<span data-ttu-id="83b48-161">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="83b48-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="83b48-162">параметры</span><span class="sxs-lookup"><span data-stu-id="83b48-162">settings</span></span>|<span data-ttu-id="83b48-163">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="83b48-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="83b48-164">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="83b48-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="83b48-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="83b48-165">Response</span></span>
<span data-ttu-id="83b48-166">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="83b48-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83b48-167">Пример</span><span class="sxs-lookup"><span data-stu-id="83b48-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="83b48-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="83b48-168">Request</span></span>
<span data-ttu-id="83b48-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="83b48-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="83b48-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="83b48-170">Response</span></span>
<span data-ttu-id="83b48-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="83b48-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



