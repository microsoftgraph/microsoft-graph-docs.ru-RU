---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a9c22f05bc3d847fc1db1bd41f77ac0178c6ae8b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515338"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="25f31-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="25f31-103">Update androidCustomConfiguration</span></span>

<span data-ttu-id="25f31-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25f31-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25f31-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="25f31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25f31-106">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-106">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25f31-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="25f31-107">Prerequisites</span></span>
<span data-ttu-id="25f31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25f31-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="25f31-110">Permission type</span></span>|<span data-ttu-id="25f31-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="25f31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25f31-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="25f31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25f31-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25f31-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25f31-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="25f31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25f31-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25f31-115">Not supported.</span></span>|
|<span data-ttu-id="25f31-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="25f31-116">Application</span></span>|<span data-ttu-id="25f31-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="25f31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25f31-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="25f31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="25f31-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="25f31-119">Request headers</span></span>
|<span data-ttu-id="25f31-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="25f31-120">Header</span></span>|<span data-ttu-id="25f31-121">Значение</span><span class="sxs-lookup"><span data-stu-id="25f31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25f31-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25f31-122">Authorization</span></span>|<span data-ttu-id="25f31-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="25f31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25f31-124">Accept</span><span class="sxs-lookup"><span data-stu-id="25f31-124">Accept</span></span>|<span data-ttu-id="25f31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25f31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25f31-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="25f31-126">Request body</span></span>
<span data-ttu-id="25f31-127">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="25f31-127">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="25f31-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-128">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="25f31-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="25f31-129">Property</span></span>|<span data-ttu-id="25f31-130">Тип</span><span class="sxs-lookup"><span data-stu-id="25f31-130">Type</span></span>|<span data-ttu-id="25f31-131">Описание</span><span class="sxs-lookup"><span data-stu-id="25f31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25f31-132">id</span><span class="sxs-lookup"><span data-stu-id="25f31-132">id</span></span>|<span data-ttu-id="25f31-133">String</span><span class="sxs-lookup"><span data-stu-id="25f31-133">String</span></span>|<span data-ttu-id="25f31-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="25f31-134">Key of the entity.</span></span> <span data-ttu-id="25f31-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25f31-136">lastModifiedDateTime</span></span>|<span data-ttu-id="25f31-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25f31-137">DateTimeOffset</span></span>|<span data-ttu-id="25f31-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="25f31-138">DateTime the object was last modified.</span></span> <span data-ttu-id="25f31-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25f31-140">createdDateTime</span></span>|<span data-ttu-id="25f31-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25f31-141">DateTimeOffset</span></span>|<span data-ttu-id="25f31-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="25f31-142">DateTime the object was created.</span></span> <span data-ttu-id="25f31-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-144">description</span><span class="sxs-lookup"><span data-stu-id="25f31-144">description</span></span>|<span data-ttu-id="25f31-145">String</span><span class="sxs-lookup"><span data-stu-id="25f31-145">String</span></span>|<span data-ttu-id="25f31-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25f31-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="25f31-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-148">displayName</span><span class="sxs-lookup"><span data-stu-id="25f31-148">displayName</span></span>|<span data-ttu-id="25f31-149">Строка</span><span class="sxs-lookup"><span data-stu-id="25f31-149">String</span></span>|<span data-ttu-id="25f31-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25f31-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="25f31-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="25f31-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-152">version</span><span class="sxs-lookup"><span data-stu-id="25f31-152">version</span></span>|<span data-ttu-id="25f31-153">Int32</span><span class="sxs-lookup"><span data-stu-id="25f31-153">Int32</span></span>|<span data-ttu-id="25f31-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="25f31-154">Version of the device configuration.</span></span> <span data-ttu-id="25f31-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="25f31-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="25f31-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="25f31-156">omaSettings</span></span>|<span data-ttu-id="25f31-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="25f31-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="25f31-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="25f31-158">OMA settings.</span></span> <span data-ttu-id="25f31-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="25f31-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="25f31-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="25f31-160">Response</span></span>
<span data-ttu-id="25f31-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="25f31-161">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25f31-162">Пример</span><span class="sxs-lookup"><span data-stu-id="25f31-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="25f31-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="25f31-163">Request</span></span>
<span data-ttu-id="25f31-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="25f31-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25f31-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="25f31-165">Response</span></span>
<span data-ttu-id="25f31-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="25f31-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




