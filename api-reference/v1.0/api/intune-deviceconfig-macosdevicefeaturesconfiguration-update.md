---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e472c0775f8317b2abac0c8481ec882b09afe87
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514335"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a6e65-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6e65-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="a6e65-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6e65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6e65-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6e65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e65-106">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6e65-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a6e65-107">Prerequisites</span></span>
<span data-ttu-id="a6e65-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e65-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e65-110">Permission type</span></span>|<span data-ttu-id="a6e65-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6e65-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6e65-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6e65-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6e65-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e65-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6e65-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6e65-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6e65-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6e65-115">Not supported.</span></span>|
|<span data-ttu-id="a6e65-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6e65-116">Application</span></span>|<span data-ttu-id="a6e65-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6e65-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6e65-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6e65-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a6e65-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="a6e65-119">Request headers</span></span>
|<span data-ttu-id="a6e65-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a6e65-120">Header</span></span>|<span data-ttu-id="a6e65-121">Значение</span><span class="sxs-lookup"><span data-stu-id="a6e65-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6e65-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6e65-122">Authorization</span></span>|<span data-ttu-id="a6e65-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6e65-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6e65-124">Accept</span><span class="sxs-lookup"><span data-stu-id="a6e65-124">Accept</span></span>|<span data-ttu-id="a6e65-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e65-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6e65-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6e65-126">Request body</span></span>
<span data-ttu-id="a6e65-127">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6e65-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="a6e65-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="a6e65-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6e65-129">Property</span></span>|<span data-ttu-id="a6e65-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a6e65-130">Type</span></span>|<span data-ttu-id="a6e65-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a6e65-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6e65-132">id</span><span class="sxs-lookup"><span data-stu-id="a6e65-132">id</span></span>|<span data-ttu-id="a6e65-133">String</span><span class="sxs-lookup"><span data-stu-id="a6e65-133">String</span></span>|<span data-ttu-id="a6e65-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a6e65-134">Key of the entity.</span></span> <span data-ttu-id="a6e65-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e65-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a6e65-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e65-137">DateTimeOffset</span></span>|<span data-ttu-id="a6e65-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a6e65-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a6e65-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e65-140">createdDateTime</span></span>|<span data-ttu-id="a6e65-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e65-141">DateTimeOffset</span></span>|<span data-ttu-id="a6e65-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a6e65-142">DateTime the object was created.</span></span> <span data-ttu-id="a6e65-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-144">description</span><span class="sxs-lookup"><span data-stu-id="a6e65-144">description</span></span>|<span data-ttu-id="a6e65-145">String</span><span class="sxs-lookup"><span data-stu-id="a6e65-145">String</span></span>|<span data-ttu-id="a6e65-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6e65-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a6e65-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e65-148">displayName</span></span>|<span data-ttu-id="a6e65-149">Строка</span><span class="sxs-lookup"><span data-stu-id="a6e65-149">String</span></span>|<span data-ttu-id="a6e65-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6e65-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a6e65-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a6e65-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a6e65-152">version</span><span class="sxs-lookup"><span data-stu-id="a6e65-152">version</span></span>|<span data-ttu-id="a6e65-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a6e65-153">Int32</span></span>|<span data-ttu-id="a6e65-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a6e65-154">Version of the device configuration.</span></span> <span data-ttu-id="a6e65-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a6e65-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a6e65-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e65-156">Response</span></span>
<span data-ttu-id="a6e65-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a6e65-157">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6e65-158">Пример</span><span class="sxs-lookup"><span data-stu-id="a6e65-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6e65-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6e65-159">Request</span></span>
<span data-ttu-id="a6e65-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6e65-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a6e65-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e65-161">Response</span></span>
<span data-ttu-id="a6e65-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6e65-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```




