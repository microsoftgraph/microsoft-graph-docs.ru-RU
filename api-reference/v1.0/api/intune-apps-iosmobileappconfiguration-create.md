---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d5ada7a620a131e17a3403ad8c30b52ca4ab5c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577324"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="d81b2-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d81b2-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="d81b2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d81b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d81b2-105">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d81b2-105">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d81b2-106">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="d81b2-106">Prerequisites</span></span>
<span data-ttu-id="d81b2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d81b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d81b2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d81b2-109">Permission type</span></span>|<span data-ttu-id="d81b2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d81b2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d81b2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d81b2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d81b2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d81b2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d81b2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d81b2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d81b2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d81b2-114">Not supported.</span></span>|
|<span data-ttu-id="d81b2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d81b2-115">Application</span></span>|<span data-ttu-id="d81b2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d81b2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d81b2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d81b2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d81b2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d81b2-118">Request headers</span></span>
|<span data-ttu-id="d81b2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d81b2-119">Header</span></span>|<span data-ttu-id="d81b2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="d81b2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d81b2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d81b2-121">Authorization</span></span>|<span data-ttu-id="d81b2-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d81b2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d81b2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d81b2-123">Accept</span></span>|<span data-ttu-id="d81b2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d81b2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d81b2-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d81b2-125">Request body</span></span>
<span data-ttu-id="d81b2-126">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d81b2-126">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="d81b2-127">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d81b2-127">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="d81b2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="d81b2-128">Property</span></span>|<span data-ttu-id="d81b2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d81b2-129">Type</span></span>|<span data-ttu-id="d81b2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d81b2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d81b2-131">id</span><span class="sxs-lookup"><span data-stu-id="d81b2-131">id</span></span>|<span data-ttu-id="d81b2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="d81b2-132">String</span></span>|<span data-ttu-id="d81b2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d81b2-133">Key of the entity.</span></span> <span data-ttu-id="d81b2-134">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-134">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-135">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d81b2-135">targetedMobileApps</span></span>|<span data-ttu-id="d81b2-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d81b2-136">String collection</span></span>|<span data-ttu-id="d81b2-137">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="d81b2-137">the associated app.</span></span> <span data-ttu-id="d81b2-138">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-138">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d81b2-139">createdDateTime</span></span>|<span data-ttu-id="d81b2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81b2-140">DateTimeOffset</span></span>|<span data-ttu-id="d81b2-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d81b2-141">DateTime the object was created.</span></span> <span data-ttu-id="d81b2-142">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-142">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-143">description</span><span class="sxs-lookup"><span data-stu-id="d81b2-143">description</span></span>|<span data-ttu-id="d81b2-144">String</span><span class="sxs-lookup"><span data-stu-id="d81b2-144">String</span></span>|<span data-ttu-id="d81b2-145">Администратор предоставил описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d81b2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d81b2-146">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-146">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d81b2-147">lastModifiedDateTime</span></span>|<span data-ttu-id="d81b2-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d81b2-148">DateTimeOffset</span></span>|<span data-ttu-id="d81b2-149">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d81b2-149">DateTime the object was last modified.</span></span> <span data-ttu-id="d81b2-150">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-150">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-151">displayName</span><span class="sxs-lookup"><span data-stu-id="d81b2-151">displayName</span></span>|<span data-ttu-id="d81b2-152">String</span><span class="sxs-lookup"><span data-stu-id="d81b2-152">String</span></span>|<span data-ttu-id="d81b2-153">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d81b2-153">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d81b2-154">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-154">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-155">версия</span><span class="sxs-lookup"><span data-stu-id="d81b2-155">version</span></span>|<span data-ttu-id="d81b2-156">Int32</span><span class="sxs-lookup"><span data-stu-id="d81b2-156">Int32</span></span>|<span data-ttu-id="d81b2-157">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d81b2-157">Version of the device configuration.</span></span> <span data-ttu-id="d81b2-158">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-158">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="d81b2-159">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="d81b2-159">encodedSettingXml</span></span>|<span data-ttu-id="d81b2-160">Двоичный</span><span class="sxs-lookup"><span data-stu-id="d81b2-160">Binary</span></span>|<span data-ttu-id="d81b2-161">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="d81b2-161">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="d81b2-162">параметры</span><span class="sxs-lookup"><span data-stu-id="d81b2-162">settings</span></span>|<span data-ttu-id="d81b2-163">Сбор данных [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="d81b2-163">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="d81b2-164">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="d81b2-164">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="d81b2-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="d81b2-165">Response</span></span>
<span data-ttu-id="d81b2-166">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="d81b2-166">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d81b2-167">Пример</span><span class="sxs-lookup"><span data-stu-id="d81b2-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d81b2-168">Запрос</span><span class="sxs-lookup"><span data-stu-id="d81b2-168">Request</span></span>
<span data-ttu-id="d81b2-169">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d81b2-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations
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

### <a name="response"></a><span data-ttu-id="d81b2-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="d81b2-170">Response</span></span>
<span data-ttu-id="d81b2-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d81b2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



