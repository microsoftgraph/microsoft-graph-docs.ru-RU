---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b690013cff406cc46017fd1ab81523be60fc028
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175152"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="a34d9-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="a34d9-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="a34d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a34d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a34d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a34d9-106">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a34d9-106">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a34d9-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="a34d9-107">Prerequisites</span></span>
<span data-ttu-id="a34d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a34d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a34d9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a34d9-110">Permission type</span></span>|<span data-ttu-id="a34d9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a34d9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a34d9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a34d9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a34d9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a34d9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a34d9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a34d9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a34d9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34d9-115">Not supported.</span></span>|
|<span data-ttu-id="a34d9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a34d9-116">Application</span></span>|<span data-ttu-id="a34d9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a34d9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a34d9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a34d9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a34d9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a34d9-119">Request headers</span></span>
|<span data-ttu-id="a34d9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a34d9-120">Header</span></span>|<span data-ttu-id="a34d9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a34d9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a34d9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a34d9-122">Authorization</span></span>|<span data-ttu-id="a34d9-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a34d9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a34d9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a34d9-124">Accept</span></span>|<span data-ttu-id="a34d9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a34d9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a34d9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a34d9-126">Request body</span></span>
<span data-ttu-id="a34d9-127">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a34d9-127">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="a34d9-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a34d9-128">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="a34d9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a34d9-129">Property</span></span>|<span data-ttu-id="a34d9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a34d9-130">Type</span></span>|<span data-ttu-id="a34d9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a34d9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a34d9-132">id</span><span class="sxs-lookup"><span data-stu-id="a34d9-132">id</span></span>|<span data-ttu-id="a34d9-133">String</span><span class="sxs-lookup"><span data-stu-id="a34d9-133">String</span></span>|<span data-ttu-id="a34d9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a34d9-134">Key of the entity.</span></span> <span data-ttu-id="a34d9-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="a34d9-136">targetedMobileApps</span></span>|<span data-ttu-id="a34d9-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a34d9-137">String collection</span></span>|<span data-ttu-id="a34d9-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="a34d9-138">the associated app.</span></span> <span data-ttu-id="a34d9-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a34d9-140">roleScopeTagIds</span></span>|<span data-ttu-id="a34d9-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a34d9-141">String collection</span></span>|<span data-ttu-id="a34d9-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a34d9-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="a34d9-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a34d9-144">createdDateTime</span></span>|<span data-ttu-id="a34d9-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a34d9-145">DateTimeOffset</span></span>|<span data-ttu-id="a34d9-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a34d9-146">DateTime the object was created.</span></span> <span data-ttu-id="a34d9-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-148">описание</span><span class="sxs-lookup"><span data-stu-id="a34d9-148">description</span></span>|<span data-ttu-id="a34d9-149">String</span><span class="sxs-lookup"><span data-stu-id="a34d9-149">String</span></span>|<span data-ttu-id="a34d9-150">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="a34d9-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a34d9-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a34d9-152">lastModifiedDateTime</span></span>|<span data-ttu-id="a34d9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a34d9-153">DateTimeOffset</span></span>|<span data-ttu-id="a34d9-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a34d9-154">DateTime the object was last modified.</span></span> <span data-ttu-id="a34d9-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-156">displayName</span><span class="sxs-lookup"><span data-stu-id="a34d9-156">displayName</span></span>|<span data-ttu-id="a34d9-157">String</span><span class="sxs-lookup"><span data-stu-id="a34d9-157">String</span></span>|<span data-ttu-id="a34d9-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a34d9-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a34d9-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-160">версия</span><span class="sxs-lookup"><span data-stu-id="a34d9-160">version</span></span>|<span data-ttu-id="a34d9-161">Int32</span><span class="sxs-lookup"><span data-stu-id="a34d9-161">Int32</span></span>|<span data-ttu-id="a34d9-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a34d9-162">Version of the device configuration.</span></span> <span data-ttu-id="a34d9-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="a34d9-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="a34d9-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="a34d9-164">encodedSettingXml</span></span>|<span data-ttu-id="a34d9-165">Двоичный</span><span class="sxs-lookup"><span data-stu-id="a34d9-165">Binary</span></span>|<span data-ttu-id="a34d9-166">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="a34d9-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="a34d9-167">параметры</span><span class="sxs-lookup"><span data-stu-id="a34d9-167">settings</span></span>|<span data-ttu-id="a34d9-168">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="a34d9-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="a34d9-169">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="a34d9-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="a34d9-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="a34d9-170">Response</span></span>
<span data-ttu-id="a34d9-171">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="a34d9-171">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a34d9-172">Пример</span><span class="sxs-lookup"><span data-stu-id="a34d9-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a34d9-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="a34d9-173">Request</span></span>
<span data-ttu-id="a34d9-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a34d9-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a34d9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="a34d9-175">Response</span></span>
<span data-ttu-id="a34d9-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a34d9-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




