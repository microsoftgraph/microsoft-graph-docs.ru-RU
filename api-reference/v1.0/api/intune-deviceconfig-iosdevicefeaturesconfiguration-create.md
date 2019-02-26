---
title: Создание объекта iosDeviceFeaturesConfiguration
description: Создание объекта iosDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 159247c7bde00b98fd9f25275bcab1be74f034fb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264262"
---
# <a name="create-iosdevicefeaturesconfiguration"></a><span data-ttu-id="6cd33-103">Создание объекта iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cd33-103">Create iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="6cd33-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cd33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cd33-105">Создание объекта [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-105">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cd33-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6cd33-106">Prerequisites</span></span>
<span data-ttu-id="6cd33-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6cd33-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cd33-109">Permission type</span></span>|<span data-ttu-id="6cd33-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cd33-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cd33-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cd33-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6cd33-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cd33-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6cd33-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cd33-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cd33-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd33-114">Not supported.</span></span>|
|<span data-ttu-id="6cd33-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cd33-115">Application</span></span>|<span data-ttu-id="6cd33-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cd33-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cd33-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cd33-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6cd33-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6cd33-118">Request headers</span></span>
|<span data-ttu-id="6cd33-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cd33-119">Header</span></span>|<span data-ttu-id="6cd33-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6cd33-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cd33-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cd33-121">Authorization</span></span>|<span data-ttu-id="6cd33-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6cd33-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cd33-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6cd33-123">Accept</span></span>|<span data-ttu-id="6cd33-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6cd33-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cd33-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6cd33-125">Request body</span></span>
<span data-ttu-id="6cd33-126">В теле запроса добавьте представление объекта iosDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cd33-126">In the request body, supply a JSON representation for the iosDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="6cd33-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6cd33-127">The following table shows the properties that are required when you create the iosDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="6cd33-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cd33-128">Property</span></span>|<span data-ttu-id="6cd33-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6cd33-129">Type</span></span>|<span data-ttu-id="6cd33-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6cd33-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cd33-131">id</span><span class="sxs-lookup"><span data-stu-id="6cd33-131">id</span></span>|<span data-ttu-id="6cd33-132">String</span><span class="sxs-lookup"><span data-stu-id="6cd33-132">String</span></span>|<span data-ttu-id="6cd33-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6cd33-133">Key of the entity.</span></span> <span data-ttu-id="6cd33-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cd33-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6cd33-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cd33-136">DateTimeOffset</span></span>|<span data-ttu-id="6cd33-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6cd33-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6cd33-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cd33-139">createdDateTime</span></span>|<span data-ttu-id="6cd33-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cd33-140">DateTimeOffset</span></span>|<span data-ttu-id="6cd33-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6cd33-141">DateTime the object was created.</span></span> <span data-ttu-id="6cd33-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-143">description</span><span class="sxs-lookup"><span data-stu-id="6cd33-143">description</span></span>|<span data-ttu-id="6cd33-144">Строка</span><span class="sxs-lookup"><span data-stu-id="6cd33-144">String</span></span>|<span data-ttu-id="6cd33-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cd33-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6cd33-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6cd33-147">displayName</span></span>|<span data-ttu-id="6cd33-148">Строка</span><span class="sxs-lookup"><span data-stu-id="6cd33-148">String</span></span>|<span data-ttu-id="6cd33-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cd33-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6cd33-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6cd33-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-151">version</span><span class="sxs-lookup"><span data-stu-id="6cd33-151">version</span></span>|<span data-ttu-id="6cd33-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6cd33-152">Int32</span></span>|<span data-ttu-id="6cd33-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6cd33-153">Version of the device configuration.</span></span> <span data-ttu-id="6cd33-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6cd33-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6cd33-155">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="6cd33-155">assetTagTemplate</span></span>|<span data-ttu-id="6cd33-156">String</span><span class="sxs-lookup"><span data-stu-id="6cd33-156">String</span></span>|<span data-ttu-id="6cd33-157">Сведения о теге ресурса для устройства, отображаемые в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="6cd33-157">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="6cd33-158">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="6cd33-158">lockScreenFootnote</span></span>|<span data-ttu-id="6cd33-159">String</span><span class="sxs-lookup"><span data-stu-id="6cd33-159">String</span></span>|<span data-ttu-id="6cd33-160">Сноска, отображаемая в окне входа и на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="6cd33-160">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="6cd33-161">Доступна в iOS 9.3.1 и более поздних версий.</span><span class="sxs-lookup"><span data-stu-id="6cd33-161">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="6cd33-162">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="6cd33-162">homeScreenDockIcons</span></span>|<span data-ttu-id="6cd33-163">Коллекция [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="6cd33-163">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="6cd33-164">Список приложений и папок, которые должны отображаться на панели Dock на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="6cd33-164">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="6cd33-165">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6cd33-165">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6cd33-166">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="6cd33-166">homeScreenPages</span></span>|<span data-ttu-id="6cd33-167">Коллекция [iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md)</span><span class="sxs-lookup"><span data-stu-id="6cd33-167">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="6cd33-168">Список страниц на начальном экране.</span><span class="sxs-lookup"><span data-stu-id="6cd33-168">A list of pages on the Home Screen.</span></span> <span data-ttu-id="6cd33-169">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6cd33-169">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6cd33-170">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="6cd33-170">notificationSettings</span></span>|<span data-ttu-id="6cd33-171">Коллекция [iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6cd33-171">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="6cd33-172">Параметры уведомления для каждого идентификатора пакета. Применимы только к устройствам, находящимся в защищенном режиме (для iOS 9.3 и более поздних версий).</span><span class="sxs-lookup"><span data-stu-id="6cd33-172">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="6cd33-173">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="6cd33-173">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="6cd33-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cd33-174">Response</span></span>
<span data-ttu-id="6cd33-175">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6cd33-175">If successful, this method returns a `201 Created` response code and a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cd33-176">Пример</span><span class="sxs-lookup"><span data-stu-id="6cd33-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cd33-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cd33-177">Request</span></span>
<span data-ttu-id="6cd33-178">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cd33-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6cd33-179">Ответ</span><span class="sxs-lookup"><span data-stu-id="6cd33-179">Response</span></span>
<span data-ttu-id="6cd33-p112">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6cd33-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



