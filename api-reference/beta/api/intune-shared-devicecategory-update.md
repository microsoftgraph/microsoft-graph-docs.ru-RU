---
title: Обновление объекта deviceCategory
description: Обновление свойств объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4dd8b61a9d07ccf8a6b79f3859034ee49cd5907
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979780"
---
# <a name="update-devicecategory"></a><span data-ttu-id="ac716-103">Обновление объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ac716-103">Update deviceCategory</span></span>

> <span data-ttu-id="ac716-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ac716-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac716-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac716-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac716-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac716-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac716-107">Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="ac716-107">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac716-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ac716-108">Prerequisites</span></span>

<span data-ttu-id="ac716-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac716-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac716-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac716-111">Permission type</span></span>|<span data-ttu-id="ac716-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac716-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac716-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac716-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ac716-114">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ac716-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="ac716-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac716-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="ac716-116">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="ac716-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ac716-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac716-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ac716-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac716-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac716-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac716-119">Not supported.</span></span>|
|<span data-ttu-id="ac716-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac716-120">Application</span></span>|<span data-ttu-id="ac716-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac716-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac716-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac716-122">HTTP Request</span></span>

<span data-ttu-id="ac716-123">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="ac716-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

<span data-ttu-id="ac716-124">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="ac716-124">**On-boarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="ac716-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac716-125">Request headers</span></span>

|<span data-ttu-id="ac716-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ac716-126">Header</span></span>|<span data-ttu-id="ac716-127">Значение</span><span class="sxs-lookup"><span data-stu-id="ac716-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac716-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac716-128">Authorization</span></span>|<span data-ttu-id="ac716-129">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac716-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac716-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ac716-130">Accept</span></span>|<span data-ttu-id="ac716-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ac716-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac716-132">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ac716-132">Request body</span></span>

<span data-ttu-id="ac716-133">В теле запроса добавьте представление объекта [deviceCategory](../resources/intune-shared-devicecategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac716-133">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

<span data-ttu-id="ac716-134">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="ac716-134">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>

|<span data-ttu-id="ac716-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac716-135">Property</span></span>|<span data-ttu-id="ac716-136">Тип</span><span class="sxs-lookup"><span data-stu-id="ac716-136">Type</span></span>|<span data-ttu-id="ac716-137">Описание</span><span class="sxs-lookup"><span data-stu-id="ac716-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac716-138">id</span><span class="sxs-lookup"><span data-stu-id="ac716-138">id</span></span>|<span data-ttu-id="ac716-139">String</span><span class="sxs-lookup"><span data-stu-id="ac716-139">String</span></span>|<span data-ttu-id="ac716-140">Уникальный идентификатор категории устройства.</span><span class="sxs-lookup"><span data-stu-id="ac716-140">Unique identifier for the device category.</span></span> <span data-ttu-id="ac716-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ac716-141">Read-only.</span></span>|
|<span data-ttu-id="ac716-142">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="ac716-142">**Onboarding**</span></span>|
|<span data-ttu-id="ac716-143">description</span><span class="sxs-lookup"><span data-stu-id="ac716-143">description</span></span>|<span data-ttu-id="ac716-144">String</span><span class="sxs-lookup"><span data-stu-id="ac716-144">String</span></span>|<span data-ttu-id="ac716-145">Необязательное описание категории устройств.</span><span class="sxs-lookup"><span data-stu-id="ac716-145">Optional description for the device category.</span></span>|
|<span data-ttu-id="ac716-146">displayName</span><span class="sxs-lookup"><span data-stu-id="ac716-146">displayName</span></span>|<span data-ttu-id="ac716-147">Строка</span><span class="sxs-lookup"><span data-stu-id="ac716-147">String</span></span>|<span data-ttu-id="ac716-148">Отображаемое имя категории устройств.</span><span class="sxs-lookup"><span data-stu-id="ac716-148">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="ac716-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac716-149">Response</span></span>

<span data-ttu-id="ac716-150">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ac716-150">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac716-151">Пример</span><span class="sxs-lookup"><span data-stu-id="ac716-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac716-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac716-152">Request</span></span>

<span data-ttu-id="ac716-153">Ниже приведено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="ac716-153">Here are examples of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="ac716-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="ac716-154">Response</span></span>

<span data-ttu-id="ac716-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ac716-155">Here is an example of the response.</span></span> <span data-ttu-id="ac716-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="ac716-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ac716-157">Свойства ответа будут зависеть от контекста.</span><span class="sxs-lookup"><span data-stu-id="ac716-157">Response properties will vary according to context.</span></span>

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



