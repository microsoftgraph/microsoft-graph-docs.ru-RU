---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f634d5ca490a7ae28ab134dbcbb60fff7f2e1721
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940154"
---
# <a name="get-devicecategory"></a><span data-ttu-id="fe830-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="fe830-103">Get deviceCategory</span></span>

> <span data-ttu-id="fe830-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe830-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe830-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe830-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe830-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe830-107">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="fe830-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe830-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="fe830-108">Prerequisites</span></span>

<span data-ttu-id="fe830-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe830-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe830-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe830-111">Permission type</span></span>|<span data-ttu-id="fe830-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fe830-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe830-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe830-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fe830-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fe830-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe830-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe830-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fe830-116">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fe830-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fe830-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe830-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="fe830-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fe830-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe830-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe830-119">Not supported.</span></span>|
|<span data-ttu-id="fe830-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe830-120">Application</span></span>||
| <span data-ttu-id="fe830-121">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fe830-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="fe830-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe830-122">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="fe830-123">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fe830-123">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="fe830-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe830-124">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe830-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe830-125">HTTP Request</span></span>

<span data-ttu-id="fe830-126">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="fe830-126">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="fe830-127">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="fe830-127">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe830-128">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fe830-128">Optional query parameters</span></span>

<span data-ttu-id="fe830-129">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fe830-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe830-130">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe830-130">Request headers</span></span>

|<span data-ttu-id="fe830-131">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fe830-131">Header</span></span>|<span data-ttu-id="fe830-132">Значение</span><span class="sxs-lookup"><span data-stu-id="fe830-132">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe830-133">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fe830-133">Authorization</span></span>|<span data-ttu-id="fe830-134">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe830-134">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe830-135">Accept</span><span class="sxs-lookup"><span data-stu-id="fe830-135">Accept</span></span>|<span data-ttu-id="fe830-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fe830-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe830-137">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fe830-137">Request body</span></span>

<span data-ttu-id="fe830-138">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fe830-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe830-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe830-139">Response</span></span>

<span data-ttu-id="fe830-140">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fe830-140">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe830-141">Пример</span><span class="sxs-lookup"><span data-stu-id="fe830-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe830-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe830-142">Request</span></span>

<span data-ttu-id="fe830-143">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="fe830-143">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="fe830-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="fe830-144">Response</span></span>

<span data-ttu-id="fe830-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe830-145">Here is an example of the response.</span></span> <span data-ttu-id="fe830-146">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="fe830-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fe830-147">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="fe830-147">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```











