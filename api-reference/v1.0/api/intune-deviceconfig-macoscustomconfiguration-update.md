---
title: Обновление объекта macOSCustomConfiguration
description: Обновление свойств объекта macOSCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 3d27b4e0821317e719dc9a7bbdae41c95721678f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314359"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="a08d3-103">Обновление объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a08d3-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="a08d3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a08d3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a08d3-105">Обновление свойств объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a08d3-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a08d3-106">Prerequisites</span></span>
<span data-ttu-id="a08d3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a08d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08d3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a08d3-109">Permission type</span></span>|<span data-ttu-id="a08d3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a08d3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a08d3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a08d3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a08d3-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08d3-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a08d3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a08d3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a08d3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a08d3-114">Not supported.</span></span>|
|<span data-ttu-id="a08d3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a08d3-115">Application</span></span>|<span data-ttu-id="a08d3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a08d3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a08d3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a08d3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a08d3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a08d3-118">Request headers</span></span>
|<span data-ttu-id="a08d3-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a08d3-119">Header</span></span>|<span data-ttu-id="a08d3-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a08d3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a08d3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a08d3-121">Authorization</span></span>|<span data-ttu-id="a08d3-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a08d3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a08d3-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a08d3-123">Accept</span></span>|<span data-ttu-id="a08d3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a08d3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a08d3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a08d3-125">Request body</span></span>
<span data-ttu-id="a08d3-126">В теле запроса добавьте представление объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a08d3-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="a08d3-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="a08d3-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a08d3-128">Property</span></span>|<span data-ttu-id="a08d3-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a08d3-129">Type</span></span>|<span data-ttu-id="a08d3-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a08d3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a08d3-131">id</span><span class="sxs-lookup"><span data-stu-id="a08d3-131">id</span></span>|<span data-ttu-id="a08d3-132">Строка</span><span class="sxs-lookup"><span data-stu-id="a08d3-132">String</span></span>|<span data-ttu-id="a08d3-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a08d3-133">Key of the entity.</span></span> <span data-ttu-id="a08d3-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a08d3-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a08d3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a08d3-136">DateTimeOffset</span></span>|<span data-ttu-id="a08d3-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="a08d3-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a08d3-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a08d3-139">createdDateTime</span></span>|<span data-ttu-id="a08d3-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a08d3-140">DateTimeOffset</span></span>|<span data-ttu-id="a08d3-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="a08d3-141">DateTime the object was created.</span></span> <span data-ttu-id="a08d3-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-143">описание</span><span class="sxs-lookup"><span data-stu-id="a08d3-143">description</span></span>|<span data-ttu-id="a08d3-144">Строка</span><span class="sxs-lookup"><span data-stu-id="a08d3-144">String</span></span>|<span data-ttu-id="a08d3-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a08d3-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a08d3-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a08d3-147">displayName</span></span>|<span data-ttu-id="a08d3-148">Строка</span><span class="sxs-lookup"><span data-stu-id="a08d3-148">String</span></span>|<span data-ttu-id="a08d3-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a08d3-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a08d3-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-151">version</span><span class="sxs-lookup"><span data-stu-id="a08d3-151">version</span></span>|<span data-ttu-id="a08d3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a08d3-152">Int32</span></span>|<span data-ttu-id="a08d3-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="a08d3-153">Version of the device configuration.</span></span> <span data-ttu-id="a08d3-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a08d3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a08d3-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="a08d3-155">payloadName</span></span>|<span data-ttu-id="a08d3-156">String</span><span class="sxs-lookup"><span data-stu-id="a08d3-156">String</span></span>|<span data-ttu-id="a08d3-157">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="a08d3-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a08d3-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a08d3-158">payloadFileName</span></span>|<span data-ttu-id="a08d3-159">String</span><span class="sxs-lookup"><span data-stu-id="a08d3-159">String</span></span>|<span data-ttu-id="a08d3-160">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a08d3-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a08d3-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="a08d3-161">\*.xml).</span></span>|
|<span data-ttu-id="a08d3-162">payload</span><span class="sxs-lookup"><span data-stu-id="a08d3-162">payload</span></span>|<span data-ttu-id="a08d3-163">Binary</span><span class="sxs-lookup"><span data-stu-id="a08d3-163">Binary</span></span>|<span data-ttu-id="a08d3-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="a08d3-164">Payload.</span></span> <span data-ttu-id="a08d3-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="a08d3-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a08d3-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="a08d3-166">Response</span></span>
<span data-ttu-id="a08d3-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a08d3-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a08d3-168">Пример</span><span class="sxs-lookup"><span data-stu-id="a08d3-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="a08d3-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="a08d3-169">Request</span></span>
<span data-ttu-id="a08d3-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a08d3-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="a08d3-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="a08d3-171">Response</span></span>
<span data-ttu-id="a08d3-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a08d3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



