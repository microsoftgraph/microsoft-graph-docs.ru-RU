---
title: Создание объекта iosDeviceFeaturesConfiguration
description: Создание объекта iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e191d89416402c8037cf7970e858681a1db14887
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514573"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="53428-103">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="53428-103">Create iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="53428-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53428-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53428-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53428-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53428-106">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-106">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53428-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53428-107">Prerequisites</span></span>
<span data-ttu-id="53428-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53428-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53428-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53428-110">Permission type</span></span>|<span data-ttu-id="53428-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53428-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53428-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53428-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53428-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53428-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53428-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53428-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53428-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53428-115">Not supported.</span></span>|
|<span data-ttu-id="53428-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53428-116">Application</span></span>|<span data-ttu-id="53428-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53428-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53428-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53428-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="53428-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="53428-119">Request headers</span></span>
|<span data-ttu-id="53428-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53428-120">Header</span></span>|<span data-ttu-id="53428-121">Значение</span><span class="sxs-lookup"><span data-stu-id="53428-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53428-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53428-122">Authorization</span></span>|<span data-ttu-id="53428-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53428-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53428-124">Accept</span><span class="sxs-lookup"><span data-stu-id="53428-124">Accept</span></span>|<span data-ttu-id="53428-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53428-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53428-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53428-126">Request body</span></span>
<span data-ttu-id="53428-127">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53428-127">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="53428-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="53428-128">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="53428-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="53428-129">Property</span></span>|<span data-ttu-id="53428-130">Тип</span><span class="sxs-lookup"><span data-stu-id="53428-130">Type</span></span>|<span data-ttu-id="53428-131">Описание</span><span class="sxs-lookup"><span data-stu-id="53428-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53428-132">id</span><span class="sxs-lookup"><span data-stu-id="53428-132">id</span></span>|<span data-ttu-id="53428-133">Строка</span><span class="sxs-lookup"><span data-stu-id="53428-133">String</span></span>|<span data-ttu-id="53428-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53428-134">Key of the entity.</span></span> <span data-ttu-id="53428-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53428-136">lastModifiedDateTime</span></span>|<span data-ttu-id="53428-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53428-137">DateTimeOffset</span></span>|<span data-ttu-id="53428-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="53428-138">DateTime the object was last modified.</span></span> <span data-ttu-id="53428-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53428-140">createdDateTime</span></span>|<span data-ttu-id="53428-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53428-141">DateTimeOffset</span></span>|<span data-ttu-id="53428-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="53428-142">DateTime the object was created.</span></span> <span data-ttu-id="53428-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-144">description</span><span class="sxs-lookup"><span data-stu-id="53428-144">description</span></span>|<span data-ttu-id="53428-145">String</span><span class="sxs-lookup"><span data-stu-id="53428-145">String</span></span>|<span data-ttu-id="53428-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53428-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="53428-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-148">displayName</span><span class="sxs-lookup"><span data-stu-id="53428-148">displayName</span></span>|<span data-ttu-id="53428-149">Строка</span><span class="sxs-lookup"><span data-stu-id="53428-149">String</span></span>|<span data-ttu-id="53428-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53428-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="53428-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53428-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-152">version</span><span class="sxs-lookup"><span data-stu-id="53428-152">version</span></span>|<span data-ttu-id="53428-153">Int32</span><span class="sxs-lookup"><span data-stu-id="53428-153">Int32</span></span>|<span data-ttu-id="53428-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="53428-154">Version of the device configuration.</span></span> <span data-ttu-id="53428-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53428-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="53428-156">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="53428-156">assetTagTemplate</span></span>|<span data-ttu-id="53428-157">Строка</span><span class="sxs-lookup"><span data-stu-id="53428-157">String</span></span>|<span data-ttu-id="53428-158">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="53428-158">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="53428-159">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="53428-159">lockScreenFootnote</span></span>|<span data-ttu-id="53428-160">String</span><span class="sxs-lookup"><span data-stu-id="53428-160">String</span></span>|<span data-ttu-id="53428-161">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="53428-161">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="53428-162">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="53428-162">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="53428-163">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="53428-163">homeScreenDockIcons</span></span>|<span data-ttu-id="53428-164">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="53428-164">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="53428-165">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="53428-165">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="53428-166">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="53428-166">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="53428-167">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="53428-167">homeScreenPages</span></span>|<span data-ttu-id="53428-168">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="53428-168">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="53428-169">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="53428-169">A list of pages on the Home Screen.</span></span> <span data-ttu-id="53428-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="53428-170">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="53428-171">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="53428-171">notificationSettings</span></span>|<span data-ttu-id="53428-172">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="53428-172">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="53428-173">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="53428-173">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="53428-174">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="53428-174">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="53428-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="53428-175">Response</span></span>
<span data-ttu-id="53428-176">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53428-176">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53428-177">Пример</span><span class="sxs-lookup"><span data-stu-id="53428-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="53428-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="53428-178">Request</span></span>
<span data-ttu-id="53428-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53428-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="53428-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="53428-180">Response</span></span>
<span data-ttu-id="53428-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53428-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```




