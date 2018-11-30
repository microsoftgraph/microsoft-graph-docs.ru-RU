---
title: Создание объекта macOSDeviceFeaturesConfiguration
description: Создание объекта macOSDeviceFeaturesConfiguration.
ms.openlocfilehash: e8d6d16ce66e512d44cbae63ec41122b526ac471
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024476"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="937ce-103">Создание объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="937ce-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="937ce-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="937ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="937ce-105">Создание объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="937ce-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="937ce-106">Prerequisites</span></span>
<span data-ttu-id="937ce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="937ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="937ce-109">Permission type</span></span>|<span data-ttu-id="937ce-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="937ce-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="937ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="937ce-111">Delegated (work or school account)</span></span>|<span data-ttu-id="937ce-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937ce-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="937ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="937ce-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="937ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937ce-114">Not supported.</span></span>|
|<span data-ttu-id="937ce-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="937ce-115">Application</span></span>|<span data-ttu-id="937ce-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="937ce-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="937ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="937ce-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="937ce-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="937ce-118">Request headers</span></span>
|<span data-ttu-id="937ce-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="937ce-119">Header</span></span>|<span data-ttu-id="937ce-120">Значение</span><span class="sxs-lookup"><span data-stu-id="937ce-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="937ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="937ce-121">Authorization</span></span>|<span data-ttu-id="937ce-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="937ce-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="937ce-123">Accept</span><span class="sxs-lookup"><span data-stu-id="937ce-123">Accept</span></span>|<span data-ttu-id="937ce-124">application/json</span><span class="sxs-lookup"><span data-stu-id="937ce-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="937ce-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="937ce-125">Request body</span></span>
<span data-ttu-id="937ce-126">В теле запроса добавьте представление объекта macOSDeviceFeaturesConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="937ce-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="937ce-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSDeviceFeaturesConfiguration.</span><span class="sxs-lookup"><span data-stu-id="937ce-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="937ce-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="937ce-128">Property</span></span>|<span data-ttu-id="937ce-129">Тип</span><span class="sxs-lookup"><span data-stu-id="937ce-129">Type</span></span>|<span data-ttu-id="937ce-130">Описание</span><span class="sxs-lookup"><span data-stu-id="937ce-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="937ce-131">id</span><span class="sxs-lookup"><span data-stu-id="937ce-131">id</span></span>|<span data-ttu-id="937ce-132">String</span><span class="sxs-lookup"><span data-stu-id="937ce-132">String</span></span>|<span data-ttu-id="937ce-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="937ce-133">Key of the entity.</span></span> <span data-ttu-id="937ce-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="937ce-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="937ce-135">lastModifiedDateTime</span></span>|<span data-ttu-id="937ce-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="937ce-136">DateTimeOffset</span></span>|<span data-ttu-id="937ce-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="937ce-137">DateTime the object was last modified.</span></span> <span data-ttu-id="937ce-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="937ce-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="937ce-139">createdDateTime</span></span>|<span data-ttu-id="937ce-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="937ce-140">DateTimeOffset</span></span>|<span data-ttu-id="937ce-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="937ce-141">DateTime the object was created.</span></span> <span data-ttu-id="937ce-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="937ce-143">описание</span><span class="sxs-lookup"><span data-stu-id="937ce-143">description</span></span>|<span data-ttu-id="937ce-144">String</span><span class="sxs-lookup"><span data-stu-id="937ce-144">String</span></span>|<span data-ttu-id="937ce-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="937ce-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="937ce-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="937ce-147">displayName</span><span class="sxs-lookup"><span data-stu-id="937ce-147">displayName</span></span>|<span data-ttu-id="937ce-148">String</span><span class="sxs-lookup"><span data-stu-id="937ce-148">String</span></span>|<span data-ttu-id="937ce-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="937ce-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="937ce-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="937ce-151">version</span><span class="sxs-lookup"><span data-stu-id="937ce-151">version</span></span>|<span data-ttu-id="937ce-152">Int32</span><span class="sxs-lookup"><span data-stu-id="937ce-152">Int32</span></span>|<span data-ttu-id="937ce-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="937ce-153">Version of the device configuration.</span></span> <span data-ttu-id="937ce-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="937ce-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="937ce-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="937ce-155">Response</span></span>
<span data-ttu-id="937ce-156">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="937ce-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="937ce-157">Пример</span><span class="sxs-lookup"><span data-stu-id="937ce-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="937ce-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="937ce-158">Request</span></span>
<span data-ttu-id="937ce-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="937ce-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="937ce-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="937ce-160">Response</span></span>
<span data-ttu-id="937ce-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="937ce-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



