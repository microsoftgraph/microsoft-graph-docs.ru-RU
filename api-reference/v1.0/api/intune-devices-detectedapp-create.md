---
title: Создание объекта detectedApp
description: Создание объекта detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4542c9e675751cd20f2cd5739ae73b4110f97ef9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753771"
---
# <a name="create-detectedapp"></a><span data-ttu-id="4e5ac-103">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="4e5ac-103">Create detectedApp</span></span>

<span data-ttu-id="4e5ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e5ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4e5ac-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e5ac-106">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="4e5ac-106">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e5ac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4e5ac-107">Prerequisites</span></span>
<span data-ttu-id="4e5ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e5ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e5ac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4e5ac-110">Permission type</span></span>|<span data-ttu-id="4e5ac-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4e5ac-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e5ac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4e5ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e5ac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5ac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4e5ac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4e5ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e5ac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-115">Not supported.</span></span>|
|<span data-ttu-id="4e5ac-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4e5ac-116">Application</span></span>|<span data-ttu-id="4e5ac-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e5ac-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e5ac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4e5ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="4e5ac-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4e5ac-119">Request headers</span></span>
|<span data-ttu-id="4e5ac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4e5ac-120">Header</span></span>|<span data-ttu-id="4e5ac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4e5ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e5ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e5ac-122">Authorization</span></span>|<span data-ttu-id="4e5ac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e5ac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4e5ac-124">Accept</span></span>|<span data-ttu-id="4e5ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e5ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e5ac-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4e5ac-126">Request body</span></span>
<span data-ttu-id="4e5ac-127">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-127">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="4e5ac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-128">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="4e5ac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e5ac-129">Property</span></span>|<span data-ttu-id="4e5ac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4e5ac-130">Type</span></span>|<span data-ttu-id="4e5ac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4e5ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e5ac-132">id</span><span class="sxs-lookup"><span data-stu-id="4e5ac-132">id</span></span>|<span data-ttu-id="4e5ac-133">String</span><span class="sxs-lookup"><span data-stu-id="4e5ac-133">String</span></span>|<span data-ttu-id="4e5ac-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="4e5ac-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="4e5ac-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-136">Read-only.</span></span>|
|<span data-ttu-id="4e5ac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4e5ac-137">displayName</span></span>|<span data-ttu-id="4e5ac-138">String</span><span class="sxs-lookup"><span data-stu-id="4e5ac-138">String</span></span>|<span data-ttu-id="4e5ac-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-139">Name of the discovered application.</span></span> <span data-ttu-id="4e5ac-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4e5ac-140">Read-only</span></span>|
|<span data-ttu-id="4e5ac-141">version</span><span class="sxs-lookup"><span data-stu-id="4e5ac-141">version</span></span>|<span data-ttu-id="4e5ac-142">String</span><span class="sxs-lookup"><span data-stu-id="4e5ac-142">String</span></span>|<span data-ttu-id="4e5ac-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-143">Version of the discovered application.</span></span> <span data-ttu-id="4e5ac-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4e5ac-144">Read-only</span></span>|
|<span data-ttu-id="4e5ac-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="4e5ac-145">sizeInByte</span></span>|<span data-ttu-id="4e5ac-146">Int64</span><span class="sxs-lookup"><span data-stu-id="4e5ac-146">Int64</span></span>|<span data-ttu-id="4e5ac-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-147">Discovered application size in bytes.</span></span> <span data-ttu-id="4e5ac-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4e5ac-148">Read-only</span></span>|
|<span data-ttu-id="4e5ac-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4e5ac-149">deviceCount</span></span>|<span data-ttu-id="4e5ac-150">Int32</span><span class="sxs-lookup"><span data-stu-id="4e5ac-150">Int32</span></span>|<span data-ttu-id="4e5ac-151">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="4e5ac-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e5ac-152">Response</span></span>
<span data-ttu-id="4e5ac-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-153">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e5ac-154">Пример</span><span class="sxs-lookup"><span data-stu-id="4e5ac-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e5ac-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="4e5ac-155">Request</span></span>
<span data-ttu-id="4e5ac-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e5ac-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="4e5ac-157">Response</span></span>
<span data-ttu-id="4e5ac-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4e5ac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




