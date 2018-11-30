---
title: Обновление объекта iosCustomConfiguration
description: Обновление свойств объекта iosCustomConfiguration.
ms.openlocfilehash: 6151c93e83bd35db70d6c5428d55bde92e8027de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026481"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="6bea1-103">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6bea1-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="6bea1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bea1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bea1-105">Обновление свойств объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-105">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bea1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6bea1-106">Prerequisites</span></span>
<span data-ttu-id="6bea1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bea1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bea1-109">Permission type</span></span>|<span data-ttu-id="6bea1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bea1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bea1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bea1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6bea1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bea1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6bea1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bea1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bea1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bea1-114">Not supported.</span></span>|
|<span data-ttu-id="6bea1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bea1-115">Application</span></span>|<span data-ttu-id="6bea1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bea1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bea1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bea1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6bea1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bea1-118">Request headers</span></span>
|<span data-ttu-id="6bea1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bea1-119">Header</span></span>|<span data-ttu-id="6bea1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6bea1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bea1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bea1-121">Authorization</span></span>|<span data-ttu-id="6bea1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6bea1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bea1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6bea1-123">Accept</span></span>|<span data-ttu-id="6bea1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6bea1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bea1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bea1-125">Request body</span></span>
<span data-ttu-id="6bea1-126">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bea1-126">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="6bea1-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-127">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="6bea1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bea1-128">Property</span></span>|<span data-ttu-id="6bea1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6bea1-129">Type</span></span>|<span data-ttu-id="6bea1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6bea1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bea1-131">id</span><span class="sxs-lookup"><span data-stu-id="6bea1-131">id</span></span>|<span data-ttu-id="6bea1-132">String</span><span class="sxs-lookup"><span data-stu-id="6bea1-132">String</span></span>|<span data-ttu-id="6bea1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6bea1-133">Key of the entity.</span></span> <span data-ttu-id="6bea1-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6bea1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6bea1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bea1-136">DateTimeOffset</span></span>|<span data-ttu-id="6bea1-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="6bea1-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6bea1-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6bea1-139">createdDateTime</span></span>|<span data-ttu-id="6bea1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bea1-140">DateTimeOffset</span></span>|<span data-ttu-id="6bea1-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="6bea1-141">DateTime the object was created.</span></span> <span data-ttu-id="6bea1-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-143">описание</span><span class="sxs-lookup"><span data-stu-id="6bea1-143">description</span></span>|<span data-ttu-id="6bea1-144">String</span><span class="sxs-lookup"><span data-stu-id="6bea1-144">String</span></span>|<span data-ttu-id="6bea1-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6bea1-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6bea1-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6bea1-147">displayName</span></span>|<span data-ttu-id="6bea1-148">String</span><span class="sxs-lookup"><span data-stu-id="6bea1-148">String</span></span>|<span data-ttu-id="6bea1-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6bea1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6bea1-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-151">version</span><span class="sxs-lookup"><span data-stu-id="6bea1-151">version</span></span>|<span data-ttu-id="6bea1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6bea1-152">Int32</span></span>|<span data-ttu-id="6bea1-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="6bea1-153">Version of the device configuration.</span></span> <span data-ttu-id="6bea1-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6bea1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6bea1-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="6bea1-155">payloadName</span></span>|<span data-ttu-id="6bea1-156">String</span><span class="sxs-lookup"><span data-stu-id="6bea1-156">String</span></span>|<span data-ttu-id="6bea1-157">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="6bea1-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="6bea1-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="6bea1-158">payloadFileName</span></span>|<span data-ttu-id="6bea1-159">String</span><span class="sxs-lookup"><span data-stu-id="6bea1-159">String</span></span>|<span data-ttu-id="6bea1-160">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="6bea1-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="6bea1-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="6bea1-161">\*.xml).</span></span>|
|<span data-ttu-id="6bea1-162">payload</span><span class="sxs-lookup"><span data-stu-id="6bea1-162">payload</span></span>|<span data-ttu-id="6bea1-163">Binary</span><span class="sxs-lookup"><span data-stu-id="6bea1-163">Binary</span></span>|<span data-ttu-id="6bea1-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="6bea1-164">Payload.</span></span> <span data-ttu-id="6bea1-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="6bea1-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="6bea1-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bea1-166">Response</span></span>
<span data-ttu-id="6bea1-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6bea1-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bea1-168">Пример</span><span class="sxs-lookup"><span data-stu-id="6bea1-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="6bea1-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bea1-169">Request</span></span>
<span data-ttu-id="6bea1-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bea1-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="6bea1-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bea1-171">Response</span></span>
<span data-ttu-id="6bea1-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6bea1-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
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



