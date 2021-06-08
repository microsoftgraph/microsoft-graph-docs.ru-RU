---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: facb9911f634c3a747e3f98647d3c8c63133887b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760582"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="07348-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="07348-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="07348-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07348-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07348-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07348-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07348-106">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07348-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="07348-107">Prerequisites</span></span>
<span data-ttu-id="07348-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07348-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07348-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="07348-110">Permission type</span></span>|<span data-ttu-id="07348-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="07348-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07348-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="07348-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07348-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07348-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07348-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="07348-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07348-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07348-115">Not supported.</span></span>|
|<span data-ttu-id="07348-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="07348-116">Application</span></span>|<span data-ttu-id="07348-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07348-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07348-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="07348-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="07348-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="07348-119">Request headers</span></span>
|<span data-ttu-id="07348-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="07348-120">Header</span></span>|<span data-ttu-id="07348-121">Значение</span><span class="sxs-lookup"><span data-stu-id="07348-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07348-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07348-122">Authorization</span></span>|<span data-ttu-id="07348-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="07348-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07348-124">Accept</span><span class="sxs-lookup"><span data-stu-id="07348-124">Accept</span></span>|<span data-ttu-id="07348-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07348-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07348-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="07348-126">Request body</span></span>
<span data-ttu-id="07348-127">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07348-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="07348-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="07348-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="07348-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="07348-129">Property</span></span>|<span data-ttu-id="07348-130">Тип</span><span class="sxs-lookup"><span data-stu-id="07348-130">Type</span></span>|<span data-ttu-id="07348-131">Описание</span><span class="sxs-lookup"><span data-stu-id="07348-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07348-132">id</span><span class="sxs-lookup"><span data-stu-id="07348-132">id</span></span>|<span data-ttu-id="07348-133">String</span><span class="sxs-lookup"><span data-stu-id="07348-133">String</span></span>|<span data-ttu-id="07348-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="07348-134">Key of the entity.</span></span> <span data-ttu-id="07348-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07348-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="07348-136">lastModifiedDateTime</span></span>|<span data-ttu-id="07348-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07348-137">DateTimeOffset</span></span>|<span data-ttu-id="07348-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="07348-138">DateTime the object was last modified.</span></span> <span data-ttu-id="07348-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07348-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="07348-140">createdDateTime</span></span>|<span data-ttu-id="07348-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07348-141">DateTimeOffset</span></span>|<span data-ttu-id="07348-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="07348-142">DateTime the object was created.</span></span> <span data-ttu-id="07348-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07348-144">description</span><span class="sxs-lookup"><span data-stu-id="07348-144">description</span></span>|<span data-ttu-id="07348-145">String</span><span class="sxs-lookup"><span data-stu-id="07348-145">String</span></span>|<span data-ttu-id="07348-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07348-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="07348-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07348-148">displayName</span><span class="sxs-lookup"><span data-stu-id="07348-148">displayName</span></span>|<span data-ttu-id="07348-149">String</span><span class="sxs-lookup"><span data-stu-id="07348-149">String</span></span>|<span data-ttu-id="07348-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07348-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="07348-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="07348-152">version</span><span class="sxs-lookup"><span data-stu-id="07348-152">version</span></span>|<span data-ttu-id="07348-153">Int32</span><span class="sxs-lookup"><span data-stu-id="07348-153">Int32</span></span>|<span data-ttu-id="07348-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="07348-154">Version of the device configuration.</span></span> <span data-ttu-id="07348-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="07348-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="07348-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="07348-156">Response</span></span>
<span data-ttu-id="07348-157">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="07348-157">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07348-158">Пример</span><span class="sxs-lookup"><span data-stu-id="07348-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="07348-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="07348-159">Request</span></span>
<span data-ttu-id="07348-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="07348-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="07348-161">Отклик</span><span class="sxs-lookup"><span data-stu-id="07348-161">Response</span></span>
<span data-ttu-id="07348-p108">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="07348-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




