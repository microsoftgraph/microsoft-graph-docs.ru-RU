---
title: Создание объекта macOSCustomConfiguration
description: Создание объекта macOSCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ff6c3782c9633e67f470121c825bf9a63db050c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576110"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="3de95-103">Создание объекта macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3de95-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="3de95-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3de95-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3de95-105">Создание объекта [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3de95-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3de95-106">Prerequisites</span></span>
<span data-ttu-id="3de95-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3de95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3de95-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3de95-109">Permission type</span></span>|<span data-ttu-id="3de95-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3de95-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3de95-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3de95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3de95-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3de95-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3de95-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3de95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3de95-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de95-114">Not supported.</span></span>|
|<span data-ttu-id="3de95-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3de95-115">Application</span></span>|<span data-ttu-id="3de95-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3de95-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3de95-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3de95-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3de95-118">Request headers</span></span>
|<span data-ttu-id="3de95-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3de95-119">Header</span></span>|<span data-ttu-id="3de95-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3de95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3de95-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3de95-121">Authorization</span></span>|<span data-ttu-id="3de95-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3de95-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3de95-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3de95-123">Accept</span></span>|<span data-ttu-id="3de95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3de95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3de95-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3de95-125">Request body</span></span>
<span data-ttu-id="3de95-126">В теле запроса добавьте представление объекта macOSCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de95-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="3de95-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта macOSCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="3de95-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="3de95-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de95-128">Property</span></span>|<span data-ttu-id="3de95-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3de95-129">Type</span></span>|<span data-ttu-id="3de95-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3de95-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3de95-131">id</span><span class="sxs-lookup"><span data-stu-id="3de95-131">id</span></span>|<span data-ttu-id="3de95-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3de95-132">String</span></span>|<span data-ttu-id="3de95-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3de95-133">Key of the entity.</span></span> <span data-ttu-id="3de95-134">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3de95-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3de95-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de95-136">DateTimeOffset</span></span>|<span data-ttu-id="3de95-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="3de95-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3de95-138">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3de95-139">createdDateTime</span></span>|<span data-ttu-id="3de95-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3de95-140">DateTimeOffset</span></span>|<span data-ttu-id="3de95-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="3de95-141">DateTime the object was created.</span></span> <span data-ttu-id="3de95-142">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-143">description</span><span class="sxs-lookup"><span data-stu-id="3de95-143">description</span></span>|<span data-ttu-id="3de95-144">String</span><span class="sxs-lookup"><span data-stu-id="3de95-144">String</span></span>|<span data-ttu-id="3de95-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de95-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3de95-146">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3de95-147">displayName</span></span>|<span data-ttu-id="3de95-148">Строка</span><span class="sxs-lookup"><span data-stu-id="3de95-148">String</span></span>|<span data-ttu-id="3de95-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de95-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3de95-150">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3de95-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-151">version</span><span class="sxs-lookup"><span data-stu-id="3de95-151">version</span></span>|<span data-ttu-id="3de95-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3de95-152">Int32</span></span>|<span data-ttu-id="3de95-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="3de95-153">Version of the device configuration.</span></span> <span data-ttu-id="3de95-154">Наследуется от объекта [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3de95-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3de95-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="3de95-155">payloadName</span></span>|<span data-ttu-id="3de95-156">String</span><span class="sxs-lookup"><span data-stu-id="3de95-156">String</span></span>|<span data-ttu-id="3de95-157">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="3de95-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="3de95-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="3de95-158">payloadFileName</span></span>|<span data-ttu-id="3de95-159">String</span><span class="sxs-lookup"><span data-stu-id="3de95-159">String</span></span>|<span data-ttu-id="3de95-160">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="3de95-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="3de95-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="3de95-161">\*.xml).</span></span>|
|<span data-ttu-id="3de95-162">payload</span><span class="sxs-lookup"><span data-stu-id="3de95-162">payload</span></span>|<span data-ttu-id="3de95-163">Binary</span><span class="sxs-lookup"><span data-stu-id="3de95-163">Binary</span></span>|<span data-ttu-id="3de95-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="3de95-164">Payload.</span></span> <span data-ttu-id="3de95-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="3de95-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="3de95-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de95-166">Response</span></span>
<span data-ttu-id="3de95-167">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3de95-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3de95-168">Пример</span><span class="sxs-lookup"><span data-stu-id="3de95-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="3de95-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="3de95-169">Request</span></span>
<span data-ttu-id="3de95-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3de95-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="3de95-171">Отклик</span><span class="sxs-lookup"><span data-stu-id="3de95-171">Response</span></span>
<span data-ttu-id="3de95-p109">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3de95-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



