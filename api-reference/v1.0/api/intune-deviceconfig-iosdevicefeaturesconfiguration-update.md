---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4bd08c4c4dbfa0e74f4c634f067dc428a41b7fb6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514545"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="066cf-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="066cf-103">Update iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="066cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="066cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="066cf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="066cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="066cf-106">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-106">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="066cf-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="066cf-107">Prerequisites</span></span>
<span data-ttu-id="066cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="066cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="066cf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="066cf-110">Permission type</span></span>|<span data-ttu-id="066cf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="066cf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="066cf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="066cf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="066cf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="066cf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="066cf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="066cf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="066cf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066cf-115">Not supported.</span></span>|
|<span data-ttu-id="066cf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="066cf-116">Application</span></span>|<span data-ttu-id="066cf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="066cf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="066cf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="066cf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="066cf-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="066cf-119">Request headers</span></span>
|<span data-ttu-id="066cf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="066cf-120">Header</span></span>|<span data-ttu-id="066cf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="066cf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="066cf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="066cf-122">Authorization</span></span>|<span data-ttu-id="066cf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="066cf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="066cf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="066cf-124">Accept</span></span>|<span data-ttu-id="066cf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="066cf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="066cf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="066cf-126">Request body</span></span>
<span data-ttu-id="066cf-127">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="066cf-127">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="066cf-128">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-128">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="066cf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="066cf-129">Property</span></span>|<span data-ttu-id="066cf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="066cf-130">Type</span></span>|<span data-ttu-id="066cf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="066cf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="066cf-132">id</span><span class="sxs-lookup"><span data-stu-id="066cf-132">id</span></span>|<span data-ttu-id="066cf-133">Строка</span><span class="sxs-lookup"><span data-stu-id="066cf-133">String</span></span>|<span data-ttu-id="066cf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="066cf-134">Key of the entity.</span></span> <span data-ttu-id="066cf-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="066cf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="066cf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="066cf-137">DateTimeOffset</span></span>|<span data-ttu-id="066cf-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="066cf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="066cf-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="066cf-140">createdDateTime</span></span>|<span data-ttu-id="066cf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="066cf-141">DateTimeOffset</span></span>|<span data-ttu-id="066cf-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="066cf-142">DateTime the object was created.</span></span> <span data-ttu-id="066cf-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-144">description</span><span class="sxs-lookup"><span data-stu-id="066cf-144">description</span></span>|<span data-ttu-id="066cf-145">String</span><span class="sxs-lookup"><span data-stu-id="066cf-145">String</span></span>|<span data-ttu-id="066cf-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="066cf-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="066cf-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-148">displayName</span><span class="sxs-lookup"><span data-stu-id="066cf-148">displayName</span></span>|<span data-ttu-id="066cf-149">Строка</span><span class="sxs-lookup"><span data-stu-id="066cf-149">String</span></span>|<span data-ttu-id="066cf-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="066cf-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="066cf-151">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="066cf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-152">version</span><span class="sxs-lookup"><span data-stu-id="066cf-152">version</span></span>|<span data-ttu-id="066cf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="066cf-153">Int32</span></span>|<span data-ttu-id="066cf-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="066cf-154">Version of the device configuration.</span></span> <span data-ttu-id="066cf-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="066cf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="066cf-156">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="066cf-156">assetTagTemplate</span></span>|<span data-ttu-id="066cf-157">Строка</span><span class="sxs-lookup"><span data-stu-id="066cf-157">String</span></span>|<span data-ttu-id="066cf-158">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="066cf-158">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="066cf-159">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="066cf-159">lockScreenFootnote</span></span>|<span data-ttu-id="066cf-160">String</span><span class="sxs-lookup"><span data-stu-id="066cf-160">String</span></span>|<span data-ttu-id="066cf-161">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="066cf-161">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="066cf-162">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="066cf-162">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="066cf-163">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="066cf-163">homeScreenDockIcons</span></span>|<span data-ttu-id="066cf-164">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="066cf-164">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="066cf-165">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="066cf-165">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="066cf-166">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="066cf-166">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="066cf-167">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="066cf-167">homeScreenPages</span></span>|<span data-ttu-id="066cf-168">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="066cf-168">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="066cf-169">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="066cf-169">A list of pages on the Home Screen.</span></span> <span data-ttu-id="066cf-170">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="066cf-170">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="066cf-171">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="066cf-171">notificationSettings</span></span>|<span data-ttu-id="066cf-172">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="066cf-172">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="066cf-173">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="066cf-173">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="066cf-174">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="066cf-174">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="066cf-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="066cf-175">Response</span></span>
<span data-ttu-id="066cf-176">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="066cf-176">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="066cf-177">Пример</span><span class="sxs-lookup"><span data-stu-id="066cf-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="066cf-178">Запрос</span><span class="sxs-lookup"><span data-stu-id="066cf-178">Request</span></span>
<span data-ttu-id="066cf-179">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="066cf-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="066cf-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="066cf-180">Response</span></span>
<span data-ttu-id="066cf-p112">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="066cf-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




