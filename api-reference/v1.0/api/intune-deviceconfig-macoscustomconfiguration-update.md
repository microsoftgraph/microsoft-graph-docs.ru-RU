---
title: Обновление объекта macOSCustomConfiguration
description: Обновление свойств объекта macOSCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 593ad00a4d88ed9e55a273e1bdb90a3da0bf19fd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388060"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="e0312-103">Обновление объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0312-103">Update macOSCustomConfiguration</span></span>

<span data-ttu-id="e0312-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0312-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0312-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e0312-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0312-106">Обновление свойств объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-106">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0312-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e0312-107">Prerequisites</span></span>
<span data-ttu-id="e0312-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0312-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0312-110">Permission type</span></span>|<span data-ttu-id="e0312-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0312-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0312-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0312-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0312-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0312-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0312-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0312-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0312-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0312-115">Not supported.</span></span>|
|<span data-ttu-id="e0312-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0312-116">Application</span></span>|<span data-ttu-id="e0312-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0312-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0312-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0312-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0312-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e0312-119">Request headers</span></span>
|<span data-ttu-id="e0312-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0312-120">Header</span></span>|<span data-ttu-id="e0312-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e0312-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0312-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0312-122">Authorization</span></span>|<span data-ttu-id="e0312-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0312-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0312-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e0312-124">Accept</span></span>|<span data-ttu-id="e0312-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0312-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0312-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0312-126">Request body</span></span>
<span data-ttu-id="e0312-127">В теле запроса добавьте представление объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0312-127">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="e0312-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-128">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="e0312-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0312-129">Property</span></span>|<span data-ttu-id="e0312-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e0312-130">Type</span></span>|<span data-ttu-id="e0312-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e0312-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0312-132">id</span><span class="sxs-lookup"><span data-stu-id="e0312-132">id</span></span>|<span data-ttu-id="e0312-133">Строка</span><span class="sxs-lookup"><span data-stu-id="e0312-133">String</span></span>|<span data-ttu-id="e0312-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e0312-134">Key of the entity.</span></span> <span data-ttu-id="e0312-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0312-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e0312-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0312-137">DateTimeOffset</span></span>|<span data-ttu-id="e0312-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="e0312-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e0312-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0312-140">createdDateTime</span></span>|<span data-ttu-id="e0312-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0312-141">DateTimeOffset</span></span>|<span data-ttu-id="e0312-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="e0312-142">DateTime the object was created.</span></span> <span data-ttu-id="e0312-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-144">description</span><span class="sxs-lookup"><span data-stu-id="e0312-144">description</span></span>|<span data-ttu-id="e0312-145">String</span><span class="sxs-lookup"><span data-stu-id="e0312-145">String</span></span>|<span data-ttu-id="e0312-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0312-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0312-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e0312-148">displayName</span></span>|<span data-ttu-id="e0312-149">Строка</span><span class="sxs-lookup"><span data-stu-id="e0312-149">String</span></span>|<span data-ttu-id="e0312-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0312-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0312-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0312-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-152">version</span><span class="sxs-lookup"><span data-stu-id="e0312-152">version</span></span>|<span data-ttu-id="e0312-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e0312-153">Int32</span></span>|<span data-ttu-id="e0312-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="e0312-154">Version of the device configuration.</span></span> <span data-ttu-id="e0312-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e0312-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0312-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="e0312-156">payloadName</span></span>|<span data-ttu-id="e0312-157">String</span><span class="sxs-lookup"><span data-stu-id="e0312-157">String</span></span>|<span data-ttu-id="e0312-158">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="e0312-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="e0312-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e0312-159">payloadFileName</span></span>|<span data-ttu-id="e0312-160">String</span><span class="sxs-lookup"><span data-stu-id="e0312-160">String</span></span>|<span data-ttu-id="e0312-161">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="e0312-161">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="e0312-162">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="e0312-162">\*.xml).</span></span>|
|<span data-ttu-id="e0312-163">payload</span><span class="sxs-lookup"><span data-stu-id="e0312-163">payload</span></span>|<span data-ttu-id="e0312-164">Binary</span><span class="sxs-lookup"><span data-stu-id="e0312-164">Binary</span></span>|<span data-ttu-id="e0312-165">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="e0312-165">Payload.</span></span> <span data-ttu-id="e0312-166">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="e0312-166">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="e0312-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0312-167">Response</span></span>
<span data-ttu-id="e0312-168">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e0312-168">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0312-169">Пример</span><span class="sxs-lookup"><span data-stu-id="e0312-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0312-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0312-170">Request</span></span>
<span data-ttu-id="e0312-171">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0312-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="e0312-172">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0312-172">Response</span></span>
<span data-ttu-id="e0312-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e0312-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```






