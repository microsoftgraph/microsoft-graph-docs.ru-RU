---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b62523d4a17571c0ff6931b8ee462f21b4a1daa4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174540"
---
# <a name="get-devicecategory"></a><span data-ttu-id="6ccbe-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="6ccbe-103">Get deviceCategory</span></span>

> <span data-ttu-id="6ccbe-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6ccbe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ccbe-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ccbe-107">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="6ccbe-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ccbe-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6ccbe-108">Prerequisites</span></span>

<span data-ttu-id="6ccbe-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ccbe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="6ccbe-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6ccbe-111">Permission type</span></span>|<span data-ttu-id="6ccbe-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6ccbe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ccbe-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6ccbe-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6ccbe-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6ccbe-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="6ccbe-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ccbe-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="6ccbe-116">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="6ccbe-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="6ccbe-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ccbe-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="6ccbe-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6ccbe-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ccbe-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-119">Not supported.</span></span>|
|<span data-ttu-id="6ccbe-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6ccbe-120">Application</span></span>|<span data-ttu-id="6ccbe-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ccbe-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6ccbe-122">HTTP Request</span></span>

<span data-ttu-id="6ccbe-123">**Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="6ccbe-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="6ccbe-124">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="6ccbe-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6ccbe-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6ccbe-125">Optional query parameters</span></span>

<span data-ttu-id="6ccbe-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ccbe-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6ccbe-127">Request headers</span></span>

|<span data-ttu-id="6ccbe-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6ccbe-128">Header</span></span>|<span data-ttu-id="6ccbe-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6ccbe-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ccbe-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ccbe-130">Authorization</span></span>|<span data-ttu-id="6ccbe-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6ccbe-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ccbe-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6ccbe-132">Accept</span></span>|<span data-ttu-id="6ccbe-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6ccbe-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ccbe-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6ccbe-134">Request body</span></span>

<span data-ttu-id="6ccbe-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ccbe-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ccbe-136">Response</span></span>

<span data-ttu-id="6ccbe-137">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ccbe-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6ccbe-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ccbe-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="6ccbe-139">Request</span></span>

<span data-ttu-id="6ccbe-140">Ниже приведены примеры запроса.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="6ccbe-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="6ccbe-141">Response</span></span>

<span data-ttu-id="6ccbe-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-142">Here is an example of the response.</span></span> <span data-ttu-id="6ccbe-143">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6ccbe-144">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="6ccbe-144">Properties returned from an actual call vary according to context.</span></span>

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



