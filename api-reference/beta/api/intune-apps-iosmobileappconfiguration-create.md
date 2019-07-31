---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3b1dc13ed78c7a6a17b6dea8b81bb11bddc2082f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35951752"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="0d79d-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0d79d-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="0d79d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d79d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d79d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d79d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d79d-106">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0d79d-106">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d79d-107">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="0d79d-107">Prerequisites</span></span>
<span data-ttu-id="0d79d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0d79d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d79d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0d79d-110">Permission type</span></span>|<span data-ttu-id="0d79d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0d79d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d79d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0d79d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d79d-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d79d-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0d79d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0d79d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d79d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d79d-115">Not supported.</span></span>|
|<span data-ttu-id="0d79d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0d79d-116">Application</span></span>|<span data-ttu-id="0d79d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0d79d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d79d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0d79d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0d79d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0d79d-119">Request headers</span></span>
|<span data-ttu-id="0d79d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0d79d-120">Header</span></span>|<span data-ttu-id="0d79d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="0d79d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d79d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0d79d-122">Authorization</span></span>|<span data-ttu-id="0d79d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0d79d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d79d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="0d79d-124">Accept</span></span>|<span data-ttu-id="0d79d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d79d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d79d-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0d79d-126">Request body</span></span>
<span data-ttu-id="0d79d-127">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d79d-127">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="0d79d-128">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="0d79d-128">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="0d79d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d79d-129">Property</span></span>|<span data-ttu-id="0d79d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="0d79d-130">Type</span></span>|<span data-ttu-id="0d79d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="0d79d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d79d-132">id</span><span class="sxs-lookup"><span data-stu-id="0d79d-132">id</span></span>|<span data-ttu-id="0d79d-133">String</span><span class="sxs-lookup"><span data-stu-id="0d79d-133">String</span></span>|<span data-ttu-id="0d79d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0d79d-134">Key of the entity.</span></span> <span data-ttu-id="0d79d-135">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-135">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-136">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0d79d-136">targetedMobileApps</span></span>|<span data-ttu-id="0d79d-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0d79d-137">String collection</span></span>|<span data-ttu-id="0d79d-138">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="0d79d-138">the associated app.</span></span> <span data-ttu-id="0d79d-139">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-139">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0d79d-140">roleScopeTagIds</span></span>|<span data-ttu-id="0d79d-141">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="0d79d-141">String collection</span></span>|<span data-ttu-id="0d79d-142">Список тегов областей для этой сущности конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="0d79d-142">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="0d79d-143">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-143">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0d79d-144">createdDateTime</span></span>|<span data-ttu-id="0d79d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d79d-145">DateTimeOffset</span></span>|<span data-ttu-id="0d79d-146">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="0d79d-146">DateTime the object was created.</span></span> <span data-ttu-id="0d79d-147">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-147">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-148">description</span><span class="sxs-lookup"><span data-stu-id="0d79d-148">description</span></span>|<span data-ttu-id="0d79d-149">String</span><span class="sxs-lookup"><span data-stu-id="0d79d-149">String</span></span>|<span data-ttu-id="0d79d-150">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d79d-150">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0d79d-151">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-151">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d79d-152">lastModifiedDateTime</span></span>|<span data-ttu-id="0d79d-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d79d-153">DateTimeOffset</span></span>|<span data-ttu-id="0d79d-154">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="0d79d-154">DateTime the object was last modified.</span></span> <span data-ttu-id="0d79d-155">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-155">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-156">displayName</span><span class="sxs-lookup"><span data-stu-id="0d79d-156">displayName</span></span>|<span data-ttu-id="0d79d-157">Строка</span><span class="sxs-lookup"><span data-stu-id="0d79d-157">String</span></span>|<span data-ttu-id="0d79d-158">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d79d-158">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0d79d-159">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-159">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-160">версия</span><span class="sxs-lookup"><span data-stu-id="0d79d-160">version</span></span>|<span data-ttu-id="0d79d-161">Int32</span><span class="sxs-lookup"><span data-stu-id="0d79d-161">Int32</span></span>|<span data-ttu-id="0d79d-162">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="0d79d-162">Version of the device configuration.</span></span> <span data-ttu-id="0d79d-163">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-163">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="0d79d-164">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="0d79d-164">encodedSettingXml</span></span>|<span data-ttu-id="0d79d-165">Двоичный</span><span class="sxs-lookup"><span data-stu-id="0d79d-165">Binary</span></span>|<span data-ttu-id="0d79d-166">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="0d79d-166">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="0d79d-167">параметры</span><span class="sxs-lookup"><span data-stu-id="0d79d-167">settings</span></span>|<span data-ttu-id="0d79d-168">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d79d-168">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="0d79d-169">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="0d79d-169">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="0d79d-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0d79d-170">Response</span></span>
<span data-ttu-id="0d79d-171">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="0d79d-171">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d79d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="0d79d-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d79d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="0d79d-173">Request</span></span>
<span data-ttu-id="0d79d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0d79d-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0d79d-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="0d79d-175">Response</span></span>
<span data-ttu-id="0d79d-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0d79d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





