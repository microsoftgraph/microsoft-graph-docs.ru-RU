---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bfea341aafb25ea010162d270eab451900c0d04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394945"
---
# <a name="update-detectedapp"></a><span data-ttu-id="137ee-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="137ee-103">Update detectedApp</span></span>

> <span data-ttu-id="137ee-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="137ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="137ee-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="137ee-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="137ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="137ee-107">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="137ee-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="137ee-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="137ee-108">Prerequisites</span></span>
<span data-ttu-id="137ee-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="137ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="137ee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="137ee-111">Permission type</span></span>|<span data-ttu-id="137ee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="137ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="137ee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="137ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="137ee-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="137ee-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="137ee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="137ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="137ee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137ee-116">Not supported.</span></span>|
|<span data-ttu-id="137ee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="137ee-117">Application</span></span>|<span data-ttu-id="137ee-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="137ee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="137ee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="137ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="137ee-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="137ee-120">Request headers</span></span>
|<span data-ttu-id="137ee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="137ee-121">Header</span></span>|<span data-ttu-id="137ee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="137ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="137ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="137ee-123">Authorization</span></span>|<span data-ttu-id="137ee-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="137ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="137ee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="137ee-125">Accept</span></span>|<span data-ttu-id="137ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="137ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="137ee-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="137ee-127">Request body</span></span>
<span data-ttu-id="137ee-128">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="137ee-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="137ee-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="137ee-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="137ee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="137ee-130">Property</span></span>|<span data-ttu-id="137ee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="137ee-131">Type</span></span>|<span data-ttu-id="137ee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="137ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="137ee-133">id</span><span class="sxs-lookup"><span data-stu-id="137ee-133">id</span></span>|<span data-ttu-id="137ee-134">String</span><span class="sxs-lookup"><span data-stu-id="137ee-134">String</span></span>|<span data-ttu-id="137ee-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="137ee-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="137ee-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="137ee-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="137ee-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="137ee-137">Read-only.</span></span>|
|<span data-ttu-id="137ee-138">displayName</span><span class="sxs-lookup"><span data-stu-id="137ee-138">displayName</span></span>|<span data-ttu-id="137ee-139">String</span><span class="sxs-lookup"><span data-stu-id="137ee-139">String</span></span>|<span data-ttu-id="137ee-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="137ee-140">Name of the discovered application.</span></span> <span data-ttu-id="137ee-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="137ee-141">Read-only</span></span>|
|<span data-ttu-id="137ee-142">version</span><span class="sxs-lookup"><span data-stu-id="137ee-142">version</span></span>|<span data-ttu-id="137ee-143">String</span><span class="sxs-lookup"><span data-stu-id="137ee-143">String</span></span>|<span data-ttu-id="137ee-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="137ee-144">Version of the discovered application.</span></span> <span data-ttu-id="137ee-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="137ee-145">Read-only</span></span>|
|<span data-ttu-id="137ee-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="137ee-146">sizeInByte</span></span>|<span data-ttu-id="137ee-147">Int64</span><span class="sxs-lookup"><span data-stu-id="137ee-147">Int64</span></span>|<span data-ttu-id="137ee-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="137ee-148">Discovered application size in bytes.</span></span> <span data-ttu-id="137ee-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="137ee-149">Read-only</span></span>|
|<span data-ttu-id="137ee-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="137ee-150">deviceCount</span></span>|<span data-ttu-id="137ee-151">Int32</span><span class="sxs-lookup"><span data-stu-id="137ee-151">Int32</span></span>|<span data-ttu-id="137ee-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="137ee-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="137ee-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="137ee-153">Response</span></span>
<span data-ttu-id="137ee-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="137ee-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="137ee-155">Пример</span><span class="sxs-lookup"><span data-stu-id="137ee-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="137ee-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="137ee-156">Request</span></span>
<span data-ttu-id="137ee-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="137ee-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="137ee-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="137ee-158">Response</span></span>
<span data-ttu-id="137ee-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="137ee-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




