---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa64e0071da331ec79eaea581e1c91bb514ad04d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980430"
---
# <a name="get-devicecategory"></a><span data-ttu-id="58517-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="58517-103">Get deviceCategory</span></span>

<span data-ttu-id="58517-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58517-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58517-105">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="58517-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58517-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58517-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58517-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="58517-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58517-108">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="58517-108">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58517-109">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="58517-109">Prerequisites</span></span>

<span data-ttu-id="58517-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58517-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58517-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="58517-112">Permission type</span></span>|<span data-ttu-id="58517-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="58517-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58517-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="58517-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="58517-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="58517-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="58517-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58517-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="58517-117">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="58517-117">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="58517-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58517-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="58517-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="58517-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58517-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="58517-120">Not supported.</span></span>|
|<span data-ttu-id="58517-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="58517-121">Application</span></span>||
| <span data-ttu-id="58517-122">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="58517-122">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="58517-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58517-123">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="58517-124">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="58517-124">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="58517-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="58517-125">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58517-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="58517-126">HTTP Request</span></span>

<span data-ttu-id="58517-127">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="58517-127">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="58517-128">**Адаптация**</span><span class="sxs-lookup"><span data-stu-id="58517-128">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58517-129">Необязательные параметры запроса</span><span class="sxs-lookup"><span data-stu-id="58517-129">Optional query parameters</span></span>

<span data-ttu-id="58517-130">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="58517-130">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="58517-131">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="58517-131">Request headers</span></span>

|<span data-ttu-id="58517-132">Заголовок</span><span class="sxs-lookup"><span data-stu-id="58517-132">Header</span></span>|<span data-ttu-id="58517-133">Значение</span><span class="sxs-lookup"><span data-stu-id="58517-133">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58517-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="58517-134">Authorization</span></span>|<span data-ttu-id="58517-135">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="58517-135">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58517-136">Accept</span><span class="sxs-lookup"><span data-stu-id="58517-136">Accept</span></span>|<span data-ttu-id="58517-137">application/json</span><span class="sxs-lookup"><span data-stu-id="58517-137">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58517-138">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="58517-138">Request body</span></span>

<span data-ttu-id="58517-139">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="58517-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58517-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="58517-140">Response</span></span>

<span data-ttu-id="58517-141">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="58517-141">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58517-142">Пример</span><span class="sxs-lookup"><span data-stu-id="58517-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="58517-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="58517-143">Request</span></span>

<span data-ttu-id="58517-144">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="58517-144">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="58517-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="58517-145">Response</span></span>

<span data-ttu-id="58517-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="58517-146">Here is an example of the response.</span></span> <span data-ttu-id="58517-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="58517-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="58517-148">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="58517-148">Properties returned from an actual call vary according to context.</span></span>

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












