---
title: Создание объекта detectedApp
description: Создание объекта detectedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4316079f6d6eb4b20dfa636550c44bc759edecea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42513639"
---
# <a name="create-detectedapp"></a><span data-ttu-id="af023-103">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="af023-103">Create detectedApp</span></span>

<span data-ttu-id="af023-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af023-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="af023-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af023-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af023-106">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="af023-106">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af023-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af023-107">Prerequisites</span></span>
<span data-ttu-id="af023-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af023-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af023-110">Permission type</span></span>|<span data-ttu-id="af023-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af023-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af023-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af023-112">Delegated (work or school account)</span></span>|<span data-ttu-id="af023-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af023-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af023-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af023-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af023-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af023-115">Not supported.</span></span>|
|<span data-ttu-id="af023-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af023-116">Application</span></span>|<span data-ttu-id="af023-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af023-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af023-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af023-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="af023-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="af023-119">Request headers</span></span>
|<span data-ttu-id="af023-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af023-120">Header</span></span>|<span data-ttu-id="af023-121">Значение</span><span class="sxs-lookup"><span data-stu-id="af023-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af023-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="af023-122">Authorization</span></span>|<span data-ttu-id="af023-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af023-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af023-124">Accept</span><span class="sxs-lookup"><span data-stu-id="af023-124">Accept</span></span>|<span data-ttu-id="af023-125">application/json</span><span class="sxs-lookup"><span data-stu-id="af023-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af023-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="af023-126">Request body</span></span>
<span data-ttu-id="af023-127">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af023-127">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="af023-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="af023-128">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="af023-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="af023-129">Property</span></span>|<span data-ttu-id="af023-130">Тип</span><span class="sxs-lookup"><span data-stu-id="af023-130">Type</span></span>|<span data-ttu-id="af023-131">Описание</span><span class="sxs-lookup"><span data-stu-id="af023-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af023-132">id</span><span class="sxs-lookup"><span data-stu-id="af023-132">id</span></span>|<span data-ttu-id="af023-133">String</span><span class="sxs-lookup"><span data-stu-id="af023-133">String</span></span>|<span data-ttu-id="af023-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="af023-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="af023-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="af023-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="af023-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="af023-136">Read-only.</span></span>|
|<span data-ttu-id="af023-137">displayName</span><span class="sxs-lookup"><span data-stu-id="af023-137">displayName</span></span>|<span data-ttu-id="af023-138">Строка</span><span class="sxs-lookup"><span data-stu-id="af023-138">String</span></span>|<span data-ttu-id="af023-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="af023-139">Name of the discovered application.</span></span> <span data-ttu-id="af023-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="af023-140">Read-only</span></span>|
|<span data-ttu-id="af023-141">version</span><span class="sxs-lookup"><span data-stu-id="af023-141">version</span></span>|<span data-ttu-id="af023-142">String</span><span class="sxs-lookup"><span data-stu-id="af023-142">String</span></span>|<span data-ttu-id="af023-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="af023-143">Version of the discovered application.</span></span> <span data-ttu-id="af023-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="af023-144">Read-only</span></span>|
|<span data-ttu-id="af023-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="af023-145">sizeInByte</span></span>|<span data-ttu-id="af023-146">Int64</span><span class="sxs-lookup"><span data-stu-id="af023-146">Int64</span></span>|<span data-ttu-id="af023-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="af023-147">Discovered application size in bytes.</span></span> <span data-ttu-id="af023-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="af023-148">Read-only</span></span>|
|<span data-ttu-id="af023-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="af023-149">deviceCount</span></span>|<span data-ttu-id="af023-150">Int32</span><span class="sxs-lookup"><span data-stu-id="af023-150">Int32</span></span>|<span data-ttu-id="af023-151">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="af023-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="af023-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="af023-152">Response</span></span>
<span data-ttu-id="af023-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af023-153">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af023-154">Пример</span><span class="sxs-lookup"><span data-stu-id="af023-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="af023-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="af023-155">Request</span></span>
<span data-ttu-id="af023-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af023-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="af023-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="af023-157">Response</span></span>
<span data-ttu-id="af023-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="af023-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




