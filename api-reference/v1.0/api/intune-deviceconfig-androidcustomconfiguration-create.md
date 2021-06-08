---
title: Создание объекта androidCustomConfiguration
description: Создание объекта androidCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5de44371b295c520d33ea6c8ae04925055bd2ab0
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759312"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="eea1b-103">Создание объекта androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="eea1b-103">Create androidCustomConfiguration</span></span>

<span data-ttu-id="eea1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eea1b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eea1b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eea1b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eea1b-106">Создание объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-106">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eea1b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="eea1b-107">Prerequisites</span></span>
<span data-ttu-id="eea1b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eea1b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea1b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eea1b-110">Permission type</span></span>|<span data-ttu-id="eea1b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eea1b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eea1b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eea1b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eea1b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea1b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eea1b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eea1b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea1b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eea1b-115">Not supported.</span></span>|
|<span data-ttu-id="eea1b-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="eea1b-116">Application</span></span>|<span data-ttu-id="eea1b-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eea1b-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eea1b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eea1b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eea1b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="eea1b-119">Request headers</span></span>
|<span data-ttu-id="eea1b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eea1b-120">Header</span></span>|<span data-ttu-id="eea1b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="eea1b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eea1b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eea1b-122">Authorization</span></span>|<span data-ttu-id="eea1b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eea1b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eea1b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="eea1b-124">Accept</span></span>|<span data-ttu-id="eea1b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eea1b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea1b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="eea1b-126">Request body</span></span>
<span data-ttu-id="eea1b-127">В тексте запроса добавьте представление объекта androidCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eea1b-127">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="eea1b-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="eea1b-128">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="eea1b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="eea1b-129">Property</span></span>|<span data-ttu-id="eea1b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="eea1b-130">Type</span></span>|<span data-ttu-id="eea1b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="eea1b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eea1b-132">id</span><span class="sxs-lookup"><span data-stu-id="eea1b-132">id</span></span>|<span data-ttu-id="eea1b-133">String</span><span class="sxs-lookup"><span data-stu-id="eea1b-133">String</span></span>|<span data-ttu-id="eea1b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="eea1b-134">Key of the entity.</span></span> <span data-ttu-id="eea1b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eea1b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eea1b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea1b-137">DateTimeOffset</span></span>|<span data-ttu-id="eea1b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="eea1b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="eea1b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eea1b-140">createdDateTime</span></span>|<span data-ttu-id="eea1b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eea1b-141">DateTimeOffset</span></span>|<span data-ttu-id="eea1b-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="eea1b-142">DateTime the object was created.</span></span> <span data-ttu-id="eea1b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-144">description</span><span class="sxs-lookup"><span data-stu-id="eea1b-144">description</span></span>|<span data-ttu-id="eea1b-145">String</span><span class="sxs-lookup"><span data-stu-id="eea1b-145">String</span></span>|<span data-ttu-id="eea1b-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eea1b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eea1b-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="eea1b-148">displayName</span></span>|<span data-ttu-id="eea1b-149">String</span><span class="sxs-lookup"><span data-stu-id="eea1b-149">String</span></span>|<span data-ttu-id="eea1b-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eea1b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eea1b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-152">version</span><span class="sxs-lookup"><span data-stu-id="eea1b-152">version</span></span>|<span data-ttu-id="eea1b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="eea1b-153">Int32</span></span>|<span data-ttu-id="eea1b-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="eea1b-154">Version of the device configuration.</span></span> <span data-ttu-id="eea1b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eea1b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eea1b-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="eea1b-156">omaSettings</span></span>|<span data-ttu-id="eea1b-157">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="eea1b-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="eea1b-158">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="eea1b-158">OMA settings.</span></span> <span data-ttu-id="eea1b-159">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="eea1b-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="eea1b-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea1b-160">Response</span></span>
<span data-ttu-id="eea1b-161">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="eea1b-161">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eea1b-162">Пример</span><span class="sxs-lookup"><span data-stu-id="eea1b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="eea1b-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="eea1b-163">Request</span></span>
<span data-ttu-id="eea1b-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eea1b-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 376

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="eea1b-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="eea1b-165">Response</span></span>
<span data-ttu-id="eea1b-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="eea1b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 548

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```




