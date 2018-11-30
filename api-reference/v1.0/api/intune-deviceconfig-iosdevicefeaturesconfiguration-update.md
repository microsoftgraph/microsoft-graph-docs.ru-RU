---
title: Update iosDeviceFeaturesConfiguration
description: Обновление свойств объекта iosDeviceFeaturesConfiguration.
ms.openlocfilehash: 473e28586e51d858320605957e446d730023c8f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026777"
---
# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="cf1dd-103">Update iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf1dd-103">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="cf1dd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf1dd-105">Обновление свойств объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-105">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf1dd-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="cf1dd-106">Prerequisites</span></span>
<span data-ttu-id="cf1dd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf1dd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cf1dd-109">Permission type</span></span>|<span data-ttu-id="cf1dd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf1dd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf1dd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf1dd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf1dd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf1dd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-114">Not supported.</span></span>|
|<span data-ttu-id="cf1dd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cf1dd-115">Application</span></span>|<span data-ttu-id="cf1dd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf1dd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cf1dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cf1dd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cf1dd-118">Request headers</span></span>
|<span data-ttu-id="cf1dd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cf1dd-119">Header</span></span>|<span data-ttu-id="cf1dd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="cf1dd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf1dd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf1dd-121">Authorization</span></span>|<span data-ttu-id="cf1dd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cf1dd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf1dd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf1dd-123">Accept</span></span>|<span data-ttu-id="cf1dd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf1dd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf1dd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cf1dd-125">Request body</span></span>
<span data-ttu-id="cf1dd-126">В тексте запроса добавьте представление объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-126">In the request body, supply a JSON representation for the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="cf1dd-127">В приведенной ниже таблице указаны свойства, которые необходимо указать при создании объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-127">The following table shows the properties that are required when you create the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="cf1dd-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="cf1dd-128">Property</span></span>|<span data-ttu-id="cf1dd-129">Тип</span><span class="sxs-lookup"><span data-stu-id="cf1dd-129">Type</span></span>|<span data-ttu-id="cf1dd-130">Описание</span><span class="sxs-lookup"><span data-stu-id="cf1dd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf1dd-131">id</span><span class="sxs-lookup"><span data-stu-id="cf1dd-131">id</span></span>|<span data-ttu-id="cf1dd-132">String</span><span class="sxs-lookup"><span data-stu-id="cf1dd-132">String</span></span>|<span data-ttu-id="cf1dd-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-133">Key of the entity.</span></span> <span data-ttu-id="cf1dd-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf1dd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="cf1dd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1dd-136">DateTimeOffset</span></span>|<span data-ttu-id="cf1dd-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-137">DateTime the object was last modified.</span></span> <span data-ttu-id="cf1dd-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf1dd-139">createdDateTime</span></span>|<span data-ttu-id="cf1dd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf1dd-140">DateTimeOffset</span></span>|<span data-ttu-id="cf1dd-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-141">DateTime the object was created.</span></span> <span data-ttu-id="cf1dd-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-143">описание</span><span class="sxs-lookup"><span data-stu-id="cf1dd-143">description</span></span>|<span data-ttu-id="cf1dd-144">String</span><span class="sxs-lookup"><span data-stu-id="cf1dd-144">String</span></span>|<span data-ttu-id="cf1dd-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cf1dd-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="cf1dd-147">displayName</span></span>|<span data-ttu-id="cf1dd-148">String</span><span class="sxs-lookup"><span data-stu-id="cf1dd-148">String</span></span>|<span data-ttu-id="cf1dd-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cf1dd-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-151">version</span><span class="sxs-lookup"><span data-stu-id="cf1dd-151">version</span></span>|<span data-ttu-id="cf1dd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="cf1dd-152">Int32</span></span>|<span data-ttu-id="cf1dd-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-153">Version of the device configuration.</span></span> <span data-ttu-id="cf1dd-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cf1dd-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="cf1dd-155">assetTagTemplate</span></span>|<span data-ttu-id="cf1dd-156">String</span><span class="sxs-lookup"><span data-stu-id="cf1dd-156">String</span></span>|<span data-ttu-id="cf1dd-157">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="cf1dd-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="cf1dd-158">lockScreenFootnote</span></span>|<span data-ttu-id="cf1dd-159">String</span><span class="sxs-lookup"><span data-stu-id="cf1dd-159">String</span></span>|<span data-ttu-id="cf1dd-160">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="cf1dd-161">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="cf1dd-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="cf1dd-162">homeScreenDockIcons</span></span>|<span data-ttu-id="cf1dd-163">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="cf1dd-164">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="cf1dd-165">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cf1dd-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="cf1dd-166">homeScreenPages</span></span>|<span data-ttu-id="cf1dd-167">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="cf1dd-168">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="cf1dd-169">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="cf1dd-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="cf1dd-170">notificationSettings</span></span>|<span data-ttu-id="cf1dd-171">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cf1dd-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="cf1dd-172">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="cf1dd-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="cf1dd-173">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="cf1dd-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf1dd-174">Response</span></span>
<span data-ttu-id="cf1dd-175">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-175">If successful, this method returns a `200 OK` response code and an updated [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf1dd-176">Пример</span><span class="sxs-lookup"><span data-stu-id="cf1dd-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf1dd-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="cf1dd-177">Request</span></span>
<span data-ttu-id="cf1dd-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cf1dd-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf1dd-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="cf1dd-179">Response</span></span>
<span data-ttu-id="cf1dd-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="cf1dd-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



