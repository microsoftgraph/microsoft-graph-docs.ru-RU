---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 875cb3eae1388139dbf1d3a46d462369dd3e1e9b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330638"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="9f9d5-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9f9d5-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="9f9d5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f9d5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f9d5-106">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f9d5-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f9d5-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="9f9d5-107">Prerequisites</span></span>
<span data-ttu-id="9f9d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f9d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f9d5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f9d5-110">Permission type</span></span>|<span data-ttu-id="9f9d5-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f9d5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9f9d5-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f9d5-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9f9d5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f9d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-115">Not supported.</span></span>|
|<span data-ttu-id="9f9d5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9f9d5-116">Application</span></span>|<span data-ttu-id="9f9d5-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f9d5-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f9d5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f9d5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f9d5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f9d5-119">Request headers</span></span>
|<span data-ttu-id="9f9d5-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f9d5-120">Header</span></span>|<span data-ttu-id="9f9d5-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9f9d5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f9d5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f9d5-122">Authorization</span></span>|<span data-ttu-id="9f9d5-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f9d5-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9f9d5-124">Accept</span></span>|<span data-ttu-id="9f9d5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9f9d5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f9d5-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9f9d5-126">Request body</span></span>
<span data-ttu-id="9f9d5-127">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="9f9d5-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9f9d5-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="9f9d5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f9d5-129">Property</span></span>|<span data-ttu-id="9f9d5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9f9d5-130">Type</span></span>|<span data-ttu-id="9f9d5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9f9d5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f9d5-132">id</span><span class="sxs-lookup"><span data-stu-id="9f9d5-132">id</span></span>|<span data-ttu-id="9f9d5-133">String</span><span class="sxs-lookup"><span data-stu-id="9f9d5-133">String</span></span>|<span data-ttu-id="9f9d5-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-134">Key of the entity.</span></span> <span data-ttu-id="9f9d5-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="9f9d5-136">targetedMobileApps</span></span>|<span data-ttu-id="9f9d5-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9f9d5-137">String collection</span></span>|<span data-ttu-id="9f9d5-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="9f9d5-138">the associated app.</span></span> <span data-ttu-id="9f9d5-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9f9d5-140">roleScopeTagIds</span></span>|<span data-ttu-id="9f9d5-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f9d5-141">String collection</span></span>|<span data-ttu-id="9f9d5-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="9f9d5-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d5-144">createdDateTime</span></span>|<span data-ttu-id="9f9d5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d5-145">DateTimeOffset</span></span>|<span data-ttu-id="9f9d5-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-146">DateTime the object was created.</span></span> <span data-ttu-id="9f9d5-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-148">description</span><span class="sxs-lookup"><span data-stu-id="9f9d5-148">description</span></span>|<span data-ttu-id="9f9d5-149">String</span><span class="sxs-lookup"><span data-stu-id="9f9d5-149">String</span></span>|<span data-ttu-id="9f9d5-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9f9d5-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f9d5-152">lastModifiedDateTime</span></span>|<span data-ttu-id="9f9d5-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f9d5-153">DateTimeOffset</span></span>|<span data-ttu-id="9f9d5-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-154">DateTime the object was last modified.</span></span> <span data-ttu-id="9f9d5-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-156">displayName</span><span class="sxs-lookup"><span data-stu-id="9f9d5-156">displayName</span></span>|<span data-ttu-id="9f9d5-157">Строка</span><span class="sxs-lookup"><span data-stu-id="9f9d5-157">String</span></span>|<span data-ttu-id="9f9d5-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9f9d5-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-160">версия</span><span class="sxs-lookup"><span data-stu-id="9f9d5-160">version</span></span>|<span data-ttu-id="9f9d5-161">Int32</span><span class="sxs-lookup"><span data-stu-id="9f9d5-161">Int32</span></span>|<span data-ttu-id="9f9d5-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-162">Version of the device configuration.</span></span> <span data-ttu-id="9f9d5-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9f9d5-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="9f9d5-164">encodedSettingXml</span></span>|<span data-ttu-id="9f9d5-165">Двоичный</span><span class="sxs-lookup"><span data-stu-id="9f9d5-165">Binary</span></span>|<span data-ttu-id="9f9d5-166">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="9f9d5-167">параметры</span><span class="sxs-lookup"><span data-stu-id="9f9d5-167">settings</span></span>|<span data-ttu-id="9f9d5-168">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="9f9d5-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="9f9d5-169">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="9f9d5-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="9f9d5-170">Response</span></span>
<span data-ttu-id="9f9d5-171">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-171">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f9d5-172">Пример</span><span class="sxs-lookup"><span data-stu-id="9f9d5-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f9d5-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f9d5-173">Request</span></span>
<span data-ttu-id="9f9d5-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 596

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
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

### <a name="response"></a><span data-ttu-id="9f9d5-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f9d5-175">Response</span></span>
<span data-ttu-id="9f9d5-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9f9d5-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
  "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
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






