---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5bfaf7cacc04efbbdaee97cecf9f550a2cfe5f22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469792"
---
# <a name="update-detectedapp"></a><span data-ttu-id="44852-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="44852-103">Update detectedApp</span></span>

<span data-ttu-id="44852-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44852-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44852-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44852-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44852-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44852-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44852-107">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="44852-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44852-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="44852-108">Prerequisites</span></span>
<span data-ttu-id="44852-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44852-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44852-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="44852-111">Permission type</span></span>|<span data-ttu-id="44852-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="44852-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44852-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="44852-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44852-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44852-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44852-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="44852-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44852-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44852-116">Not supported.</span></span>|
|<span data-ttu-id="44852-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="44852-117">Application</span></span>|<span data-ttu-id="44852-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44852-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44852-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="44852-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="44852-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="44852-120">Request headers</span></span>
|<span data-ttu-id="44852-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="44852-121">Header</span></span>|<span data-ttu-id="44852-122">Значение</span><span class="sxs-lookup"><span data-stu-id="44852-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44852-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44852-123">Authorization</span></span>|<span data-ttu-id="44852-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="44852-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44852-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44852-125">Accept</span></span>|<span data-ttu-id="44852-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44852-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44852-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="44852-127">Request body</span></span>
<span data-ttu-id="44852-128">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44852-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="44852-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="44852-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="44852-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="44852-130">Property</span></span>|<span data-ttu-id="44852-131">Тип</span><span class="sxs-lookup"><span data-stu-id="44852-131">Type</span></span>|<span data-ttu-id="44852-132">Описание</span><span class="sxs-lookup"><span data-stu-id="44852-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44852-133">id</span><span class="sxs-lookup"><span data-stu-id="44852-133">id</span></span>|<span data-ttu-id="44852-134">String</span><span class="sxs-lookup"><span data-stu-id="44852-134">String</span></span>|<span data-ttu-id="44852-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="44852-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="44852-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="44852-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="44852-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="44852-137">Read-only.</span></span>|
|<span data-ttu-id="44852-138">displayName</span><span class="sxs-lookup"><span data-stu-id="44852-138">displayName</span></span>|<span data-ttu-id="44852-139">Строка</span><span class="sxs-lookup"><span data-stu-id="44852-139">String</span></span>|<span data-ttu-id="44852-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="44852-140">Name of the discovered application.</span></span> <span data-ttu-id="44852-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="44852-141">Read-only</span></span>|
|<span data-ttu-id="44852-142">version</span><span class="sxs-lookup"><span data-stu-id="44852-142">version</span></span>|<span data-ttu-id="44852-143">String</span><span class="sxs-lookup"><span data-stu-id="44852-143">String</span></span>|<span data-ttu-id="44852-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="44852-144">Version of the discovered application.</span></span> <span data-ttu-id="44852-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="44852-145">Read-only</span></span>|
|<span data-ttu-id="44852-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="44852-146">sizeInByte</span></span>|<span data-ttu-id="44852-147">Int64</span><span class="sxs-lookup"><span data-stu-id="44852-147">Int64</span></span>|<span data-ttu-id="44852-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="44852-148">Discovered application size in bytes.</span></span> <span data-ttu-id="44852-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="44852-149">Read-only</span></span>|
|<span data-ttu-id="44852-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="44852-150">deviceCount</span></span>|<span data-ttu-id="44852-151">Int32</span><span class="sxs-lookup"><span data-stu-id="44852-151">Int32</span></span>|<span data-ttu-id="44852-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="44852-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="44852-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="44852-153">Response</span></span>
<span data-ttu-id="44852-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="44852-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44852-155">Пример</span><span class="sxs-lookup"><span data-stu-id="44852-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="44852-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="44852-156">Request</span></span>
<span data-ttu-id="44852-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="44852-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="44852-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="44852-158">Response</span></span>
<span data-ttu-id="44852-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="44852-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```





