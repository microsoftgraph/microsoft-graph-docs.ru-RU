---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 754ad2470797262f9f1cd52741a45500ec3d4096
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756283"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="8668d-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8668d-103">Update macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="8668d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8668d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8668d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8668d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8668d-106">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8668d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="8668d-107">Prerequisites</span></span>
<span data-ttu-id="8668d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8668d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8668d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8668d-110">Permission type</span></span>|<span data-ttu-id="8668d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8668d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8668d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8668d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8668d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8668d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8668d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8668d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8668d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8668d-115">Not supported.</span></span>|
|<span data-ttu-id="8668d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="8668d-116">Application</span></span>|<span data-ttu-id="8668d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8668d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8668d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8668d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8668d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8668d-119">Request headers</span></span>
|<span data-ttu-id="8668d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8668d-120">Header</span></span>|<span data-ttu-id="8668d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8668d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8668d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8668d-122">Authorization</span></span>|<span data-ttu-id="8668d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8668d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8668d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8668d-124">Accept</span></span>|<span data-ttu-id="8668d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8668d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8668d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8668d-126">Request body</span></span>
<span data-ttu-id="8668d-127">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8668d-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="8668d-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="8668d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8668d-129">Property</span></span>|<span data-ttu-id="8668d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8668d-130">Type</span></span>|<span data-ttu-id="8668d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8668d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8668d-132">id</span><span class="sxs-lookup"><span data-stu-id="8668d-132">id</span></span>|<span data-ttu-id="8668d-133">String</span><span class="sxs-lookup"><span data-stu-id="8668d-133">String</span></span>|<span data-ttu-id="8668d-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8668d-134">Key of the entity.</span></span> <span data-ttu-id="8668d-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8668d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8668d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8668d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8668d-137">DateTimeOffset</span></span>|<span data-ttu-id="8668d-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="8668d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8668d-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8668d-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8668d-140">createdDateTime</span></span>|<span data-ttu-id="8668d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8668d-141">DateTimeOffset</span></span>|<span data-ttu-id="8668d-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="8668d-142">DateTime the object was created.</span></span> <span data-ttu-id="8668d-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8668d-144">description</span><span class="sxs-lookup"><span data-stu-id="8668d-144">description</span></span>|<span data-ttu-id="8668d-145">String</span><span class="sxs-lookup"><span data-stu-id="8668d-145">String</span></span>|<span data-ttu-id="8668d-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8668d-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8668d-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8668d-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8668d-148">displayName</span></span>|<span data-ttu-id="8668d-149">String</span><span class="sxs-lookup"><span data-stu-id="8668d-149">String</span></span>|<span data-ttu-id="8668d-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8668d-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8668d-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8668d-152">version</span><span class="sxs-lookup"><span data-stu-id="8668d-152">version</span></span>|<span data-ttu-id="8668d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8668d-153">Int32</span></span>|<span data-ttu-id="8668d-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="8668d-154">Version of the device configuration.</span></span> <span data-ttu-id="8668d-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8668d-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8668d-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="8668d-156">Response</span></span>
<span data-ttu-id="8668d-157">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8668d-157">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8668d-158">Пример</span><span class="sxs-lookup"><span data-stu-id="8668d-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="8668d-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="8668d-159">Request</span></span>
<span data-ttu-id="8668d-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8668d-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8668d-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="8668d-161">Response</span></span>
<span data-ttu-id="8668d-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8668d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




