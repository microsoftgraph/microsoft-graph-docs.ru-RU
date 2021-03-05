---
title: Обновление объекта iosCustomConfiguration
description: Обновление свойств объекта iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9440c5924afa742256687396ff70b3ef3d91f0db
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471679"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="9966b-103">Обновление объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="9966b-103">Update iosCustomConfiguration</span></span>

<span data-ttu-id="9966b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9966b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9966b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9966b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9966b-106">Обновление свойств объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-106">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9966b-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9966b-107">Prerequisites</span></span>
<span data-ttu-id="9966b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9966b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9966b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9966b-110">Permission type</span></span>|<span data-ttu-id="9966b-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9966b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9966b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9966b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9966b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9966b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9966b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9966b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9966b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9966b-115">Not supported.</span></span>|
|<span data-ttu-id="9966b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9966b-116">Application</span></span>|<span data-ttu-id="9966b-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9966b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9966b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9966b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9966b-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9966b-119">Request headers</span></span>
|<span data-ttu-id="9966b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9966b-120">Header</span></span>|<span data-ttu-id="9966b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9966b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9966b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9966b-122">Authorization</span></span>|<span data-ttu-id="9966b-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9966b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9966b-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9966b-124">Accept</span></span>|<span data-ttu-id="9966b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9966b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9966b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9966b-126">Request body</span></span>
<span data-ttu-id="9966b-127">В теле запроса добавьте представление объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9966b-127">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="9966b-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-128">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="9966b-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9966b-129">Property</span></span>|<span data-ttu-id="9966b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9966b-130">Type</span></span>|<span data-ttu-id="9966b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9966b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9966b-132">id</span><span class="sxs-lookup"><span data-stu-id="9966b-132">id</span></span>|<span data-ttu-id="9966b-133">String</span><span class="sxs-lookup"><span data-stu-id="9966b-133">String</span></span>|<span data-ttu-id="9966b-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9966b-134">Key of the entity.</span></span> <span data-ttu-id="9966b-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9966b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9966b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9966b-137">DateTimeOffset</span></span>|<span data-ttu-id="9966b-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="9966b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9966b-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9966b-140">createdDateTime</span></span>|<span data-ttu-id="9966b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9966b-141">DateTimeOffset</span></span>|<span data-ttu-id="9966b-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="9966b-142">DateTime the object was created.</span></span> <span data-ttu-id="9966b-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-144">description</span><span class="sxs-lookup"><span data-stu-id="9966b-144">description</span></span>|<span data-ttu-id="9966b-145">String</span><span class="sxs-lookup"><span data-stu-id="9966b-145">String</span></span>|<span data-ttu-id="9966b-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9966b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9966b-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="9966b-148">displayName</span></span>|<span data-ttu-id="9966b-149">String</span><span class="sxs-lookup"><span data-stu-id="9966b-149">String</span></span>|<span data-ttu-id="9966b-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9966b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9966b-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-152">version</span><span class="sxs-lookup"><span data-stu-id="9966b-152">version</span></span>|<span data-ttu-id="9966b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9966b-153">Int32</span></span>|<span data-ttu-id="9966b-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9966b-154">Version of the device configuration.</span></span> <span data-ttu-id="9966b-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9966b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9966b-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="9966b-156">payloadName</span></span>|<span data-ttu-id="9966b-157">String</span><span class="sxs-lookup"><span data-stu-id="9966b-157">String</span></span>|<span data-ttu-id="9966b-158">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="9966b-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="9966b-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="9966b-159">payloadFileName</span></span>|<span data-ttu-id="9966b-160">String</span><span class="sxs-lookup"><span data-stu-id="9966b-160">String</span></span>|<span data-ttu-id="9966b-161">Имя файла полезной нагрузки (\*.mobileconfig \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="9966b-161">Payload file name (\*.mobileconfig \| \*.xml).</span></span>|
|<span data-ttu-id="9966b-162">payload</span><span class="sxs-lookup"><span data-stu-id="9966b-162">payload</span></span>|<span data-ttu-id="9966b-163">Binary</span><span class="sxs-lookup"><span data-stu-id="9966b-163">Binary</span></span>|<span data-ttu-id="9966b-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="9966b-164">Payload.</span></span> <span data-ttu-id="9966b-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="9966b-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="9966b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="9966b-166">Response</span></span>
<span data-ttu-id="9966b-167">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9966b-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9966b-168">Пример</span><span class="sxs-lookup"><span data-stu-id="9966b-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="9966b-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="9966b-169">Request</span></span>
<span data-ttu-id="9966b-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9966b-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9966b-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="9966b-171">Response</span></span>
<span data-ttu-id="9966b-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9966b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









