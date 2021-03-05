---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51ae9c2755a6de77950769f3bf7550025662b58a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473758"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="823ac-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="823ac-103">Create iosCustomConfiguration</span></span>

<span data-ttu-id="823ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="823ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="823ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="823ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="823ac-106">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-106">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="823ac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="823ac-107">Prerequisites</span></span>
<span data-ttu-id="823ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="823ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="823ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="823ac-110">Permission type</span></span>|<span data-ttu-id="823ac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="823ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="823ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="823ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="823ac-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823ac-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="823ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="823ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="823ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="823ac-115">Not supported.</span></span>|
|<span data-ttu-id="823ac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="823ac-116">Application</span></span>|<span data-ttu-id="823ac-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="823ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="823ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="823ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="823ac-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="823ac-119">Request headers</span></span>
|<span data-ttu-id="823ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="823ac-120">Header</span></span>|<span data-ttu-id="823ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="823ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="823ac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="823ac-122">Authorization</span></span>|<span data-ttu-id="823ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="823ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="823ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="823ac-124">Accept</span></span>|<span data-ttu-id="823ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="823ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="823ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="823ac-126">Request body</span></span>
<span data-ttu-id="823ac-127">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="823ac-127">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="823ac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="823ac-128">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="823ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="823ac-129">Property</span></span>|<span data-ttu-id="823ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="823ac-130">Type</span></span>|<span data-ttu-id="823ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="823ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="823ac-132">id</span><span class="sxs-lookup"><span data-stu-id="823ac-132">id</span></span>|<span data-ttu-id="823ac-133">String</span><span class="sxs-lookup"><span data-stu-id="823ac-133">String</span></span>|<span data-ttu-id="823ac-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="823ac-134">Key of the entity.</span></span> <span data-ttu-id="823ac-135">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="823ac-136">lastModifiedDateTime</span></span>|<span data-ttu-id="823ac-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823ac-137">DateTimeOffset</span></span>|<span data-ttu-id="823ac-138">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="823ac-138">DateTime the object was last modified.</span></span> <span data-ttu-id="823ac-139">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="823ac-140">createdDateTime</span></span>|<span data-ttu-id="823ac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823ac-141">DateTimeOffset</span></span>|<span data-ttu-id="823ac-142">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="823ac-142">DateTime the object was created.</span></span> <span data-ttu-id="823ac-143">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-144">description</span><span class="sxs-lookup"><span data-stu-id="823ac-144">description</span></span>|<span data-ttu-id="823ac-145">String</span><span class="sxs-lookup"><span data-stu-id="823ac-145">String</span></span>|<span data-ttu-id="823ac-146">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="823ac-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="823ac-147">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-148">displayName</span><span class="sxs-lookup"><span data-stu-id="823ac-148">displayName</span></span>|<span data-ttu-id="823ac-149">String</span><span class="sxs-lookup"><span data-stu-id="823ac-149">String</span></span>|<span data-ttu-id="823ac-150">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="823ac-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="823ac-151">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-152">version</span><span class="sxs-lookup"><span data-stu-id="823ac-152">version</span></span>|<span data-ttu-id="823ac-153">Int32</span><span class="sxs-lookup"><span data-stu-id="823ac-153">Int32</span></span>|<span data-ttu-id="823ac-154">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="823ac-154">Version of the device configuration.</span></span> <span data-ttu-id="823ac-155">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="823ac-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="823ac-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="823ac-156">payloadName</span></span>|<span data-ttu-id="823ac-157">String</span><span class="sxs-lookup"><span data-stu-id="823ac-157">String</span></span>|<span data-ttu-id="823ac-158">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="823ac-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="823ac-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="823ac-159">payloadFileName</span></span>|<span data-ttu-id="823ac-160">String</span><span class="sxs-lookup"><span data-stu-id="823ac-160">String</span></span>|<span data-ttu-id="823ac-161">Имя файла полезной нагрузки (\*.mobileconfig \| \*.xml).</span><span class="sxs-lookup"><span data-stu-id="823ac-161">Payload file name (\*.mobileconfig \| \*.xml).</span></span>|
|<span data-ttu-id="823ac-162">payload</span><span class="sxs-lookup"><span data-stu-id="823ac-162">payload</span></span>|<span data-ttu-id="823ac-163">Binary</span><span class="sxs-lookup"><span data-stu-id="823ac-163">Binary</span></span>|<span data-ttu-id="823ac-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="823ac-164">Payload.</span></span> <span data-ttu-id="823ac-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="823ac-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="823ac-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="823ac-166">Response</span></span>
<span data-ttu-id="823ac-167">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="823ac-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="823ac-168">Пример</span><span class="sxs-lookup"><span data-stu-id="823ac-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="823ac-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="823ac-169">Request</span></span>
<span data-ttu-id="823ac-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="823ac-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="823ac-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="823ac-171">Response</span></span>
<span data-ttu-id="823ac-p109">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="823ac-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









