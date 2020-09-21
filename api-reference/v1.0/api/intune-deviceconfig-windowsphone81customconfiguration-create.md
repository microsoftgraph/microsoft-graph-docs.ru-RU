---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9db05f97cb16b2190a289305ce360001e3b1c89d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968145"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="4b0b9-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b0b9-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="4b0b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b0b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b0b9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b0b9-106">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b0b9-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4b0b9-107">Prerequisites</span></span>
<span data-ttu-id="4b0b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0b9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4b0b9-110">Permission type</span></span>|<span data-ttu-id="4b0b9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4b0b9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b0b9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4b0b9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b0b9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b0b9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b0b9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4b0b9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b0b9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-115">Not supported.</span></span>|
|<span data-ttu-id="4b0b9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4b0b9-116">Application</span></span>|<span data-ttu-id="4b0b9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b0b9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4b0b9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b0b9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4b0b9-119">Request headers</span></span>
|<span data-ttu-id="4b0b9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4b0b9-120">Header</span></span>|<span data-ttu-id="4b0b9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4b0b9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b0b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b0b9-122">Authorization</span></span>|<span data-ttu-id="4b0b9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b0b9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4b0b9-124">Accept</span></span>|<span data-ttu-id="4b0b9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0b9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b0b9-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4b0b9-126">Request body</span></span>
<span data-ttu-id="4b0b9-127">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="4b0b9-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="4b0b9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b0b9-129">Property</span></span>|<span data-ttu-id="4b0b9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4b0b9-130">Type</span></span>|<span data-ttu-id="4b0b9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4b0b9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b0b9-132">id</span><span class="sxs-lookup"><span data-stu-id="4b0b9-132">id</span></span>|<span data-ttu-id="4b0b9-133">String</span><span class="sxs-lookup"><span data-stu-id="4b0b9-133">String</span></span>|<span data-ttu-id="4b0b9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-134">Key of the entity.</span></span> <span data-ttu-id="4b0b9-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b0b9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4b0b9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b0b9-137">DateTimeOffset</span></span>|<span data-ttu-id="4b0b9-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4b0b9-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b0b9-140">createdDateTime</span></span>|<span data-ttu-id="4b0b9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b0b9-141">DateTimeOffset</span></span>|<span data-ttu-id="4b0b9-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-142">DateTime the object was created.</span></span> <span data-ttu-id="4b0b9-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-144">description</span><span class="sxs-lookup"><span data-stu-id="4b0b9-144">description</span></span>|<span data-ttu-id="4b0b9-145">String</span><span class="sxs-lookup"><span data-stu-id="4b0b9-145">String</span></span>|<span data-ttu-id="4b0b9-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b0b9-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="4b0b9-148">displayName</span></span>|<span data-ttu-id="4b0b9-149">String</span><span class="sxs-lookup"><span data-stu-id="4b0b9-149">String</span></span>|<span data-ttu-id="4b0b9-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b0b9-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-152">version</span><span class="sxs-lookup"><span data-stu-id="4b0b9-152">version</span></span>|<span data-ttu-id="4b0b9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4b0b9-153">Int32</span></span>|<span data-ttu-id="4b0b9-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-154">Version of the device configuration.</span></span> <span data-ttu-id="4b0b9-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4b0b9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b0b9-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4b0b9-156">omaSettings</span></span>|<span data-ttu-id="4b0b9-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4b0b9-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4b0b9-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-158">OMA settings.</span></span> <span data-ttu-id="4b0b9-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4b0b9-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0b9-160">Response</span></span>
<span data-ttu-id="4b0b9-161">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-161">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0b9-162">Пример</span><span class="sxs-lookup"><span data-stu-id="4b0b9-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0b9-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="4b0b9-163">Request</span></span>
<span data-ttu-id="4b0b9-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4b0b9-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="4b0b9-165">Response</span></span>
<span data-ttu-id="4b0b9-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4b0b9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









