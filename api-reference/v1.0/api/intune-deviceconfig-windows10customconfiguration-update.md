---
title: Обновление объекта windows10CustomConfiguration
description: Обновление свойств объекта windows10CustomConfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e4067e25b8a97fbc57a5168c16ded515e9a6092e
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365567"
---
# <a name="update-windows10customconfiguration"></a><span data-ttu-id="38cd6-103">Обновление объекта windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="38cd6-103">Update windows10CustomConfiguration</span></span>

> <span data-ttu-id="38cd6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="38cd6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38cd6-105">Обновление свойств объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-105">Update the properties of a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38cd6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="38cd6-106">Prerequisites</span></span>
<span data-ttu-id="38cd6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38cd6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38cd6-109">Permission type</span></span>|<span data-ttu-id="38cd6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38cd6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38cd6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38cd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="38cd6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38cd6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38cd6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38cd6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38cd6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38cd6-114">Not supported.</span></span>|
|<span data-ttu-id="38cd6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38cd6-115">Application</span></span>|<span data-ttu-id="38cd6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38cd6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38cd6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38cd6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38cd6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38cd6-118">Request headers</span></span>
|<span data-ttu-id="38cd6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38cd6-119">Header</span></span>|<span data-ttu-id="38cd6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="38cd6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38cd6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38cd6-121">Authorization</span></span>|<span data-ttu-id="38cd6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38cd6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38cd6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="38cd6-123">Accept</span></span>|<span data-ttu-id="38cd6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="38cd6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38cd6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="38cd6-125">Request body</span></span>
<span data-ttu-id="38cd6-126">В теле запроса добавьте представление объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38cd6-126">In the request body, supply a JSON representation for the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

<span data-ttu-id="38cd6-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-127">The following table shows the properties that are required when you create the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span></span>

|<span data-ttu-id="38cd6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="38cd6-128">Property</span></span>|<span data-ttu-id="38cd6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="38cd6-129">Type</span></span>|<span data-ttu-id="38cd6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="38cd6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38cd6-131">id</span><span class="sxs-lookup"><span data-stu-id="38cd6-131">id</span></span>|<span data-ttu-id="38cd6-132">String</span><span class="sxs-lookup"><span data-stu-id="38cd6-132">String</span></span>|<span data-ttu-id="38cd6-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="38cd6-133">Key of the entity.</span></span> <span data-ttu-id="38cd6-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38cd6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="38cd6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38cd6-136">DateTimeOffset</span></span>|<span data-ttu-id="38cd6-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="38cd6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="38cd6-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38cd6-139">createdDateTime</span></span>|<span data-ttu-id="38cd6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38cd6-140">DateTimeOffset</span></span>|<span data-ttu-id="38cd6-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="38cd6-141">DateTime the object was created.</span></span> <span data-ttu-id="38cd6-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-143">description</span><span class="sxs-lookup"><span data-stu-id="38cd6-143">description</span></span>|<span data-ttu-id="38cd6-144">String</span><span class="sxs-lookup"><span data-stu-id="38cd6-144">String</span></span>|<span data-ttu-id="38cd6-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38cd6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38cd6-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="38cd6-147">displayName</span></span>|<span data-ttu-id="38cd6-148">Строка</span><span class="sxs-lookup"><span data-stu-id="38cd6-148">String</span></span>|<span data-ttu-id="38cd6-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38cd6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38cd6-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38cd6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-151">version</span><span class="sxs-lookup"><span data-stu-id="38cd6-151">version</span></span>|<span data-ttu-id="38cd6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="38cd6-152">Int32</span></span>|<span data-ttu-id="38cd6-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="38cd6-153">Version of the device configuration.</span></span> <span data-ttu-id="38cd6-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38cd6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38cd6-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="38cd6-155">omaSettings</span></span>|<span data-ttu-id="38cd6-156">Коллекция [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38cd6-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="38cd6-157">Параметры OMA.</span><span class="sxs-lookup"><span data-stu-id="38cd6-157">OMA settings.</span></span> <span data-ttu-id="38cd6-158">Эта коллекция может содержать не более 1000 элементов.</span><span class="sxs-lookup"><span data-stu-id="38cd6-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="38cd6-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="38cd6-159">Response</span></span>
<span data-ttu-id="38cd6-160">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="38cd6-160">If successful, this method returns a `200 OK` response code and an updated [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38cd6-161">Пример</span><span class="sxs-lookup"><span data-stu-id="38cd6-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="38cd6-162">Запрос</span><span class="sxs-lookup"><span data-stu-id="38cd6-162">Request</span></span>
<span data-ttu-id="38cd6-163">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38cd6-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="38cd6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="38cd6-164">Response</span></span>
<span data-ttu-id="38cd6-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38cd6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




