---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8986a64ffb06898c0935c3e07c9cb78641c58f4e
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940140"
---
# <a name="update-devicecategory"></a><span data-ttu-id="faf53-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="faf53-103">Update deviceCategory</span></span>

> <span data-ttu-id="faf53-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faf53-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="faf53-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="faf53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="faf53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faf53-107">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="faf53-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="faf53-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="faf53-108">Prerequisites</span></span>

<span data-ttu-id="faf53-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="faf53-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf53-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="faf53-111">Permission type</span></span>|<span data-ttu-id="faf53-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="faf53-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="faf53-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="faf53-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="faf53-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="faf53-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="faf53-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf53-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="faf53-116">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="faf53-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faf53-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf53-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="faf53-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="faf53-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="faf53-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf53-119">Not supported.</span></span>|
|<span data-ttu-id="faf53-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="faf53-120">Application</span></span>||
| <span data-ttu-id="faf53-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="faf53-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="faf53-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf53-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="faf53-123">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="faf53-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="faf53-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="faf53-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="faf53-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="faf53-125">HTTP Request</span></span>

<span data-ttu-id="faf53-126">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="faf53-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="faf53-127">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="faf53-127">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="faf53-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="faf53-128">Request headers</span></span>

|<span data-ttu-id="faf53-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="faf53-129">Header</span></span>|<span data-ttu-id="faf53-130">Значение</span><span class="sxs-lookup"><span data-stu-id="faf53-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faf53-131">Авторизация</span><span class="sxs-lookup"><span data-stu-id="faf53-131">Authorization</span></span>|<span data-ttu-id="faf53-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="faf53-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faf53-133">Accept</span><span class="sxs-lookup"><span data-stu-id="faf53-133">Accept</span></span>|<span data-ttu-id="faf53-134">application/json</span><span class="sxs-lookup"><span data-stu-id="faf53-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf53-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="faf53-135">Request body</span></span>

<span data-ttu-id="faf53-136">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faf53-136">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="faf53-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="faf53-137">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="faf53-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="faf53-138">Property</span></span>|<span data-ttu-id="faf53-139">Тип</span><span class="sxs-lookup"><span data-stu-id="faf53-139">Type</span></span>|<span data-ttu-id="faf53-140">Описание</span><span class="sxs-lookup"><span data-stu-id="faf53-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faf53-141">id</span><span class="sxs-lookup"><span data-stu-id="faf53-141">id</span></span>|<span data-ttu-id="faf53-142">String</span><span class="sxs-lookup"><span data-stu-id="faf53-142">String</span></span>|<span data-ttu-id="faf53-143">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="faf53-143">Unique identifier for the device category.</span></span> <span data-ttu-id="faf53-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="faf53-144">Read-only.</span></span>|
|<span data-ttu-id="faf53-145">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="faf53-145">**Onboarding**</span></span>|
|<span data-ttu-id="faf53-146">description</span><span class="sxs-lookup"><span data-stu-id="faf53-146">description</span></span>|<span data-ttu-id="faf53-147">String</span><span class="sxs-lookup"><span data-stu-id="faf53-147">String</span></span>|<span data-ttu-id="faf53-148">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="faf53-148">Optional description for the device category.</span></span>|
|<span data-ttu-id="faf53-149">displayName</span><span class="sxs-lookup"><span data-stu-id="faf53-149">displayName</span></span>|<span data-ttu-id="faf53-150">Строка</span><span class="sxs-lookup"><span data-stu-id="faf53-150">String</span></span>|<span data-ttu-id="faf53-151">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="faf53-151">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="faf53-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="faf53-152">Response</span></span>

<span data-ttu-id="faf53-153">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="faf53-153">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf53-154">Пример</span><span class="sxs-lookup"><span data-stu-id="faf53-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="faf53-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="faf53-155">Request</span></span>

<span data-ttu-id="faf53-156">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="faf53-156">Here are examples of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="faf53-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="faf53-157">Response</span></span>

<span data-ttu-id="faf53-158">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="faf53-158">Here is an example of the response.</span></span> <span data-ttu-id="faf53-159">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="faf53-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="faf53-160">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="faf53-160">Response properties will vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```











