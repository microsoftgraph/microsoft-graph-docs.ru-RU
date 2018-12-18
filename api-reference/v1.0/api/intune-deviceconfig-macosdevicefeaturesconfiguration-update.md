---
title: Обновление объекта macOSDeviceFeaturesConfiguration
description: Обновление свойств объекта macOSDeviceFeaturesConfiguration.
author: tfitzmac
ms.openlocfilehash: aecefa3e348613fa2aa0f9974f2aafbce56c8051
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348456"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="625d7-103">Обновление объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="625d7-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="625d7-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="625d7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="625d7-105">Обновление свойств объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="625d7-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="625d7-106">Prerequisites</span></span>
<span data-ttu-id="625d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="625d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="625d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="625d7-109">Permission type</span></span>|<span data-ttu-id="625d7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="625d7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="625d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="625d7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="625d7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625d7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="625d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="625d7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="625d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="625d7-114">Not supported.</span></span>|
|<span data-ttu-id="625d7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="625d7-115">Application</span></span>|<span data-ttu-id="625d7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="625d7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="625d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="625d7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="625d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="625d7-118">Request headers</span></span>
|<span data-ttu-id="625d7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="625d7-119">Header</span></span>|<span data-ttu-id="625d7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="625d7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="625d7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="625d7-121">Authorization</span></span>|<span data-ttu-id="625d7-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="625d7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="625d7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="625d7-123">Accept</span></span>|<span data-ttu-id="625d7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="625d7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="625d7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="625d7-125">Request body</span></span>
<span data-ttu-id="625d7-126">В теле запроса добавьте представление объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="625d7-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="625d7-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="625d7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="625d7-128">Property</span></span>|<span data-ttu-id="625d7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="625d7-129">Type</span></span>|<span data-ttu-id="625d7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="625d7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="625d7-131">id</span><span class="sxs-lookup"><span data-stu-id="625d7-131">id</span></span>|<span data-ttu-id="625d7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="625d7-132">String</span></span>|<span data-ttu-id="625d7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="625d7-133">Key of the entity.</span></span> <span data-ttu-id="625d7-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="625d7-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="625d7-135">lastModifiedDateTime</span></span>|<span data-ttu-id="625d7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="625d7-136">DateTimeOffset</span></span>|<span data-ttu-id="625d7-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="625d7-137">DateTime the object was last modified.</span></span> <span data-ttu-id="625d7-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="625d7-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="625d7-139">createdDateTime</span></span>|<span data-ttu-id="625d7-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="625d7-140">DateTimeOffset</span></span>|<span data-ttu-id="625d7-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="625d7-141">DateTime the object was created.</span></span> <span data-ttu-id="625d7-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="625d7-143">описание</span><span class="sxs-lookup"><span data-stu-id="625d7-143">description</span></span>|<span data-ttu-id="625d7-144">Строка</span><span class="sxs-lookup"><span data-stu-id="625d7-144">String</span></span>|<span data-ttu-id="625d7-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="625d7-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="625d7-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="625d7-147">displayName</span><span class="sxs-lookup"><span data-stu-id="625d7-147">displayName</span></span>|<span data-ttu-id="625d7-148">Строка</span><span class="sxs-lookup"><span data-stu-id="625d7-148">String</span></span>|<span data-ttu-id="625d7-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="625d7-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="625d7-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="625d7-151">version</span><span class="sxs-lookup"><span data-stu-id="625d7-151">version</span></span>|<span data-ttu-id="625d7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="625d7-152">Int32</span></span>|<span data-ttu-id="625d7-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="625d7-153">Version of the device configuration.</span></span> <span data-ttu-id="625d7-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="625d7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="625d7-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="625d7-155">Response</span></span>
<span data-ttu-id="625d7-156">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="625d7-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="625d7-157">Пример</span><span class="sxs-lookup"><span data-stu-id="625d7-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="625d7-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="625d7-158">Request</span></span>
<span data-ttu-id="625d7-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="625d7-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="625d7-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="625d7-160">Response</span></span>
<span data-ttu-id="625d7-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="625d7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```



