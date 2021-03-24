---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 277affa12d91ca51165e40324c74c2649801b3a9
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146456"
---
# <a name="update-detectedapp"></a><span data-ttu-id="ad865-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="ad865-103">Update detectedApp</span></span>

<span data-ttu-id="ad865-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad865-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad865-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad865-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad865-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad865-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad865-107">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad865-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad865-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad865-108">Prerequisites</span></span>
<span data-ttu-id="ad865-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad865-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad865-111">Permission type</span></span>|<span data-ttu-id="ad865-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad865-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad865-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad865-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad865-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad865-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ad865-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad865-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad865-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad865-116">Not supported.</span></span>|
|<span data-ttu-id="ad865-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad865-117">Application</span></span>|<span data-ttu-id="ad865-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad865-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad865-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad865-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ad865-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad865-120">Request headers</span></span>
|<span data-ttu-id="ad865-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad865-121">Header</span></span>|<span data-ttu-id="ad865-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad865-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad865-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad865-123">Authorization</span></span>|<span data-ttu-id="ad865-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad865-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad865-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad865-125">Accept</span></span>|<span data-ttu-id="ad865-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad865-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad865-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad865-127">Request body</span></span>
<span data-ttu-id="ad865-128">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad865-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="ad865-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="ad865-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="ad865-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad865-130">Property</span></span>|<span data-ttu-id="ad865-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad865-131">Type</span></span>|<span data-ttu-id="ad865-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad865-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad865-133">id</span><span class="sxs-lookup"><span data-stu-id="ad865-133">id</span></span>|<span data-ttu-id="ad865-134">Строка</span><span class="sxs-lookup"><span data-stu-id="ad865-134">String</span></span>|<span data-ttu-id="ad865-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="ad865-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="ad865-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="ad865-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="ad865-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ad865-137">Read-only.</span></span>|
|<span data-ttu-id="ad865-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ad865-138">displayName</span></span>|<span data-ttu-id="ad865-139">Строка</span><span class="sxs-lookup"><span data-stu-id="ad865-139">String</span></span>|<span data-ttu-id="ad865-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="ad865-140">Name of the discovered application.</span></span> <span data-ttu-id="ad865-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ad865-141">Read-only</span></span>|
|<span data-ttu-id="ad865-142">version</span><span class="sxs-lookup"><span data-stu-id="ad865-142">version</span></span>|<span data-ttu-id="ad865-143">String</span><span class="sxs-lookup"><span data-stu-id="ad865-143">String</span></span>|<span data-ttu-id="ad865-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="ad865-144">Version of the discovered application.</span></span> <span data-ttu-id="ad865-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ad865-145">Read-only</span></span>|
|<span data-ttu-id="ad865-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="ad865-146">sizeInByte</span></span>|<span data-ttu-id="ad865-147">Int64</span><span class="sxs-lookup"><span data-stu-id="ad865-147">Int64</span></span>|<span data-ttu-id="ad865-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="ad865-148">Discovered application size in bytes.</span></span> <span data-ttu-id="ad865-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="ad865-149">Read-only</span></span>|
|<span data-ttu-id="ad865-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ad865-150">deviceCount</span></span>|<span data-ttu-id="ad865-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ad865-151">Int32</span></span>|<span data-ttu-id="ad865-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="ad865-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="ad865-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad865-153">Response</span></span>
<span data-ttu-id="ad865-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ad865-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad865-155">Пример</span><span class="sxs-lookup"><span data-stu-id="ad865-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad865-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad865-156">Request</span></span>
<span data-ttu-id="ad865-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad865-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ad865-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad865-158">Response</span></span>
<span data-ttu-id="ad865-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad865-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




