---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 80f08b4e586c6e8a1df6198e4ccd5f46f2e58ae7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516562"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="b4f1c-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b4f1c-103">Update iosMobileAppConfiguration</span></span>

<span data-ttu-id="b4f1c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4f1c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4f1c-106">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4f1c-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4f1c-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="b4f1c-107">Prerequisites</span></span>
<span data-ttu-id="b4f1c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4f1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4f1c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4f1c-110">Permission type</span></span>|<span data-ttu-id="b4f1c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4f1c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b4f1c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4f1c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b4f1c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4f1c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-115">Not supported.</span></span>|
|<span data-ttu-id="b4f1c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4f1c-116">Application</span></span>|<span data-ttu-id="b4f1c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4f1c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4f1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b4f1c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b4f1c-119">Request headers</span></span>
|<span data-ttu-id="b4f1c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b4f1c-120">Header</span></span>|<span data-ttu-id="b4f1c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b4f1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4f1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4f1c-122">Authorization</span></span>|<span data-ttu-id="b4f1c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4f1c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b4f1c-124">Accept</span></span>|<span data-ttu-id="b4f1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b4f1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4f1c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4f1c-126">Request body</span></span>
<span data-ttu-id="b4f1c-127">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="b4f1c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b4f1c-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="b4f1c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4f1c-129">Property</span></span>|<span data-ttu-id="b4f1c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b4f1c-130">Type</span></span>|<span data-ttu-id="b4f1c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b4f1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4f1c-132">id</span><span class="sxs-lookup"><span data-stu-id="b4f1c-132">id</span></span>|<span data-ttu-id="b4f1c-133">String</span><span class="sxs-lookup"><span data-stu-id="b4f1c-133">String</span></span>|<span data-ttu-id="b4f1c-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-134">Key of the entity.</span></span> <span data-ttu-id="b4f1c-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b4f1c-136">targetedMobileApps</span></span>|<span data-ttu-id="b4f1c-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="b4f1c-137">String collection</span></span>|<span data-ttu-id="b4f1c-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="b4f1c-138">the associated app.</span></span> <span data-ttu-id="b4f1c-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b4f1c-140">createdDateTime</span></span>|<span data-ttu-id="b4f1c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4f1c-141">DateTimeOffset</span></span>|<span data-ttu-id="b4f1c-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-142">DateTime the object was created.</span></span> <span data-ttu-id="b4f1c-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-144">description</span><span class="sxs-lookup"><span data-stu-id="b4f1c-144">description</span></span>|<span data-ttu-id="b4f1c-145">String</span><span class="sxs-lookup"><span data-stu-id="b4f1c-145">String</span></span>|<span data-ttu-id="b4f1c-146">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b4f1c-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b4f1c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="b4f1c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4f1c-149">DateTimeOffset</span></span>|<span data-ttu-id="b4f1c-150">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-150">DateTime the object was last modified.</span></span> <span data-ttu-id="b4f1c-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-152">displayName</span><span class="sxs-lookup"><span data-stu-id="b4f1c-152">displayName</span></span>|<span data-ttu-id="b4f1c-153">Строка</span><span class="sxs-lookup"><span data-stu-id="b4f1c-153">String</span></span>|<span data-ttu-id="b4f1c-154">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-154">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b4f1c-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-156">версия</span><span class="sxs-lookup"><span data-stu-id="b4f1c-156">version</span></span>|<span data-ttu-id="b4f1c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="b4f1c-157">Int32</span></span>|<span data-ttu-id="b4f1c-158">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-158">Version of the device configuration.</span></span> <span data-ttu-id="b4f1c-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="b4f1c-160">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="b4f1c-160">encodedSettingXml</span></span>|<span data-ttu-id="b4f1c-161">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b4f1c-161">Binary</span></span>|<span data-ttu-id="b4f1c-162">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-162">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="b4f1c-163">параметры</span><span class="sxs-lookup"><span data-stu-id="b4f1c-163">settings</span></span>|<span data-ttu-id="b4f1c-164">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1c-164">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="b4f1c-165">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-165">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="b4f1c-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4f1c-166">Response</span></span>
<span data-ttu-id="b4f1c-167">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-167">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4f1c-168">Пример</span><span class="sxs-lookup"><span data-stu-id="b4f1c-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4f1c-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4f1c-169">Request</span></span>
<span data-ttu-id="b4f1c-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b4f1c-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4f1c-171">Response</span></span>
<span data-ttu-id="b4f1c-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b4f1c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




