---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75080639484fc13ec37958e15c4823d86d8bbb4c
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "37354513"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="f2fef-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2fef-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="f2fef-104">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2fef-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2fef-105">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2fef-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f2fef-106">Prerequisites</span></span>
<span data-ttu-id="f2fef-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2fef-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2fef-109">Permission type</span></span>|<span data-ttu-id="f2fef-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2fef-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2fef-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2fef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2fef-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2fef-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f2fef-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2fef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2fef-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2fef-114">Not supported.</span></span>|
|<span data-ttu-id="f2fef-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2fef-115">Application</span></span>|<span data-ttu-id="f2fef-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2fef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2fef-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2fef-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f2fef-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f2fef-118">Request headers</span></span>
|<span data-ttu-id="f2fef-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f2fef-119">Header</span></span>|<span data-ttu-id="f2fef-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f2fef-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2fef-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2fef-121">Authorization</span></span>|<span data-ttu-id="f2fef-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2fef-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2fef-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f2fef-123">Accept</span></span>|<span data-ttu-id="f2fef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2fef-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2fef-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f2fef-125">Request body</span></span>
<span data-ttu-id="f2fef-126">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2fef-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="f2fef-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="f2fef-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2fef-128">Property</span></span>|<span data-ttu-id="f2fef-129">Тип</span><span class="sxs-lookup"><span data-stu-id="f2fef-129">Type</span></span>|<span data-ttu-id="f2fef-130">Описание</span><span class="sxs-lookup"><span data-stu-id="f2fef-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fef-131">id</span><span class="sxs-lookup"><span data-stu-id="f2fef-131">id</span></span>|<span data-ttu-id="f2fef-132">String</span><span class="sxs-lookup"><span data-stu-id="f2fef-132">String</span></span>|<span data-ttu-id="f2fef-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f2fef-133">Key of the entity.</span></span> <span data-ttu-id="f2fef-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fef-135">lastModifiedDateTime</span></span>|<span data-ttu-id="f2fef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fef-136">DateTimeOffset</span></span>|<span data-ttu-id="f2fef-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="f2fef-137">DateTime the object was last modified.</span></span> <span data-ttu-id="f2fef-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2fef-139">createdDateTime</span></span>|<span data-ttu-id="f2fef-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2fef-140">DateTimeOffset</span></span>|<span data-ttu-id="f2fef-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="f2fef-141">DateTime the object was created.</span></span> <span data-ttu-id="f2fef-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-143">description</span><span class="sxs-lookup"><span data-stu-id="f2fef-143">description</span></span>|<span data-ttu-id="f2fef-144">String</span><span class="sxs-lookup"><span data-stu-id="f2fef-144">String</span></span>|<span data-ttu-id="f2fef-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2fef-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f2fef-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-147">displayName</span><span class="sxs-lookup"><span data-stu-id="f2fef-147">displayName</span></span>|<span data-ttu-id="f2fef-148">Строка</span><span class="sxs-lookup"><span data-stu-id="f2fef-148">String</span></span>|<span data-ttu-id="f2fef-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2fef-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f2fef-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f2fef-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-151">version</span><span class="sxs-lookup"><span data-stu-id="f2fef-151">version</span></span>|<span data-ttu-id="f2fef-152">Int32</span><span class="sxs-lookup"><span data-stu-id="f2fef-152">Int32</span></span>|<span data-ttu-id="f2fef-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="f2fef-153">Version of the device configuration.</span></span> <span data-ttu-id="f2fef-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f2fef-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f2fef-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="f2fef-155">omaSettings</span></span>|<span data-ttu-id="f2fef-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f2fef-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="f2fef-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="f2fef-157">OMA settings.</span></span> <span data-ttu-id="f2fef-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="f2fef-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="f2fef-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="f2fef-159">Response</span></span>
<span data-ttu-id="f2fef-160">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f2fef-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2fef-161">Пример</span><span class="sxs-lookup"><span data-stu-id="f2fef-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2fef-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2fef-162">Request</span></span>
<span data-ttu-id="f2fef-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2fef-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2fef-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2fef-164">Response</span></span>
<span data-ttu-id="f2fef-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f2fef-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




