---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 77bfb3880db9b7e36c8e6b9e8d2a8b53ab3450d6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914999"
---
# <a name="update-detectedapp"></a><span data-ttu-id="2f15f-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="2f15f-103">Update detectedApp</span></span>

> <span data-ttu-id="2f15f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2f15f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2f15f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f15f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f15f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2f15f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2f15f-107">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f15f-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f15f-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f15f-108">Prerequisites</span></span>
<span data-ttu-id="2f15f-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f15f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f15f-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f15f-111">Permission type</span></span>|<span data-ttu-id="2f15f-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f15f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f15f-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f15f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f15f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f15f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f15f-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f15f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f15f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f15f-116">Not supported.</span></span>|
|<span data-ttu-id="2f15f-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f15f-117">Application</span></span>|<span data-ttu-id="2f15f-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f15f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f15f-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f15f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2f15f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f15f-120">Request headers</span></span>
|<span data-ttu-id="2f15f-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f15f-121">Header</span></span>|<span data-ttu-id="2f15f-122">Значение</span><span class="sxs-lookup"><span data-stu-id="2f15f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f15f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f15f-123">Authorization</span></span>|<span data-ttu-id="2f15f-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="2f15f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f15f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2f15f-125">Accept</span></span>|<span data-ttu-id="2f15f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f15f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f15f-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2f15f-127">Request body</span></span>
<span data-ttu-id="2f15f-128">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f15f-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="2f15f-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2f15f-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="2f15f-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f15f-130">Property</span></span>|<span data-ttu-id="2f15f-131">Тип</span><span class="sxs-lookup"><span data-stu-id="2f15f-131">Type</span></span>|<span data-ttu-id="2f15f-132">Описание</span><span class="sxs-lookup"><span data-stu-id="2f15f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f15f-133">id</span><span class="sxs-lookup"><span data-stu-id="2f15f-133">id</span></span>|<span data-ttu-id="2f15f-134">String</span><span class="sxs-lookup"><span data-stu-id="2f15f-134">String</span></span>|<span data-ttu-id="2f15f-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="2f15f-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="2f15f-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="2f15f-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="2f15f-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2f15f-137">Read-only.</span></span>|
|<span data-ttu-id="2f15f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2f15f-138">displayName</span></span>|<span data-ttu-id="2f15f-139">String</span><span class="sxs-lookup"><span data-stu-id="2f15f-139">String</span></span>|<span data-ttu-id="2f15f-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="2f15f-140">Name of the discovered application.</span></span> <span data-ttu-id="2f15f-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="2f15f-141">Read-only</span></span>|
|<span data-ttu-id="2f15f-142">version</span><span class="sxs-lookup"><span data-stu-id="2f15f-142">version</span></span>|<span data-ttu-id="2f15f-143">String</span><span class="sxs-lookup"><span data-stu-id="2f15f-143">String</span></span>|<span data-ttu-id="2f15f-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="2f15f-144">Version of the discovered application.</span></span> <span data-ttu-id="2f15f-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="2f15f-145">Read-only</span></span>|
|<span data-ttu-id="2f15f-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="2f15f-146">sizeInByte</span></span>|<span data-ttu-id="2f15f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="2f15f-147">Int64</span></span>|<span data-ttu-id="2f15f-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="2f15f-148">Discovered application size in bytes.</span></span> <span data-ttu-id="2f15f-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="2f15f-149">Read-only</span></span>|
|<span data-ttu-id="2f15f-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2f15f-150">deviceCount</span></span>|<span data-ttu-id="2f15f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2f15f-151">Int32</span></span>|<span data-ttu-id="2f15f-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="2f15f-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="2f15f-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f15f-153">Response</span></span>
<span data-ttu-id="2f15f-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f15f-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f15f-155">Пример</span><span class="sxs-lookup"><span data-stu-id="2f15f-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f15f-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f15f-156">Request</span></span>
<span data-ttu-id="2f15f-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f15f-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 117

{
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="2f15f-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f15f-158">Response</span></span>
<span data-ttu-id="2f15f-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2f15f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





