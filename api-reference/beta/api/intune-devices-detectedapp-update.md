---
title: Обновление объекта detectedApp
description: Обновление свойств объекта detectedApp.
ms.openlocfilehash: 58fa37603b583a4ccf0579d2c6021ed5c1e60cc4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076780"
---
# <a name="update-detectedapp"></a><span data-ttu-id="bc613-103">Обновление объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="bc613-103">Update detectedApp</span></span>

> <span data-ttu-id="bc613-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc613-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc613-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc613-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc613-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc613-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc613-107">Обновление свойств объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc613-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bc613-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bc613-108">Prerequisites</span></span>
<span data-ttu-id="bc613-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc613-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc613-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc613-111">Permission type</span></span>|<span data-ttu-id="bc613-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc613-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bc613-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc613-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bc613-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc613-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bc613-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc613-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bc613-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc613-116">Not supported.</span></span>|
|<span data-ttu-id="bc613-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc613-117">Application</span></span>|<span data-ttu-id="bc613-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc613-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc613-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc613-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="bc613-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc613-120">Request headers</span></span>
|<span data-ttu-id="bc613-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bc613-121">Header</span></span>|<span data-ttu-id="bc613-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bc613-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc613-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc613-123">Authorization</span></span>|<span data-ttu-id="bc613-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bc613-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc613-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bc613-125">Accept</span></span>|<span data-ttu-id="bc613-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc613-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc613-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc613-127">Request body</span></span>
<span data-ttu-id="bc613-128">В теле запроса добавьте представление объекта [detectedApp](../resources/intune-devices-detectedapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc613-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="bc613-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="bc613-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="bc613-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc613-130">Property</span></span>|<span data-ttu-id="bc613-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bc613-131">Type</span></span>|<span data-ttu-id="bc613-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bc613-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc613-133">id</span><span class="sxs-lookup"><span data-stu-id="bc613-133">id</span></span>|<span data-ttu-id="bc613-134">String</span><span class="sxs-lookup"><span data-stu-id="bc613-134">String</span></span>|<span data-ttu-id="bc613-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bc613-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="bc613-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="bc613-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="bc613-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bc613-137">Read-only.</span></span>|
|<span data-ttu-id="bc613-138">displayName</span><span class="sxs-lookup"><span data-stu-id="bc613-138">displayName</span></span>|<span data-ttu-id="bc613-139">String</span><span class="sxs-lookup"><span data-stu-id="bc613-139">String</span></span>|<span data-ttu-id="bc613-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bc613-140">Name of the discovered application.</span></span> <span data-ttu-id="bc613-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bc613-141">Read-only</span></span>|
|<span data-ttu-id="bc613-142">version</span><span class="sxs-lookup"><span data-stu-id="bc613-142">version</span></span>|<span data-ttu-id="bc613-143">String</span><span class="sxs-lookup"><span data-stu-id="bc613-143">String</span></span>|<span data-ttu-id="bc613-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="bc613-144">Version of the discovered application.</span></span> <span data-ttu-id="bc613-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bc613-145">Read-only</span></span>|
|<span data-ttu-id="bc613-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="bc613-146">sizeInByte</span></span>|<span data-ttu-id="bc613-147">Int64</span><span class="sxs-lookup"><span data-stu-id="bc613-147">Int64</span></span>|<span data-ttu-id="bc613-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="bc613-148">Discovered application size in bytes.</span></span> <span data-ttu-id="bc613-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="bc613-149">Read-only</span></span>|
|<span data-ttu-id="bc613-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bc613-150">deviceCount</span></span>|<span data-ttu-id="bc613-151">Int32</span><span class="sxs-lookup"><span data-stu-id="bc613-151">Int32</span></span>|<span data-ttu-id="bc613-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="bc613-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="bc613-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc613-153">Response</span></span>
<span data-ttu-id="bc613-154">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bc613-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc613-155">Пример</span><span class="sxs-lookup"><span data-stu-id="bc613-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="bc613-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc613-156">Request</span></span>
<span data-ttu-id="bc613-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc613-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bc613-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc613-158">Response</span></span>
<span data-ttu-id="bc613-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bc613-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





