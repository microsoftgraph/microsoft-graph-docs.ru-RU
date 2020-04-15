---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a80ce6fd97b3e6d5459b9060a9d47b5db1d76124
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443605"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="b790f-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b790f-103">Create iosMobileAppConfiguration</span></span>

<span data-ttu-id="b790f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b790f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b790f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b790f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b790f-106">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b790f-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b790f-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="b790f-107">Prerequisites</span></span>
<span data-ttu-id="b790f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b790f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b790f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b790f-110">Permission type</span></span>|<span data-ttu-id="b790f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b790f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b790f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b790f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b790f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b790f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b790f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b790f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b790f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b790f-115">Not supported.</span></span>|
|<span data-ttu-id="b790f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b790f-116">Application</span></span>|<span data-ttu-id="b790f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b790f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b790f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b790f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b790f-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b790f-119">Request headers</span></span>
|<span data-ttu-id="b790f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b790f-120">Header</span></span>|<span data-ttu-id="b790f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b790f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b790f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b790f-122">Authorization</span></span>|<span data-ttu-id="b790f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b790f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b790f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b790f-124">Accept</span></span>|<span data-ttu-id="b790f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b790f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b790f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b790f-126">Request body</span></span>
<span data-ttu-id="b790f-127">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b790f-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="b790f-128">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="b790f-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="b790f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b790f-129">Property</span></span>|<span data-ttu-id="b790f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b790f-130">Type</span></span>|<span data-ttu-id="b790f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b790f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b790f-132">id</span><span class="sxs-lookup"><span data-stu-id="b790f-132">id</span></span>|<span data-ttu-id="b790f-133">String</span><span class="sxs-lookup"><span data-stu-id="b790f-133">String</span></span>|<span data-ttu-id="b790f-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b790f-134">Key of the entity.</span></span> <span data-ttu-id="b790f-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b790f-136">targetedMobileApps</span></span>|<span data-ttu-id="b790f-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b790f-137">String collection</span></span>|<span data-ttu-id="b790f-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="b790f-138">the associated app.</span></span> <span data-ttu-id="b790f-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b790f-140">createdDateTime</span></span>|<span data-ttu-id="b790f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b790f-141">DateTimeOffset</span></span>|<span data-ttu-id="b790f-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b790f-142">DateTime the object was created.</span></span> <span data-ttu-id="b790f-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-144">description</span><span class="sxs-lookup"><span data-stu-id="b790f-144">description</span></span>|<span data-ttu-id="b790f-145">String</span><span class="sxs-lookup"><span data-stu-id="b790f-145">String</span></span>|<span data-ttu-id="b790f-146">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b790f-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b790f-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b790f-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b790f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b790f-149">DateTimeOffset</span></span>|<span data-ttu-id="b790f-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b790f-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b790f-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b790f-152">displayName</span></span>|<span data-ttu-id="b790f-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b790f-153">String</span></span>|<span data-ttu-id="b790f-154">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b790f-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b790f-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-156">версия</span><span class="sxs-lookup"><span data-stu-id="b790f-156">version</span></span>|<span data-ttu-id="b790f-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b790f-157">Int32</span></span>|<span data-ttu-id="b790f-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b790f-158">Version of the device configuration.</span></span> <span data-ttu-id="b790f-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b790f-160">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="b790f-160">encodedSettingXml</span></span>|<span data-ttu-id="b790f-161">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b790f-161">Binary</span></span>|<span data-ttu-id="b790f-162">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="b790f-162">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="b790f-163">параметры</span><span class="sxs-lookup"><span data-stu-id="b790f-163">settings</span></span>|<span data-ttu-id="b790f-164">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="b790f-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="b790f-165">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b790f-165">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="b790f-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="b790f-166">Response</span></span>
<span data-ttu-id="b790f-167">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="b790f-167">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b790f-168">Пример</span><span class="sxs-lookup"><span data-stu-id="b790f-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b790f-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b790f-169">Request</span></span>
<span data-ttu-id="b790f-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b790f-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b790f-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b790f-171">Response</span></span>
<span data-ttu-id="b790f-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b790f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






