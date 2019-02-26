---
title: Создание объекта iosCustomConfiguration
description: Создание объекта iosCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecdc9ca4fb9218ae77c1c144feeb4ca2cb5c389d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261616"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="2eb53-103">Создание объекта iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb53-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="2eb53-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2eb53-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb53-105">Создание объекта [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-105">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb53-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2eb53-106">Prerequisites</span></span>
<span data-ttu-id="2eb53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2eb53-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2eb53-109">Permission type</span></span>|<span data-ttu-id="2eb53-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2eb53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb53-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2eb53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb53-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb53-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb53-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2eb53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb53-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb53-114">Not supported.</span></span>|
|<span data-ttu-id="2eb53-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2eb53-115">Application</span></span>|<span data-ttu-id="2eb53-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2eb53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb53-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2eb53-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2eb53-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2eb53-118">Request headers</span></span>
|<span data-ttu-id="2eb53-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2eb53-119">Header</span></span>|<span data-ttu-id="2eb53-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2eb53-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eb53-121">Authorization</span></span>|<span data-ttu-id="2eb53-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2eb53-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb53-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2eb53-123">Accept</span></span>|<span data-ttu-id="2eb53-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb53-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb53-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2eb53-125">Request body</span></span>
<span data-ttu-id="2eb53-126">В теле запроса добавьте представление объекта iosCustomConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2eb53-126">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="2eb53-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2eb53-127">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="2eb53-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="2eb53-128">Property</span></span>|<span data-ttu-id="2eb53-129">Тип</span><span class="sxs-lookup"><span data-stu-id="2eb53-129">Type</span></span>|<span data-ttu-id="2eb53-130">Описание</span><span class="sxs-lookup"><span data-stu-id="2eb53-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2eb53-131">id</span><span class="sxs-lookup"><span data-stu-id="2eb53-131">id</span></span>|<span data-ttu-id="2eb53-132">String</span><span class="sxs-lookup"><span data-stu-id="2eb53-132">String</span></span>|<span data-ttu-id="2eb53-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb53-133">Key of the entity.</span></span> <span data-ttu-id="2eb53-134">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb53-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2eb53-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb53-136">DateTimeOffset</span></span>|<span data-ttu-id="2eb53-137">Дата и время последнего изменения объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb53-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2eb53-138">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2eb53-139">createdDateTime</span></span>|<span data-ttu-id="2eb53-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2eb53-140">DateTimeOffset</span></span>|<span data-ttu-id="2eb53-141">Дата и время создания объекта.</span><span class="sxs-lookup"><span data-stu-id="2eb53-141">DateTime the object was created.</span></span> <span data-ttu-id="2eb53-142">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-143">description</span><span class="sxs-lookup"><span data-stu-id="2eb53-143">description</span></span>|<span data-ttu-id="2eb53-144">Строка</span><span class="sxs-lookup"><span data-stu-id="2eb53-144">String</span></span>|<span data-ttu-id="2eb53-145">Указанное администратором описание конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb53-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2eb53-146">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2eb53-147">displayName</span></span>|<span data-ttu-id="2eb53-148">Строка</span><span class="sxs-lookup"><span data-stu-id="2eb53-148">String</span></span>|<span data-ttu-id="2eb53-149">Указанное администратором имя конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb53-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2eb53-150">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2eb53-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-151">version</span><span class="sxs-lookup"><span data-stu-id="2eb53-151">version</span></span>|<span data-ttu-id="2eb53-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2eb53-152">Int32</span></span>|<span data-ttu-id="2eb53-153">Версия конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="2eb53-153">Version of the device configuration.</span></span> <span data-ttu-id="2eb53-154">Наследуется от [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="2eb53-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2eb53-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="2eb53-155">payloadName</span></span>|<span data-ttu-id="2eb53-156">String</span><span class="sxs-lookup"><span data-stu-id="2eb53-156">String</span></span>|<span data-ttu-id="2eb53-157">Имя, которое видит пользователь.</span><span class="sxs-lookup"><span data-stu-id="2eb53-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="2eb53-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="2eb53-158">payloadFileName</span></span>|<span data-ttu-id="2eb53-159">String</span><span class="sxs-lookup"><span data-stu-id="2eb53-159">String</span></span>|<span data-ttu-id="2eb53-160">Имя файла полезных данных (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="2eb53-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="2eb53-161">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="2eb53-161">\*.xml).</span></span>|
|<span data-ttu-id="2eb53-162">payload</span><span class="sxs-lookup"><span data-stu-id="2eb53-162">payload</span></span>|<span data-ttu-id="2eb53-163">Binary</span><span class="sxs-lookup"><span data-stu-id="2eb53-163">Binary</span></span>|<span data-ttu-id="2eb53-164">Полезные данные</span><span class="sxs-lookup"><span data-stu-id="2eb53-164">Payload.</span></span> <span data-ttu-id="2eb53-165">(массив байтов в кодировке UTF8).</span><span class="sxs-lookup"><span data-stu-id="2eb53-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="2eb53-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="2eb53-166">Response</span></span>
<span data-ttu-id="2eb53-167">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2eb53-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eb53-168">Пример</span><span class="sxs-lookup"><span data-stu-id="2eb53-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb53-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="2eb53-169">Request</span></span>
<span data-ttu-id="2eb53-170">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2eb53-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2eb53-171">Ответ</span><span class="sxs-lookup"><span data-stu-id="2eb53-171">Response</span></span>
<span data-ttu-id="2eb53-p109">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2eb53-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



