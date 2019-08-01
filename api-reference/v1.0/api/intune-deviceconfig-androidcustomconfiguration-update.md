---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e82caa438c0c6a3813468f2d5ff5f097587a9672
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019655"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="19fba-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="19fba-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="19fba-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="19fba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fba-105">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19fba-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="19fba-106">Prerequisites</span></span>
<span data-ttu-id="19fba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19fba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19fba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="19fba-109">Permission type</span></span>|<span data-ttu-id="19fba-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="19fba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19fba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="19fba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19fba-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fba-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19fba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="19fba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19fba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fba-114">Not supported.</span></span>|
|<span data-ttu-id="19fba-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="19fba-115">Application</span></span>|<span data-ttu-id="19fba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19fba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fba-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="19fba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="19fba-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="19fba-118">Request headers</span></span>
|<span data-ttu-id="19fba-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="19fba-119">Header</span></span>|<span data-ttu-id="19fba-120">Значение</span><span class="sxs-lookup"><span data-stu-id="19fba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19fba-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="19fba-121">Authorization</span></span>|<span data-ttu-id="19fba-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="19fba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19fba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="19fba-123">Accept</span></span>|<span data-ttu-id="19fba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="19fba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fba-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="19fba-125">Request body</span></span>
<span data-ttu-id="19fba-126">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19fba-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="19fba-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="19fba-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="19fba-128">Property</span></span>|<span data-ttu-id="19fba-129">Тип</span><span class="sxs-lookup"><span data-stu-id="19fba-129">Type</span></span>|<span data-ttu-id="19fba-130">Описание</span><span class="sxs-lookup"><span data-stu-id="19fba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fba-131">id</span><span class="sxs-lookup"><span data-stu-id="19fba-131">id</span></span>|<span data-ttu-id="19fba-132">String</span><span class="sxs-lookup"><span data-stu-id="19fba-132">String</span></span>|<span data-ttu-id="19fba-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19fba-133">Key of the entity.</span></span> <span data-ttu-id="19fba-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19fba-135">lastModifiedDateTime</span></span>|<span data-ttu-id="19fba-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fba-136">DateTimeOffset</span></span>|<span data-ttu-id="19fba-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="19fba-137">DateTime the object was last modified.</span></span> <span data-ttu-id="19fba-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19fba-139">createdDateTime</span></span>|<span data-ttu-id="19fba-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fba-140">DateTimeOffset</span></span>|<span data-ttu-id="19fba-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="19fba-141">DateTime the object was created.</span></span> <span data-ttu-id="19fba-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-143">description</span><span class="sxs-lookup"><span data-stu-id="19fba-143">description</span></span>|<span data-ttu-id="19fba-144">String</span><span class="sxs-lookup"><span data-stu-id="19fba-144">String</span></span>|<span data-ttu-id="19fba-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19fba-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19fba-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-147">displayName</span><span class="sxs-lookup"><span data-stu-id="19fba-147">displayName</span></span>|<span data-ttu-id="19fba-148">Строка</span><span class="sxs-lookup"><span data-stu-id="19fba-148">String</span></span>|<span data-ttu-id="19fba-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19fba-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19fba-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19fba-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-151">version</span><span class="sxs-lookup"><span data-stu-id="19fba-151">version</span></span>|<span data-ttu-id="19fba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="19fba-152">Int32</span></span>|<span data-ttu-id="19fba-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="19fba-153">Version of the device configuration.</span></span> <span data-ttu-id="19fba-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="19fba-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19fba-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="19fba-155">omaSettings</span></span>|<span data-ttu-id="19fba-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="19fba-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="19fba-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="19fba-157">OMA settings.</span></span> <span data-ttu-id="19fba-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="19fba-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="19fba-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="19fba-159">Response</span></span>
<span data-ttu-id="19fba-160">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="19fba-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fba-161">Пример</span><span class="sxs-lookup"><span data-stu-id="19fba-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fba-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="19fba-162">Request</span></span>
<span data-ttu-id="19fba-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="19fba-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19fba-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="19fba-164">Response</span></span>
<span data-ttu-id="19fba-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="19fba-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



