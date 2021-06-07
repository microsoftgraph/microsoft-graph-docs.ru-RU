---
title: Обновление объекта windowsPhone81CustomConfiguration
description: Обновление свойств объекта windowsPhone81CustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ac366f9593ea294fabc1f35513ac61944026447d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756178"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="d8253-103">Обновление объекта windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d8253-103">Update windowsPhone81CustomConfiguration</span></span>

<span data-ttu-id="d8253-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8253-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8253-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d8253-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8253-106">Обновление свойств объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8253-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="d8253-107">Prerequisites</span></span>
<span data-ttu-id="d8253-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8253-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8253-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8253-110">Permission type</span></span>|<span data-ttu-id="d8253-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8253-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8253-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8253-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8253-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8253-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8253-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8253-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8253-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8253-115">Not supported.</span></span>|
|<span data-ttu-id="d8253-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d8253-116">Application</span></span>|<span data-ttu-id="d8253-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8253-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8253-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8253-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d8253-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d8253-119">Request headers</span></span>
|<span data-ttu-id="d8253-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8253-120">Header</span></span>|<span data-ttu-id="d8253-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d8253-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8253-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8253-122">Authorization</span></span>|<span data-ttu-id="d8253-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8253-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8253-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8253-124">Accept</span></span>|<span data-ttu-id="d8253-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8253-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8253-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8253-126">Request body</span></span>
<span data-ttu-id="d8253-127">В теле запроса добавьте представление объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8253-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="d8253-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="d8253-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8253-129">Property</span></span>|<span data-ttu-id="d8253-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d8253-130">Type</span></span>|<span data-ttu-id="d8253-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d8253-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8253-132">id</span><span class="sxs-lookup"><span data-stu-id="d8253-132">id</span></span>|<span data-ttu-id="d8253-133">String</span><span class="sxs-lookup"><span data-stu-id="d8253-133">String</span></span>|<span data-ttu-id="d8253-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d8253-134">Key of the entity.</span></span> <span data-ttu-id="d8253-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8253-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d8253-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8253-137">DateTimeOffset</span></span>|<span data-ttu-id="d8253-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="d8253-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d8253-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8253-140">createdDateTime</span></span>|<span data-ttu-id="d8253-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8253-141">DateTimeOffset</span></span>|<span data-ttu-id="d8253-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="d8253-142">DateTime the object was created.</span></span> <span data-ttu-id="d8253-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-144">description</span><span class="sxs-lookup"><span data-stu-id="d8253-144">description</span></span>|<span data-ttu-id="d8253-145">String</span><span class="sxs-lookup"><span data-stu-id="d8253-145">String</span></span>|<span data-ttu-id="d8253-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8253-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d8253-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d8253-148">displayName</span></span>|<span data-ttu-id="d8253-149">String</span><span class="sxs-lookup"><span data-stu-id="d8253-149">String</span></span>|<span data-ttu-id="d8253-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8253-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d8253-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-152">version</span><span class="sxs-lookup"><span data-stu-id="d8253-152">version</span></span>|<span data-ttu-id="d8253-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d8253-153">Int32</span></span>|<span data-ttu-id="d8253-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="d8253-154">Version of the device configuration.</span></span> <span data-ttu-id="d8253-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d8253-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d8253-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d8253-156">omaSettings</span></span>|<span data-ttu-id="d8253-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8253-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="d8253-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="d8253-158">OMA settings.</span></span> <span data-ttu-id="d8253-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="d8253-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d8253-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8253-160">Response</span></span>
<span data-ttu-id="d8253-161">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d8253-161">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8253-162">Пример</span><span class="sxs-lookup"><span data-stu-id="d8253-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8253-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8253-163">Request</span></span>
<span data-ttu-id="d8253-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8253-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 383

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d8253-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8253-165">Response</span></span>
<span data-ttu-id="d8253-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8253-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 555

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```




