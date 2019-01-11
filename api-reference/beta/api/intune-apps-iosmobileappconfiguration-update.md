---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e0780bb5d59ee690755b59ea7eeed38d0ed87fc9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819497"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="2fd52-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fd52-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="2fd52-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2fd52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fd52-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fd52-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2fd52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fd52-107">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd52-107">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fd52-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="2fd52-108">Prerequisites</span></span>
<span data-ttu-id="2fd52-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fd52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fd52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2fd52-111">Permission type</span></span>|<span data-ttu-id="2fd52-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2fd52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fd52-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2fd52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fd52-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fd52-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2fd52-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2fd52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fd52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd52-116">Not supported.</span></span>|
|<span data-ttu-id="2fd52-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2fd52-117">Application</span></span>|<span data-ttu-id="2fd52-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fd52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fd52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2fd52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2fd52-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2fd52-120">Request headers</span></span>
|<span data-ttu-id="2fd52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2fd52-121">Header</span></span>|<span data-ttu-id="2fd52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2fd52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fd52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fd52-123">Authorization</span></span>|<span data-ttu-id="2fd52-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2fd52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fd52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fd52-125">Accept</span></span>|<span data-ttu-id="2fd52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fd52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fd52-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2fd52-127">Request body</span></span>
<span data-ttu-id="2fd52-128">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fd52-128">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="2fd52-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2fd52-129">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="2fd52-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fd52-130">Property</span></span>|<span data-ttu-id="2fd52-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2fd52-131">Type</span></span>|<span data-ttu-id="2fd52-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2fd52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd52-133">id</span><span class="sxs-lookup"><span data-stu-id="2fd52-133">id</span></span>|<span data-ttu-id="2fd52-134">Строка</span><span class="sxs-lookup"><span data-stu-id="2fd52-134">String</span></span>|<span data-ttu-id="2fd52-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2fd52-135">Key of the entity.</span></span> <span data-ttu-id="2fd52-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2fd52-137">targetedMobileApps</span></span>|<span data-ttu-id="2fd52-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2fd52-138">String collection</span></span>|<span data-ttu-id="2fd52-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="2fd52-139">the associated app.</span></span> <span data-ttu-id="2fd52-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fd52-141">roleScopeTagIds</span></span>|<span data-ttu-id="2fd52-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2fd52-142">String collection</span></span>|<span data-ttu-id="2fd52-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2fd52-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="2fd52-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd52-145">createdDateTime</span></span>|<span data-ttu-id="2fd52-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd52-146">DateTimeOffset</span></span>|<span data-ttu-id="2fd52-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2fd52-147">DateTime the object was created.</span></span> <span data-ttu-id="2fd52-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-149">описание</span><span class="sxs-lookup"><span data-stu-id="2fd52-149">description</span></span>|<span data-ttu-id="2fd52-150">Строка</span><span class="sxs-lookup"><span data-stu-id="2fd52-150">String</span></span>|<span data-ttu-id="2fd52-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="2fd52-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2fd52-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fd52-153">lastModifiedDateTime</span></span>|<span data-ttu-id="2fd52-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fd52-154">DateTimeOffset</span></span>|<span data-ttu-id="2fd52-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2fd52-155">DateTime the object was last modified.</span></span> <span data-ttu-id="2fd52-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-157">displayName</span><span class="sxs-lookup"><span data-stu-id="2fd52-157">displayName</span></span>|<span data-ttu-id="2fd52-158">Строка</span><span class="sxs-lookup"><span data-stu-id="2fd52-158">String</span></span>|<span data-ttu-id="2fd52-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2fd52-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2fd52-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-161">версия</span><span class="sxs-lookup"><span data-stu-id="2fd52-161">version</span></span>|<span data-ttu-id="2fd52-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2fd52-162">Int32</span></span>|<span data-ttu-id="2fd52-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2fd52-163">Version of the device configuration.</span></span> <span data-ttu-id="2fd52-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="2fd52-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="2fd52-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="2fd52-165">encodedSettingXml</span></span>|<span data-ttu-id="2fd52-166">Двоичный</span><span class="sxs-lookup"><span data-stu-id="2fd52-166">Binary</span></span>|<span data-ttu-id="2fd52-167">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="2fd52-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="2fd52-168">параметры</span><span class="sxs-lookup"><span data-stu-id="2fd52-168">settings</span></span>|<span data-ttu-id="2fd52-169">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="2fd52-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="2fd52-170">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="2fd52-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="2fd52-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fd52-171">Response</span></span>
<span data-ttu-id="2fd52-172">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="2fd52-172">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fd52-173">Пример</span><span class="sxs-lookup"><span data-stu-id="2fd52-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fd52-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="2fd52-174">Request</span></span>
<span data-ttu-id="2fd52-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2fd52-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
Content-type: application/json
Content-length: 596

{
  "targetedMobileApps": [
    "Targeted Mobile Apps value"
  ],
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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

### <a name="response"></a><span data-ttu-id="2fd52-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="2fd52-176">Response</span></span>
<span data-ttu-id="2fd52-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2fd52-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





