---
title: Обновление объекта windowsPhone81CustomConfiguration
description: Обновление свойств объекта windowsPhone81CustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33d658d6173752befba97452a0eb1d7e9ce960d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513740"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="3e610-103">Обновление объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e610-103">Update windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="3e610-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e610-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e610-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e610-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e610-106">Обновление свойств объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e610-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3e610-107">Prerequisites</span></span>
<span data-ttu-id="3e610-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e610-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e610-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e610-110">Permission type</span></span>|<span data-ttu-id="3e610-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e610-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e610-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e610-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3e610-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e610-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3e610-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e610-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e610-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e610-115">Not supported.</span></span>|
|<span data-ttu-id="3e610-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e610-116">Application</span></span>|<span data-ttu-id="3e610-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e610-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e610-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e610-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3e610-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="3e610-119">Request headers</span></span>
|<span data-ttu-id="3e610-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e610-120">Header</span></span>|<span data-ttu-id="3e610-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3e610-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e610-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e610-122">Authorization</span></span>|<span data-ttu-id="3e610-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e610-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e610-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3e610-124">Accept</span></span>|<span data-ttu-id="3e610-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3e610-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e610-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e610-126">Request body</span></span>
<span data-ttu-id="3e610-127">В теле запроса добавьте представление объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e610-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="3e610-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="3e610-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e610-129">Property</span></span>|<span data-ttu-id="3e610-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3e610-130">Type</span></span>|<span data-ttu-id="3e610-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3e610-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e610-132">id</span><span class="sxs-lookup"><span data-stu-id="3e610-132">id</span></span>|<span data-ttu-id="3e610-133">String</span><span class="sxs-lookup"><span data-stu-id="3e610-133">String</span></span>|<span data-ttu-id="3e610-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e610-134">Key of the entity.</span></span> <span data-ttu-id="3e610-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e610-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3e610-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e610-137">DateTimeOffset</span></span>|<span data-ttu-id="3e610-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3e610-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3e610-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e610-140">createdDateTime</span></span>|<span data-ttu-id="3e610-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e610-141">DateTimeOffset</span></span>|<span data-ttu-id="3e610-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3e610-142">DateTime the object was created.</span></span> <span data-ttu-id="3e610-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-144">description</span><span class="sxs-lookup"><span data-stu-id="3e610-144">description</span></span>|<span data-ttu-id="3e610-145">String</span><span class="sxs-lookup"><span data-stu-id="3e610-145">String</span></span>|<span data-ttu-id="3e610-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e610-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3e610-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3e610-148">displayName</span></span>|<span data-ttu-id="3e610-149">Строка</span><span class="sxs-lookup"><span data-stu-id="3e610-149">String</span></span>|<span data-ttu-id="3e610-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e610-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3e610-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3e610-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-152">version</span><span class="sxs-lookup"><span data-stu-id="3e610-152">version</span></span>|<span data-ttu-id="3e610-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3e610-153">Int32</span></span>|<span data-ttu-id="3e610-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3e610-154">Version of the device configuration.</span></span> <span data-ttu-id="3e610-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3e610-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3e610-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="3e610-156">omaSettings</span></span>|<span data-ttu-id="3e610-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3e610-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="3e610-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="3e610-158">OMA settings.</span></span> <span data-ttu-id="3e610-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="3e610-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3e610-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e610-160">Response</span></span>
<span data-ttu-id="3e610-161">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3e610-161">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e610-162">Пример</span><span class="sxs-lookup"><span data-stu-id="3e610-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e610-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e610-163">Request</span></span>
<span data-ttu-id="3e610-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e610-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3e610-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e610-165">Response</span></span>
<span data-ttu-id="3e610-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e610-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




