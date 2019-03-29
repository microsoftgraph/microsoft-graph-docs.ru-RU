---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01a6738e4fcd9e86c965ff3d33aac0b9f07918e8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962836"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="34a91-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="34a91-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="34a91-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34a91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a91-105">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34a91-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="34a91-106">Prerequisites</span></span>
<span data-ttu-id="34a91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34a91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34a91-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34a91-109">Permission type</span></span>|<span data-ttu-id="34a91-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="34a91-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34a91-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34a91-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34a91-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34a91-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34a91-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34a91-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34a91-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a91-114">Not supported.</span></span>|
|<span data-ttu-id="34a91-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34a91-115">Application</span></span>|<span data-ttu-id="34a91-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34a91-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34a91-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34a91-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="34a91-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34a91-118">Request headers</span></span>
|<span data-ttu-id="34a91-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34a91-119">Header</span></span>|<span data-ttu-id="34a91-120">Значение</span><span class="sxs-lookup"><span data-stu-id="34a91-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34a91-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34a91-121">Authorization</span></span>|<span data-ttu-id="34a91-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34a91-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34a91-123">Accept</span><span class="sxs-lookup"><span data-stu-id="34a91-123">Accept</span></span>|<span data-ttu-id="34a91-124">application/json</span><span class="sxs-lookup"><span data-stu-id="34a91-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34a91-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="34a91-125">Request body</span></span>
<span data-ttu-id="34a91-126">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34a91-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="34a91-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="34a91-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="34a91-128">Property</span></span>|<span data-ttu-id="34a91-129">Тип</span><span class="sxs-lookup"><span data-stu-id="34a91-129">Type</span></span>|<span data-ttu-id="34a91-130">Описание</span><span class="sxs-lookup"><span data-stu-id="34a91-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a91-131">id</span><span class="sxs-lookup"><span data-stu-id="34a91-131">id</span></span>|<span data-ttu-id="34a91-132">Строка</span><span class="sxs-lookup"><span data-stu-id="34a91-132">String</span></span>|<span data-ttu-id="34a91-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="34a91-133">Key of the entity.</span></span> <span data-ttu-id="34a91-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34a91-135">lastModifiedDateTime</span></span>|<span data-ttu-id="34a91-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a91-136">DateTimeOffset</span></span>|<span data-ttu-id="34a91-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="34a91-137">DateTime the object was last modified.</span></span> <span data-ttu-id="34a91-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34a91-139">createdDateTime</span></span>|<span data-ttu-id="34a91-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a91-140">DateTimeOffset</span></span>|<span data-ttu-id="34a91-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="34a91-141">DateTime the object was created.</span></span> <span data-ttu-id="34a91-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-143">description</span><span class="sxs-lookup"><span data-stu-id="34a91-143">description</span></span>|<span data-ttu-id="34a91-144">String</span><span class="sxs-lookup"><span data-stu-id="34a91-144">String</span></span>|<span data-ttu-id="34a91-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a91-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34a91-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-147">displayName</span><span class="sxs-lookup"><span data-stu-id="34a91-147">displayName</span></span>|<span data-ttu-id="34a91-148">String</span><span class="sxs-lookup"><span data-stu-id="34a91-148">String</span></span>|<span data-ttu-id="34a91-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a91-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34a91-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34a91-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-151">version</span><span class="sxs-lookup"><span data-stu-id="34a91-151">version</span></span>|<span data-ttu-id="34a91-152">Int32</span><span class="sxs-lookup"><span data-stu-id="34a91-152">Int32</span></span>|<span data-ttu-id="34a91-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="34a91-153">Version of the device configuration.</span></span> <span data-ttu-id="34a91-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="34a91-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34a91-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="34a91-155">omaSettings</span></span>|<span data-ttu-id="34a91-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="34a91-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="34a91-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="34a91-157">OMA settings.</span></span> <span data-ttu-id="34a91-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="34a91-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="34a91-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="34a91-159">Response</span></span>
<span data-ttu-id="34a91-160">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="34a91-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34a91-161">Пример</span><span class="sxs-lookup"><span data-stu-id="34a91-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="34a91-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="34a91-162">Request</span></span>
<span data-ttu-id="34a91-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34a91-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34a91-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="34a91-164">Response</span></span>
<span data-ttu-id="34a91-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34a91-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



