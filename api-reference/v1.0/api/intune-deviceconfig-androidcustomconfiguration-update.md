---
title: Update androidCustomConfiguration
description: Обновление свойств объекта androidCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1993068e374a6719cfdaff0ea76ec6fcf4bc1a46
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264213"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="21733-103">Update androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="21733-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="21733-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21733-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21733-105">Обновление свойств объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21733-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="21733-106">Prerequisites</span></span>
<span data-ttu-id="21733-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="21733-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="21733-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="21733-109">Permission type</span></span>|<span data-ttu-id="21733-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="21733-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21733-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="21733-111">Delegated (work or school account)</span></span>|<span data-ttu-id="21733-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21733-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21733-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="21733-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21733-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21733-114">Not supported.</span></span>|
|<span data-ttu-id="21733-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="21733-115">Application</span></span>|<span data-ttu-id="21733-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21733-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21733-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="21733-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="21733-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="21733-118">Request headers</span></span>
|<span data-ttu-id="21733-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="21733-119">Header</span></span>|<span data-ttu-id="21733-120">Значение</span><span class="sxs-lookup"><span data-stu-id="21733-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21733-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="21733-121">Authorization</span></span>|<span data-ttu-id="21733-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="21733-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21733-123">Accept</span><span class="sxs-lookup"><span data-stu-id="21733-123">Accept</span></span>|<span data-ttu-id="21733-124">application/json</span><span class="sxs-lookup"><span data-stu-id="21733-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21733-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="21733-125">Request body</span></span>
<span data-ttu-id="21733-126">В теле запроса добавьте представление объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21733-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="21733-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="21733-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="21733-128">Property</span></span>|<span data-ttu-id="21733-129">Тип</span><span class="sxs-lookup"><span data-stu-id="21733-129">Type</span></span>|<span data-ttu-id="21733-130">Описание</span><span class="sxs-lookup"><span data-stu-id="21733-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21733-131">id</span><span class="sxs-lookup"><span data-stu-id="21733-131">id</span></span>|<span data-ttu-id="21733-132">String</span><span class="sxs-lookup"><span data-stu-id="21733-132">String</span></span>|<span data-ttu-id="21733-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="21733-133">Key of the entity.</span></span> <span data-ttu-id="21733-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21733-135">lastModifiedDateTime</span></span>|<span data-ttu-id="21733-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21733-136">DateTimeOffset</span></span>|<span data-ttu-id="21733-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="21733-137">DateTime the object was last modified.</span></span> <span data-ttu-id="21733-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21733-139">createdDateTime</span></span>|<span data-ttu-id="21733-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21733-140">DateTimeOffset</span></span>|<span data-ttu-id="21733-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="21733-141">DateTime the object was created.</span></span> <span data-ttu-id="21733-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-143">description</span><span class="sxs-lookup"><span data-stu-id="21733-143">description</span></span>|<span data-ttu-id="21733-144">String</span><span class="sxs-lookup"><span data-stu-id="21733-144">String</span></span>|<span data-ttu-id="21733-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21733-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="21733-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-147">displayName</span><span class="sxs-lookup"><span data-stu-id="21733-147">displayName</span></span>|<span data-ttu-id="21733-148">String</span><span class="sxs-lookup"><span data-stu-id="21733-148">String</span></span>|<span data-ttu-id="21733-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21733-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="21733-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="21733-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-151">version</span><span class="sxs-lookup"><span data-stu-id="21733-151">version</span></span>|<span data-ttu-id="21733-152">Int32</span><span class="sxs-lookup"><span data-stu-id="21733-152">Int32</span></span>|<span data-ttu-id="21733-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="21733-153">Version of the device configuration.</span></span> <span data-ttu-id="21733-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21733-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="21733-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="21733-155">omaSettings</span></span>|<span data-ttu-id="21733-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="21733-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="21733-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="21733-157">OMA settings.</span></span> <span data-ttu-id="21733-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="21733-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="21733-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="21733-159">Response</span></span>
<span data-ttu-id="21733-160">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="21733-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21733-161">Пример</span><span class="sxs-lookup"><span data-stu-id="21733-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="21733-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="21733-162">Request</span></span>
<span data-ttu-id="21733-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="21733-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="21733-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="21733-164">Response</span></span>
<span data-ttu-id="21733-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="21733-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



