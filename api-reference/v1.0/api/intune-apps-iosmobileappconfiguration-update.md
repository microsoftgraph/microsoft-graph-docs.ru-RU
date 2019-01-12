---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 298ca5b76b82f43daee84f7d2a36cbb0e12b058d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942124"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="3bf03-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bf03-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="3bf03-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3bf03-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bf03-105">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bf03-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bf03-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="3bf03-106">Prerequisites</span></span>
<span data-ttu-id="3bf03-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bf03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bf03-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3bf03-109">Permission type</span></span>|<span data-ttu-id="3bf03-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3bf03-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bf03-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3bf03-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3bf03-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bf03-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bf03-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3bf03-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bf03-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf03-114">Not supported.</span></span>|
|<span data-ttu-id="3bf03-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3bf03-115">Application</span></span>|<span data-ttu-id="3bf03-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3bf03-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bf03-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3bf03-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3bf03-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3bf03-118">Request headers</span></span>
|<span data-ttu-id="3bf03-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3bf03-119">Header</span></span>|<span data-ttu-id="3bf03-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3bf03-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bf03-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bf03-121">Authorization</span></span>|<span data-ttu-id="3bf03-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3bf03-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bf03-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3bf03-123">Accept</span></span>|<span data-ttu-id="3bf03-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3bf03-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bf03-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3bf03-125">Request body</span></span>
<span data-ttu-id="3bf03-126">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3bf03-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="3bf03-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3bf03-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="3bf03-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3bf03-128">Property</span></span>|<span data-ttu-id="3bf03-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3bf03-129">Type</span></span>|<span data-ttu-id="3bf03-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3bf03-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bf03-131">id</span><span class="sxs-lookup"><span data-stu-id="3bf03-131">id</span></span>|<span data-ttu-id="3bf03-132">String</span><span class="sxs-lookup"><span data-stu-id="3bf03-132">String</span></span>|<span data-ttu-id="3bf03-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3bf03-133">Key of the entity.</span></span> <span data-ttu-id="3bf03-134">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3bf03-135">targetedMobileApps</span></span>|<span data-ttu-id="3bf03-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3bf03-136">String collection</span></span>|<span data-ttu-id="3bf03-137">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="3bf03-137">the associated app.</span></span> <span data-ttu-id="3bf03-138">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3bf03-139">createdDateTime</span></span>|<span data-ttu-id="3bf03-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bf03-140">DateTimeOffset</span></span>|<span data-ttu-id="3bf03-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3bf03-141">DateTime the object was created.</span></span> <span data-ttu-id="3bf03-142">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-143">описание</span><span class="sxs-lookup"><span data-stu-id="3bf03-143">description</span></span>|<span data-ttu-id="3bf03-144">String</span><span class="sxs-lookup"><span data-stu-id="3bf03-144">String</span></span>|<span data-ttu-id="3bf03-145">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="3bf03-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3bf03-146">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3bf03-147">lastModifiedDateTime</span></span>|<span data-ttu-id="3bf03-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bf03-148">DateTimeOffset</span></span>|<span data-ttu-id="3bf03-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3bf03-149">DateTime the object was last modified.</span></span> <span data-ttu-id="3bf03-150">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-151">displayName</span><span class="sxs-lookup"><span data-stu-id="3bf03-151">displayName</span></span>|<span data-ttu-id="3bf03-152">String</span><span class="sxs-lookup"><span data-stu-id="3bf03-152">String</span></span>|<span data-ttu-id="3bf03-153">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bf03-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3bf03-154">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-155">версия</span><span class="sxs-lookup"><span data-stu-id="3bf03-155">version</span></span>|<span data-ttu-id="3bf03-156">Int32</span><span class="sxs-lookup"><span data-stu-id="3bf03-156">Int32</span></span>|<span data-ttu-id="3bf03-157">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3bf03-157">Version of the device configuration.</span></span> <span data-ttu-id="3bf03-158">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="3bf03-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="3bf03-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="3bf03-159">encodedSettingXml</span></span>|<span data-ttu-id="3bf03-160">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3bf03-160">Binary</span></span>|<span data-ttu-id="3bf03-161">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="3bf03-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="3bf03-162">параметры</span><span class="sxs-lookup"><span data-stu-id="3bf03-162">settings</span></span>|<span data-ttu-id="3bf03-163">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="3bf03-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="3bf03-164">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="3bf03-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="3bf03-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bf03-165">Response</span></span>
<span data-ttu-id="3bf03-166">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="3bf03-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bf03-167">Пример</span><span class="sxs-lookup"><span data-stu-id="3bf03-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bf03-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="3bf03-168">Request</span></span>
<span data-ttu-id="3bf03-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3bf03-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3bf03-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="3bf03-170">Response</span></span>
<span data-ttu-id="3bf03-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3bf03-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



