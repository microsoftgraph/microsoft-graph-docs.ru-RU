---
title: Создание объекта detectedApp
description: Создание объекта detectedApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 81eafad351604335d125bc01d7f314aa7a19b02c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364601"
---
# <a name="create-detectedapp"></a><span data-ttu-id="fdf3c-103">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="fdf3c-103">Create detectedApp</span></span>

> <span data-ttu-id="fdf3c-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdf3c-105">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fdf3c-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdf3c-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fdf3c-106">Prerequisites</span></span>
<span data-ttu-id="fdf3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fdf3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdf3c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fdf3c-109">Permission type</span></span>|<span data-ttu-id="fdf3c-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fdf3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdf3c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fdf3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fdf3c-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdf3c-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fdf3c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fdf3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdf3c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-114">Not supported.</span></span>|
|<span data-ttu-id="fdf3c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fdf3c-115">Application</span></span>|<span data-ttu-id="fdf3c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdf3c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fdf3c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="fdf3c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fdf3c-118">Request headers</span></span>
|<span data-ttu-id="fdf3c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fdf3c-119">Header</span></span>|<span data-ttu-id="fdf3c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fdf3c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdf3c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fdf3c-121">Authorization</span></span>|<span data-ttu-id="fdf3c-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdf3c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fdf3c-123">Accept</span></span>|<span data-ttu-id="fdf3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fdf3c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdf3c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fdf3c-125">Request body</span></span>
<span data-ttu-id="fdf3c-126">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="fdf3c-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="fdf3c-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="fdf3c-128">Property</span></span>|<span data-ttu-id="fdf3c-129">Тип</span><span class="sxs-lookup"><span data-stu-id="fdf3c-129">Type</span></span>|<span data-ttu-id="fdf3c-130">Описание</span><span class="sxs-lookup"><span data-stu-id="fdf3c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdf3c-131">id</span><span class="sxs-lookup"><span data-stu-id="fdf3c-131">id</span></span>|<span data-ttu-id="fdf3c-132">String</span><span class="sxs-lookup"><span data-stu-id="fdf3c-132">String</span></span>|<span data-ttu-id="fdf3c-133">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="fdf3c-134">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="fdf3c-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-135">Read-only.</span></span>|
|<span data-ttu-id="fdf3c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fdf3c-136">displayName</span></span>|<span data-ttu-id="fdf3c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="fdf3c-137">String</span></span>|<span data-ttu-id="fdf3c-138">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-138">Name of the discovered application.</span></span> <span data-ttu-id="fdf3c-139">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fdf3c-139">Read-only</span></span>|
|<span data-ttu-id="fdf3c-140">version</span><span class="sxs-lookup"><span data-stu-id="fdf3c-140">version</span></span>|<span data-ttu-id="fdf3c-141">String</span><span class="sxs-lookup"><span data-stu-id="fdf3c-141">String</span></span>|<span data-ttu-id="fdf3c-142">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-142">Version of the discovered application.</span></span> <span data-ttu-id="fdf3c-143">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fdf3c-143">Read-only</span></span>|
|<span data-ttu-id="fdf3c-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="fdf3c-144">sizeInByte</span></span>|<span data-ttu-id="fdf3c-145">Int64</span><span class="sxs-lookup"><span data-stu-id="fdf3c-145">Int64</span></span>|<span data-ttu-id="fdf3c-146">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-146">Discovered application size in bytes.</span></span> <span data-ttu-id="fdf3c-147">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="fdf3c-147">Read-only</span></span>|
|<span data-ttu-id="fdf3c-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fdf3c-148">deviceCount</span></span>|<span data-ttu-id="fdf3c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fdf3c-149">Int32</span></span>|<span data-ttu-id="fdf3c-150">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="fdf3c-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdf3c-151">Response</span></span>
<span data-ttu-id="fdf3c-152">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdf3c-153">Пример</span><span class="sxs-lookup"><span data-stu-id="fdf3c-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdf3c-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="fdf3c-154">Request</span></span>
<span data-ttu-id="fdf3c-155">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdf3c-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="fdf3c-156">Response</span></span>
<span data-ttu-id="fdf3c-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fdf3c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




