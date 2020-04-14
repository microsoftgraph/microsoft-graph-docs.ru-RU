---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4f78bef1c58e09fcbc88f8964e88a59966e7b18a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394980"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="fb88f-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="fb88f-103">Create iosMobileAppConfiguration</span></span>

<span data-ttu-id="fb88f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb88f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb88f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb88f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb88f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fb88f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb88f-107">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="fb88f-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fb88f-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="fb88f-108">Prerequisites</span></span>
<span data-ttu-id="fb88f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fb88f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb88f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fb88f-111">Permission type</span></span>|<span data-ttu-id="fb88f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fb88f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb88f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fb88f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fb88f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb88f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fb88f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fb88f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb88f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb88f-116">Not supported.</span></span>|
|<span data-ttu-id="fb88f-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fb88f-117">Application</span></span>|<span data-ttu-id="fb88f-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb88f-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb88f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fb88f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fb88f-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="fb88f-120">Request headers</span></span>
|<span data-ttu-id="fb88f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fb88f-121">Header</span></span>|<span data-ttu-id="fb88f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fb88f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fb88f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb88f-123">Authorization</span></span>|<span data-ttu-id="fb88f-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fb88f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fb88f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fb88f-125">Accept</span></span>|<span data-ttu-id="fb88f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fb88f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb88f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fb88f-127">Request body</span></span>
<span data-ttu-id="fb88f-128">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb88f-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="fb88f-129">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="fb88f-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="fb88f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb88f-130">Property</span></span>|<span data-ttu-id="fb88f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="fb88f-131">Type</span></span>|<span data-ttu-id="fb88f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="fb88f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb88f-133">id</span><span class="sxs-lookup"><span data-stu-id="fb88f-133">id</span></span>|<span data-ttu-id="fb88f-134">String</span><span class="sxs-lookup"><span data-stu-id="fb88f-134">String</span></span>|<span data-ttu-id="fb88f-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="fb88f-135">Key of the entity.</span></span> <span data-ttu-id="fb88f-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="fb88f-137">targetedMobileApps</span></span>|<span data-ttu-id="fb88f-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb88f-138">String collection</span></span>|<span data-ttu-id="fb88f-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="fb88f-139">the associated app.</span></span> <span data-ttu-id="fb88f-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fb88f-141">roleScopeTagIds</span></span>|<span data-ttu-id="fb88f-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb88f-142">String collection</span></span>|<span data-ttu-id="fb88f-143">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fb88f-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="fb88f-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb88f-145">createdDateTime</span></span>|<span data-ttu-id="fb88f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb88f-146">DateTimeOffset</span></span>|<span data-ttu-id="fb88f-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="fb88f-147">DateTime the object was created.</span></span> <span data-ttu-id="fb88f-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-149">description</span><span class="sxs-lookup"><span data-stu-id="fb88f-149">description</span></span>|<span data-ttu-id="fb88f-150">String</span><span class="sxs-lookup"><span data-stu-id="fb88f-150">String</span></span>|<span data-ttu-id="fb88f-151">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb88f-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fb88f-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb88f-153">lastModifiedDateTime</span></span>|<span data-ttu-id="fb88f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb88f-154">DateTimeOffset</span></span>|<span data-ttu-id="fb88f-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="fb88f-155">DateTime the object was last modified.</span></span> <span data-ttu-id="fb88f-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-157">displayName</span><span class="sxs-lookup"><span data-stu-id="fb88f-157">displayName</span></span>|<span data-ttu-id="fb88f-158">Строка</span><span class="sxs-lookup"><span data-stu-id="fb88f-158">String</span></span>|<span data-ttu-id="fb88f-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb88f-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fb88f-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-161">версия</span><span class="sxs-lookup"><span data-stu-id="fb88f-161">version</span></span>|<span data-ttu-id="fb88f-162">Int32</span><span class="sxs-lookup"><span data-stu-id="fb88f-162">Int32</span></span>|<span data-ttu-id="fb88f-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="fb88f-163">Version of the device configuration.</span></span> <span data-ttu-id="fb88f-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="fb88f-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="fb88f-165">encodedSettingXml</span></span>|<span data-ttu-id="fb88f-166">Двоичный</span><span class="sxs-lookup"><span data-stu-id="fb88f-166">Binary</span></span>|<span data-ttu-id="fb88f-167">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="fb88f-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="fb88f-168">параметры</span><span class="sxs-lookup"><span data-stu-id="fb88f-168">settings</span></span>|<span data-ttu-id="fb88f-169">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="fb88f-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="fb88f-170">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="fb88f-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="fb88f-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="fb88f-171">Response</span></span>
<span data-ttu-id="fb88f-172">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="fb88f-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fb88f-173">Пример</span><span class="sxs-lookup"><span data-stu-id="fb88f-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="fb88f-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="fb88f-174">Request</span></span>
<span data-ttu-id="fb88f-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fb88f-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="fb88f-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="fb88f-176">Response</span></span>
<span data-ttu-id="fb88f-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fb88f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



