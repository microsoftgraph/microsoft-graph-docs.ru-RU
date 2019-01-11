---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86b8eb3bc1bac0902ce36bd763c633f06919d2fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821933"
---
# <a name="update-detectedapp"></a><span data-ttu-id="a3a25-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="a3a25-103">Update detectedApp</span></span>

> <span data-ttu-id="a3a25-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a3a25-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3a25-105">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3a25-105">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3a25-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="a3a25-106">Prerequisites</span></span>
<span data-ttu-id="a3a25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3a25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3a25-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a3a25-109">Permission type</span></span>|<span data-ttu-id="a3a25-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a3a25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3a25-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a3a25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3a25-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3a25-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a3a25-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a3a25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3a25-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a25-114">Not supported.</span></span>|
|<span data-ttu-id="a3a25-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a3a25-115">Application</span></span>|<span data-ttu-id="a3a25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3a25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3a25-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a3a25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a3a25-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a3a25-118">Request headers</span></span>
|<span data-ttu-id="a3a25-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a3a25-119">Header</span></span>|<span data-ttu-id="a3a25-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a3a25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3a25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3a25-121">Authorization</span></span>|<span data-ttu-id="a3a25-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a3a25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3a25-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a3a25-123">Accept</span></span>|<span data-ttu-id="a3a25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3a25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3a25-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a3a25-125">Request body</span></span>
<span data-ttu-id="a3a25-126">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3a25-126">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="a3a25-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a3a25-127">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="a3a25-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3a25-128">Property</span></span>|<span data-ttu-id="a3a25-129">Тип</span><span class="sxs-lookup"><span data-stu-id="a3a25-129">Type</span></span>|<span data-ttu-id="a3a25-130">Описание</span><span class="sxs-lookup"><span data-stu-id="a3a25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3a25-131">id</span><span class="sxs-lookup"><span data-stu-id="a3a25-131">id</span></span>|<span data-ttu-id="a3a25-132">String</span><span class="sxs-lookup"><span data-stu-id="a3a25-132">String</span></span>|<span data-ttu-id="a3a25-133">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a25-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="a3a25-134">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a25-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="a3a25-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a3a25-135">Read-only.</span></span>|
|<span data-ttu-id="a3a25-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a3a25-136">displayName</span></span>|<span data-ttu-id="a3a25-137">String</span><span class="sxs-lookup"><span data-stu-id="a3a25-137">String</span></span>|<span data-ttu-id="a3a25-138">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a25-138">Name of the discovered application.</span></span> <span data-ttu-id="a3a25-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="a3a25-139">Read-only</span></span>|
|<span data-ttu-id="a3a25-140">version</span><span class="sxs-lookup"><span data-stu-id="a3a25-140">version</span></span>|<span data-ttu-id="a3a25-141">String</span><span class="sxs-lookup"><span data-stu-id="a3a25-141">String</span></span>|<span data-ttu-id="a3a25-142">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="a3a25-142">Version of the discovered application.</span></span> <span data-ttu-id="a3a25-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="a3a25-143">Read-only</span></span>|
|<span data-ttu-id="a3a25-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="a3a25-144">sizeInByte</span></span>|<span data-ttu-id="a3a25-145">Int64</span><span class="sxs-lookup"><span data-stu-id="a3a25-145">Int64</span></span>|<span data-ttu-id="a3a25-146">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="a3a25-146">Discovered application size in bytes.</span></span> <span data-ttu-id="a3a25-147">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="a3a25-147">Read-only</span></span>|
|<span data-ttu-id="a3a25-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a3a25-148">deviceCount</span></span>|<span data-ttu-id="a3a25-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a3a25-149">Int32</span></span>|<span data-ttu-id="a3a25-150">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="a3a25-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="a3a25-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="a3a25-151">Response</span></span>
<span data-ttu-id="a3a25-152">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a3a25-152">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3a25-153">Пример</span><span class="sxs-lookup"><span data-stu-id="a3a25-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3a25-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="a3a25-154">Request</span></span>
<span data-ttu-id="a3a25-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a3a25-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
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

### <a name="response"></a><span data-ttu-id="a3a25-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="a3a25-156">Response</span></span>
<span data-ttu-id="a3a25-p106">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a3a25-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



