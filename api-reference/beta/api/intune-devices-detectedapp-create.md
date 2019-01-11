---
title: Создание объекта detectedApp
description: Создание объекта detectedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: da35940ba44790bdaec19a6c841bb5d90312b5f3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856317"
---
# <a name="create-detectedapp"></a><span data-ttu-id="7f35c-103">Создание объекта detectedApp</span><span class="sxs-lookup"><span data-stu-id="7f35c-103">Create detectedApp</span></span>

> <span data-ttu-id="7f35c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7f35c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f35c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f35c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f35c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f35c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f35c-107">Создание объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7f35c-107">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f35c-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f35c-108">Prerequisites</span></span>
<span data-ttu-id="7f35c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f35c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f35c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f35c-111">Permission type</span></span>|<span data-ttu-id="7f35c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f35c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f35c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f35c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f35c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f35c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7f35c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f35c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f35c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f35c-116">Not supported.</span></span>|
|<span data-ttu-id="7f35c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f35c-117">Application</span></span>|<span data-ttu-id="7f35c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f35c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f35c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f35c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="7f35c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f35c-120">Request headers</span></span>
|<span data-ttu-id="7f35c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f35c-121">Header</span></span>|<span data-ttu-id="7f35c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="7f35c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f35c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f35c-123">Authorization</span></span>|<span data-ttu-id="7f35c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7f35c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f35c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f35c-125">Accept</span></span>|<span data-ttu-id="7f35c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f35c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f35c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f35c-127">Request body</span></span>
<span data-ttu-id="7f35c-128">В теле запроса добавьте представление объекта detectedApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f35c-128">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="7f35c-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта detectedApp.</span><span class="sxs-lookup"><span data-stu-id="7f35c-129">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="7f35c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f35c-130">Property</span></span>|<span data-ttu-id="7f35c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="7f35c-131">Type</span></span>|<span data-ttu-id="7f35c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="7f35c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f35c-133">id</span><span class="sxs-lookup"><span data-stu-id="7f35c-133">id</span></span>|<span data-ttu-id="7f35c-134">String</span><span class="sxs-lookup"><span data-stu-id="7f35c-134">String</span></span>|<span data-ttu-id="7f35c-135">Уникальный идентификатор для обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="7f35c-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="7f35c-136">Он создается Intune автоматически при создании приложения.</span><span class="sxs-lookup"><span data-stu-id="7f35c-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="7f35c-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7f35c-137">Read-only.</span></span>|
|<span data-ttu-id="7f35c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7f35c-138">displayName</span></span>|<span data-ttu-id="7f35c-139">String</span><span class="sxs-lookup"><span data-stu-id="7f35c-139">String</span></span>|<span data-ttu-id="7f35c-140">Имя обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="7f35c-140">Name of the discovered application.</span></span> <span data-ttu-id="7f35c-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="7f35c-141">Read-only</span></span>|
|<span data-ttu-id="7f35c-142">version</span><span class="sxs-lookup"><span data-stu-id="7f35c-142">version</span></span>|<span data-ttu-id="7f35c-143">String</span><span class="sxs-lookup"><span data-stu-id="7f35c-143">String</span></span>|<span data-ttu-id="7f35c-144">Версия обнаруженного приложения.</span><span class="sxs-lookup"><span data-stu-id="7f35c-144">Version of the discovered application.</span></span> <span data-ttu-id="7f35c-145">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="7f35c-145">Read-only</span></span>|
|<span data-ttu-id="7f35c-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="7f35c-146">sizeInByte</span></span>|<span data-ttu-id="7f35c-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7f35c-147">Int64</span></span>|<span data-ttu-id="7f35c-148">Размер обнаруженного приложения в байтах.</span><span class="sxs-lookup"><span data-stu-id="7f35c-148">Discovered application size in bytes.</span></span> <span data-ttu-id="7f35c-149">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="7f35c-149">Read-only</span></span>|
|<span data-ttu-id="7f35c-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7f35c-150">deviceCount</span></span>|<span data-ttu-id="7f35c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7f35c-151">Int32</span></span>|<span data-ttu-id="7f35c-152">Количество устройств, на которых успешно установлено это приложение.</span><span class="sxs-lookup"><span data-stu-id="7f35c-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="7f35c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f35c-153">Response</span></span>
<span data-ttu-id="7f35c-154">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f35c-154">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f35c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="7f35c-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f35c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f35c-156">Request</span></span>
<span data-ttu-id="7f35c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f35c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7f35c-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f35c-158">Response</span></span>
<span data-ttu-id="7f35c-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7f35c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





