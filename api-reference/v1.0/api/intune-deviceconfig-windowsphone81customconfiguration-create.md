---
title: Создание объекта windowsPhone81CustomConfiguration
description: Создание объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 767ee7303de1ba67ab9d4fc512f5e9933dad6c27
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43399299"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="1f75e-103">Создание объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f75e-103">Create windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="1f75e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f75e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f75e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f75e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f75e-106">Создание объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-106">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1f75e-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1f75e-107">Prerequisites</span></span>
<span data-ttu-id="1f75e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f75e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f75e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1f75e-110">Permission type</span></span>|<span data-ttu-id="1f75e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1f75e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f75e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1f75e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1f75e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f75e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1f75e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1f75e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f75e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f75e-115">Not supported.</span></span>|
|<span data-ttu-id="1f75e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1f75e-116">Application</span></span>|<span data-ttu-id="1f75e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1f75e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f75e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1f75e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f75e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="1f75e-119">Request headers</span></span>
|<span data-ttu-id="1f75e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1f75e-120">Header</span></span>|<span data-ttu-id="1f75e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1f75e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f75e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f75e-122">Authorization</span></span>|<span data-ttu-id="1f75e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1f75e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f75e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1f75e-124">Accept</span></span>|<span data-ttu-id="1f75e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1f75e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f75e-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1f75e-126">Request body</span></span>
<span data-ttu-id="1f75e-127">В теле запроса добавьте представление объекта windowsPhone81CustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f75e-127">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="1f75e-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsPhone81CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1f75e-128">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="1f75e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f75e-129">Property</span></span>|<span data-ttu-id="1f75e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1f75e-130">Type</span></span>|<span data-ttu-id="1f75e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1f75e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f75e-132">id</span><span class="sxs-lookup"><span data-stu-id="1f75e-132">id</span></span>|<span data-ttu-id="1f75e-133">String</span><span class="sxs-lookup"><span data-stu-id="1f75e-133">String</span></span>|<span data-ttu-id="1f75e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1f75e-134">Key of the entity.</span></span> <span data-ttu-id="1f75e-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1f75e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1f75e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f75e-137">DateTimeOffset</span></span>|<span data-ttu-id="1f75e-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="1f75e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1f75e-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1f75e-140">createdDateTime</span></span>|<span data-ttu-id="1f75e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f75e-141">DateTimeOffset</span></span>|<span data-ttu-id="1f75e-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="1f75e-142">DateTime the object was created.</span></span> <span data-ttu-id="1f75e-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-144">description</span><span class="sxs-lookup"><span data-stu-id="1f75e-144">description</span></span>|<span data-ttu-id="1f75e-145">String</span><span class="sxs-lookup"><span data-stu-id="1f75e-145">String</span></span>|<span data-ttu-id="1f75e-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f75e-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1f75e-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-148">displayName</span><span class="sxs-lookup"><span data-stu-id="1f75e-148">displayName</span></span>|<span data-ttu-id="1f75e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="1f75e-149">String</span></span>|<span data-ttu-id="1f75e-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f75e-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1f75e-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1f75e-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-152">version</span><span class="sxs-lookup"><span data-stu-id="1f75e-152">version</span></span>|<span data-ttu-id="1f75e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="1f75e-153">Int32</span></span>|<span data-ttu-id="1f75e-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="1f75e-154">Version of the device configuration.</span></span> <span data-ttu-id="1f75e-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1f75e-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1f75e-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1f75e-156">omaSettings</span></span>|<span data-ttu-id="1f75e-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="1f75e-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="1f75e-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="1f75e-158">OMA settings.</span></span> <span data-ttu-id="1f75e-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="1f75e-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1f75e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f75e-160">Response</span></span>
<span data-ttu-id="1f75e-161">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1f75e-161">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f75e-162">Пример</span><span class="sxs-lookup"><span data-stu-id="1f75e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="1f75e-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="1f75e-163">Request</span></span>
<span data-ttu-id="1f75e-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1f75e-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1f75e-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="1f75e-165">Response</span></span>
<span data-ttu-id="1f75e-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1f75e-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






