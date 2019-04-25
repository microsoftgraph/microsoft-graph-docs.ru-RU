---
title: Обновить iosMobileAppConfiguration
description: Обновление свойств объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2119d146e4fa2cd64bc3aa39368d749993471811
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577380"
---
# <a name="update-iosmobileappconfiguration"></a><span data-ttu-id="9898a-103">Обновить iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="9898a-103">Update iosMobileAppConfiguration</span></span>

> <span data-ttu-id="9898a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9898a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9898a-105">Обновление свойств объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9898a-105">Update the properties of a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9898a-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="9898a-106">Prerequisites</span></span>
<span data-ttu-id="9898a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9898a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9898a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9898a-109">Permission type</span></span>|<span data-ttu-id="9898a-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9898a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9898a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9898a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9898a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9898a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9898a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9898a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9898a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9898a-114">Not supported.</span></span>|
|<span data-ttu-id="9898a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9898a-115">Application</span></span>|<span data-ttu-id="9898a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9898a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9898a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9898a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9898a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9898a-118">Request headers</span></span>
|<span data-ttu-id="9898a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9898a-119">Header</span></span>|<span data-ttu-id="9898a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9898a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9898a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9898a-121">Authorization</span></span>|<span data-ttu-id="9898a-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9898a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9898a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9898a-123">Accept</span></span>|<span data-ttu-id="9898a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9898a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9898a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9898a-125">Request body</span></span>
<span data-ttu-id="9898a-126">В тексте запроса добавьте представление объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9898a-126">In the request body, supply a JSON representation for the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

<span data-ttu-id="9898a-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта[ iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9898a-127">The following table shows the properties that are required when you create the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span></span>

|<span data-ttu-id="9898a-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="9898a-128">Property</span></span>|<span data-ttu-id="9898a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="9898a-129">Type</span></span>|<span data-ttu-id="9898a-130">Описание</span><span class="sxs-lookup"><span data-stu-id="9898a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9898a-131">id</span><span class="sxs-lookup"><span data-stu-id="9898a-131">id</span></span>|<span data-ttu-id="9898a-132">Строка</span><span class="sxs-lookup"><span data-stu-id="9898a-132">String</span></span>|<span data-ttu-id="9898a-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9898a-133">Key of the entity.</span></span> <span data-ttu-id="9898a-134">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="9898a-135">targetedMobileApps</span></span>|<span data-ttu-id="9898a-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9898a-136">String collection</span></span>|<span data-ttu-id="9898a-137">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="9898a-137">the associated app.</span></span> <span data-ttu-id="9898a-138">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9898a-139">createdDateTime</span></span>|<span data-ttu-id="9898a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9898a-140">DateTimeOffset</span></span>|<span data-ttu-id="9898a-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9898a-141">DateTime the object was created.</span></span> <span data-ttu-id="9898a-142">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-143">description</span><span class="sxs-lookup"><span data-stu-id="9898a-143">description</span></span>|<span data-ttu-id="9898a-144">String</span><span class="sxs-lookup"><span data-stu-id="9898a-144">String</span></span>|<span data-ttu-id="9898a-145">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9898a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9898a-146">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9898a-147">lastModifiedDateTime</span></span>|<span data-ttu-id="9898a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9898a-148">DateTimeOffset</span></span>|<span data-ttu-id="9898a-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9898a-149">DateTime the object was last modified.</span></span> <span data-ttu-id="9898a-150">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-151">displayName</span><span class="sxs-lookup"><span data-stu-id="9898a-151">displayName</span></span>|<span data-ttu-id="9898a-152">String</span><span class="sxs-lookup"><span data-stu-id="9898a-152">String</span></span>|<span data-ttu-id="9898a-153">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9898a-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9898a-154">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-155">версия</span><span class="sxs-lookup"><span data-stu-id="9898a-155">version</span></span>|<span data-ttu-id="9898a-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9898a-156">Int32</span></span>|<span data-ttu-id="9898a-157">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9898a-157">Version of the device configuration.</span></span> <span data-ttu-id="9898a-158">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="9898a-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="9898a-159">encodedSettingXml</span></span>|<span data-ttu-id="9898a-160">Двоичный</span><span class="sxs-lookup"><span data-stu-id="9898a-160">Binary</span></span>|<span data-ttu-id="9898a-161">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="9898a-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="9898a-162">параметры</span><span class="sxs-lookup"><span data-stu-id="9898a-162">settings</span></span>|<span data-ttu-id="9898a-163">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="9898a-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="9898a-164">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="9898a-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="9898a-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="9898a-165">Response</span></span>
<span data-ttu-id="9898a-166">В случае успешного выполнения данный метод возвращает `200 OK`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="9898a-166">If successful, this method returns a `200 OK` response code and an updated [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9898a-167">Пример</span><span class="sxs-lookup"><span data-stu-id="9898a-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="9898a-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="9898a-168">Request</span></span>
<span data-ttu-id="9898a-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9898a-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9898a-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="9898a-170">Response</span></span>
<span data-ttu-id="9898a-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9898a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



