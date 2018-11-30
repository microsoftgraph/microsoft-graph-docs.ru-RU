---
title: Создать iosMobileAppConfiguration
description: Создание нового объекта iosMobileAppConfiguration.
ms.openlocfilehash: 089a3d499ac656421ed6b7e2f0fd3a3c9fcca079
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077521"
---
# <a name="create-iosmobileappconfiguration"></a><span data-ttu-id="62bb0-103">Создать iosMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="62bb0-103">Create iosMobileAppConfiguration</span></span>

> <span data-ttu-id="62bb0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="62bb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="62bb0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62bb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="62bb0-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62bb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62bb0-107">Создание нового объекта [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="62bb0-107">Create a new [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="62bb0-108">Обязательные требования</span><span class="sxs-lookup"><span data-stu-id="62bb0-108">Prerequisites</span></span>
<span data-ttu-id="62bb0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62bb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62bb0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="62bb0-111">Permission type</span></span>|<span data-ttu-id="62bb0-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="62bb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62bb0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="62bb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62bb0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62bb0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62bb0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="62bb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62bb0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62bb0-116">Not supported.</span></span>|
|<span data-ttu-id="62bb0-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="62bb0-117">Application</span></span>|<span data-ttu-id="62bb0-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="62bb0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62bb0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="62bb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="62bb0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="62bb0-120">Request headers</span></span>
|<span data-ttu-id="62bb0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="62bb0-121">Header</span></span>|<span data-ttu-id="62bb0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="62bb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62bb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62bb0-123">Authorization</span></span>|<span data-ttu-id="62bb0-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="62bb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62bb0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="62bb0-125">Accept</span></span>|<span data-ttu-id="62bb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62bb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62bb0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="62bb0-127">Request body</span></span>
<span data-ttu-id="62bb0-128">В тексте запроса добавьте представление объекта iosMobileAppConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62bb0-128">In the request body, supply a JSON representation for the iosMobileAppConfiguration object.</span></span>

<span data-ttu-id="62bb0-129">В следующей таблице указаны свойства, необходимые при создании iosMobileAppConfiguration.</span><span class="sxs-lookup"><span data-stu-id="62bb0-129">The following table shows the properties that are required when you create the iosMobileAppConfiguration.</span></span>

|<span data-ttu-id="62bb0-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="62bb0-130">Property</span></span>|<span data-ttu-id="62bb0-131">Тип</span><span class="sxs-lookup"><span data-stu-id="62bb0-131">Type</span></span>|<span data-ttu-id="62bb0-132">Описание</span><span class="sxs-lookup"><span data-stu-id="62bb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62bb0-133">id</span><span class="sxs-lookup"><span data-stu-id="62bb0-133">id</span></span>|<span data-ttu-id="62bb0-134">String</span><span class="sxs-lookup"><span data-stu-id="62bb0-134">String</span></span>|<span data-ttu-id="62bb0-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="62bb0-135">Key of the entity.</span></span> <span data-ttu-id="62bb0-136">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-136">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-137">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="62bb0-137">targetedMobileApps</span></span>|<span data-ttu-id="62bb0-138">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62bb0-138">String collection</span></span>|<span data-ttu-id="62bb0-139">приложение-обработчик</span><span class="sxs-lookup"><span data-stu-id="62bb0-139">the associated app.</span></span> <span data-ttu-id="62bb0-140">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-140">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62bb0-141">roleScopeTagIds</span></span>|<span data-ttu-id="62bb0-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62bb0-142">String collection</span></span>|<span data-ttu-id="62bb0-143">Список областей теги для данного объекта конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="62bb0-143">List of Scope Tags for this App configuration entity.</span></span> <span data-ttu-id="62bb0-144">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-144">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="62bb0-145">createdDateTime</span></span>|<span data-ttu-id="62bb0-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62bb0-146">DateTimeOffset</span></span>|<span data-ttu-id="62bb0-147">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="62bb0-147">DateTime the object was created.</span></span> <span data-ttu-id="62bb0-148">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-148">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-149">описание</span><span class="sxs-lookup"><span data-stu-id="62bb0-149">description</span></span>|<span data-ttu-id="62bb0-150">String</span><span class="sxs-lookup"><span data-stu-id="62bb0-150">String</span></span>|<span data-ttu-id="62bb0-151">Администратор предоставил описание конфигурация устройства.</span><span class="sxs-lookup"><span data-stu-id="62bb0-151">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="62bb0-152">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-152">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="62bb0-153">lastModifiedDateTime</span></span>|<span data-ttu-id="62bb0-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62bb0-154">DateTimeOffset</span></span>|<span data-ttu-id="62bb0-155">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="62bb0-155">DateTime the object was last modified.</span></span> <span data-ttu-id="62bb0-156">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-156">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-157">displayName</span><span class="sxs-lookup"><span data-stu-id="62bb0-157">displayName</span></span>|<span data-ttu-id="62bb0-158">String</span><span class="sxs-lookup"><span data-stu-id="62bb0-158">String</span></span>|<span data-ttu-id="62bb0-159">Администратор предоставил название конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62bb0-159">Admin provided name of the device configuration.</span></span> <span data-ttu-id="62bb0-160">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-160">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-161">версия</span><span class="sxs-lookup"><span data-stu-id="62bb0-161">version</span></span>|<span data-ttu-id="62bb0-162">Int32</span><span class="sxs-lookup"><span data-stu-id="62bb0-162">Int32</span></span>|<span data-ttu-id="62bb0-163">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="62bb0-163">Version of the device configuration.</span></span> <span data-ttu-id="62bb0-164">Унаследовано от [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md);</span><span class="sxs-lookup"><span data-stu-id="62bb0-164">Inherited from [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span></span>|
|<span data-ttu-id="62bb0-165">encodedSettingXml</span><span class="sxs-lookup"><span data-stu-id="62bb0-165">encodedSettingXml</span></span>|<span data-ttu-id="62bb0-166">Двоичный</span><span class="sxs-lookup"><span data-stu-id="62bb0-166">Binary</span></span>|<span data-ttu-id="62bb0-167">конфигурация приложения службы управления мобильными устройствами двоичная Base64.</span><span class="sxs-lookup"><span data-stu-id="62bb0-167">mdm app configuration Base64 binary.</span></span>|
|<span data-ttu-id="62bb0-168">параметры</span><span class="sxs-lookup"><span data-stu-id="62bb0-168">settings</span></span>|<span data-ttu-id="62bb0-169">коллекция [appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md)</span><span class="sxs-lookup"><span data-stu-id="62bb0-169">[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) collection</span></span>|<span data-ttu-id="62bb0-170">элементы параметра конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="62bb0-170">app configuration setting items.</span></span>|



## <a name="response"></a><span data-ttu-id="62bb0-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="62bb0-171">Response</span></span>
<span data-ttu-id="62bb0-172">В случае успешного выполнения данный метод возвращает `201 Created`код отклика и объект [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)в форме для обратной связи.</span><span class="sxs-lookup"><span data-stu-id="62bb0-172">If successful, this method returns a `201 Created` response code and a [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62bb0-173">Пример</span><span class="sxs-lookup"><span data-stu-id="62bb0-173">Example</span></span>
### <a name="request"></a><span data-ttu-id="62bb0-174">Запрос</span><span class="sxs-lookup"><span data-stu-id="62bb0-174">Request</span></span>
<span data-ttu-id="62bb0-175">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="62bb0-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
Content-type: application/json
Content-length: 660

{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="62bb0-176">Ответ</span><span class="sxs-lookup"><span data-stu-id="62bb0-176">Response</span></span>
<span data-ttu-id="62bb0-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="62bb0-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





