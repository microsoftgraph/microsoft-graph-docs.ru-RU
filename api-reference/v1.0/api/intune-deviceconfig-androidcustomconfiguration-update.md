---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b40b9872f3ac1b14a9eea245be297d8939963550
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474665"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="ba70e-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba70e-103">Update androidCustomConfiguration</span></span>

<span data-ttu-id="ba70e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba70e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba70e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ba70e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba70e-106">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-106">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba70e-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="ba70e-107">Prerequisites</span></span>
<span data-ttu-id="ba70e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba70e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba70e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba70e-110">Permission type</span></span>|<span data-ttu-id="ba70e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba70e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba70e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba70e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba70e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba70e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ba70e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba70e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba70e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba70e-115">Not supported.</span></span>|
|<span data-ttu-id="ba70e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba70e-116">Application</span></span>|<span data-ttu-id="ba70e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba70e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba70e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba70e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ba70e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ba70e-119">Request headers</span></span>
|<span data-ttu-id="ba70e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba70e-120">Header</span></span>|<span data-ttu-id="ba70e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ba70e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba70e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba70e-122">Authorization</span></span>|<span data-ttu-id="ba70e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba70e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba70e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ba70e-124">Accept</span></span>|<span data-ttu-id="ba70e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba70e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba70e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba70e-126">Request body</span></span>
<span data-ttu-id="ba70e-127">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ba70e-127">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="ba70e-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-128">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="ba70e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ba70e-129">Property</span></span>|<span data-ttu-id="ba70e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ba70e-130">Type</span></span>|<span data-ttu-id="ba70e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ba70e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba70e-132">id</span><span class="sxs-lookup"><span data-stu-id="ba70e-132">id</span></span>|<span data-ttu-id="ba70e-133">String</span><span class="sxs-lookup"><span data-stu-id="ba70e-133">String</span></span>|<span data-ttu-id="ba70e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ba70e-134">Key of the entity.</span></span> <span data-ttu-id="ba70e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba70e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ba70e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba70e-137">DateTimeOffset</span></span>|<span data-ttu-id="ba70e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="ba70e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ba70e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba70e-140">createdDateTime</span></span>|<span data-ttu-id="ba70e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba70e-141">DateTimeOffset</span></span>|<span data-ttu-id="ba70e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="ba70e-142">DateTime the object was created.</span></span> <span data-ttu-id="ba70e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-144">description</span><span class="sxs-lookup"><span data-stu-id="ba70e-144">description</span></span>|<span data-ttu-id="ba70e-145">String</span><span class="sxs-lookup"><span data-stu-id="ba70e-145">String</span></span>|<span data-ttu-id="ba70e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba70e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ba70e-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="ba70e-148">displayName</span></span>|<span data-ttu-id="ba70e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="ba70e-149">String</span></span>|<span data-ttu-id="ba70e-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba70e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ba70e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ba70e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-152">version</span><span class="sxs-lookup"><span data-stu-id="ba70e-152">version</span></span>|<span data-ttu-id="ba70e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ba70e-153">Int32</span></span>|<span data-ttu-id="ba70e-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="ba70e-154">Version of the device configuration.</span></span> <span data-ttu-id="ba70e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ba70e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ba70e-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ba70e-156">omaSettings</span></span>|<span data-ttu-id="ba70e-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba70e-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ba70e-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="ba70e-158">OMA settings.</span></span> <span data-ttu-id="ba70e-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="ba70e-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ba70e-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba70e-160">Response</span></span>
<span data-ttu-id="ba70e-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ba70e-161">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba70e-162">Пример</span><span class="sxs-lookup"><span data-stu-id="ba70e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba70e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba70e-163">Request</span></span>
<span data-ttu-id="ba70e-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba70e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="ba70e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba70e-165">Response</span></span>
<span data-ttu-id="ba70e-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba70e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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






