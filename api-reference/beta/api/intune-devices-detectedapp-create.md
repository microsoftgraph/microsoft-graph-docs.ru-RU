---
title: Создание объекта detectedApp
description: Создание объекта detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0949b00473e11e922db051c806174a2109362f65
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188677"
---
# <a name="create-detectedapp"></a><span data-ttu-id="bdaac-103">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="bdaac-103">Create detectedApp</span></span>

> <span data-ttu-id="bdaac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bdaac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bdaac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bdaac-106">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bdaac-106">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bdaac-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bdaac-107">Prerequisites</span></span>
<span data-ttu-id="bdaac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdaac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdaac-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bdaac-110">Permission type</span></span>|<span data-ttu-id="bdaac-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bdaac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdaac-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bdaac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bdaac-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdaac-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bdaac-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bdaac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdaac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bdaac-115">Not supported.</span></span>|
|<span data-ttu-id="bdaac-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bdaac-116">Application</span></span>|<span data-ttu-id="bdaac-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdaac-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdaac-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bdaac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="bdaac-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bdaac-119">Request headers</span></span>
|<span data-ttu-id="bdaac-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bdaac-120">Header</span></span>|<span data-ttu-id="bdaac-121">Значение</span><span class="sxs-lookup"><span data-stu-id="bdaac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdaac-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bdaac-122">Authorization</span></span>|<span data-ttu-id="bdaac-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bdaac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdaac-124">Accept</span><span class="sxs-lookup"><span data-stu-id="bdaac-124">Accept</span></span>|<span data-ttu-id="bdaac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bdaac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdaac-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bdaac-126">Request body</span></span>
<span data-ttu-id="bdaac-127">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bdaac-127">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="bdaac-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="bdaac-128">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="bdaac-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="bdaac-129">Property</span></span>|<span data-ttu-id="bdaac-130">Тип</span><span class="sxs-lookup"><span data-stu-id="bdaac-130">Type</span></span>|<span data-ttu-id="bdaac-131">Описание</span><span class="sxs-lookup"><span data-stu-id="bdaac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdaac-132">id</span><span class="sxs-lookup"><span data-stu-id="bdaac-132">id</span></span>|<span data-ttu-id="bdaac-133">String</span><span class="sxs-lookup"><span data-stu-id="bdaac-133">String</span></span>|<span data-ttu-id="bdaac-134">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bdaac-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="bdaac-135">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="bdaac-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="bdaac-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bdaac-136">Read-only.</span></span>|
|<span data-ttu-id="bdaac-137">displayName</span><span class="sxs-lookup"><span data-stu-id="bdaac-137">displayName</span></span>|<span data-ttu-id="bdaac-138">Строка</span><span class="sxs-lookup"><span data-stu-id="bdaac-138">String</span></span>|<span data-ttu-id="bdaac-139">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bdaac-139">Name of the discovered application.</span></span> <span data-ttu-id="bdaac-140">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bdaac-140">Read-only</span></span>|
|<span data-ttu-id="bdaac-141">version</span><span class="sxs-lookup"><span data-stu-id="bdaac-141">version</span></span>|<span data-ttu-id="bdaac-142">String</span><span class="sxs-lookup"><span data-stu-id="bdaac-142">String</span></span>|<span data-ttu-id="bdaac-143">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bdaac-143">Version of the discovered application.</span></span> <span data-ttu-id="bdaac-144">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bdaac-144">Read-only</span></span>|
|<span data-ttu-id="bdaac-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="bdaac-145">sizeInByte</span></span>|<span data-ttu-id="bdaac-146">Int64</span><span class="sxs-lookup"><span data-stu-id="bdaac-146">Int64</span></span>|<span data-ttu-id="bdaac-147">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="bdaac-147">Discovered application size in bytes.</span></span> <span data-ttu-id="bdaac-148">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bdaac-148">Read-only</span></span>|
|<span data-ttu-id="bdaac-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bdaac-149">deviceCount</span></span>|<span data-ttu-id="bdaac-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bdaac-150">Int32</span></span>|<span data-ttu-id="bdaac-151">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="bdaac-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="bdaac-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdaac-152">Response</span></span>
<span data-ttu-id="bdaac-153">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bdaac-153">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdaac-154">Пример</span><span class="sxs-lookup"><span data-stu-id="bdaac-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="bdaac-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="bdaac-155">Request</span></span>
<span data-ttu-id="bdaac-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bdaac-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="bdaac-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="bdaac-157">Response</span></span>
<span data-ttu-id="bdaac-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bdaac-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




