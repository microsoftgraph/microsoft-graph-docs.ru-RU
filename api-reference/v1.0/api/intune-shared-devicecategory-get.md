---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e371567d984285365fcadb6c2304a560638d0a04
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48401273"
---
# <a name="get-devicecategory"></a><span data-ttu-id="1142a-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1142a-103">Get deviceCategory</span></span>

<span data-ttu-id="1142a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1142a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1142a-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1142a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1142a-106">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="1142a-106">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1142a-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1142a-107">Prerequisites</span></span>
<span data-ttu-id="1142a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1142a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1142a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1142a-110">Permission type</span></span>|<span data-ttu-id="1142a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1142a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1142a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1142a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1142a-113">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="1142a-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1142a-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1142a-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="1142a-115">&nbsp; &nbsp; **Адаптация**</span><span class="sxs-lookup"><span data-stu-id="1142a-115">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="1142a-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1142a-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1142a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1142a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1142a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1142a-118">Not supported.</span></span>|
|<span data-ttu-id="1142a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1142a-119">Application</span></span>|<span data-ttu-id="1142a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1142a-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1142a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1142a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1142a-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1142a-122">Optional query parameters</span></span>
<span data-ttu-id="1142a-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1142a-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1142a-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1142a-124">Request headers</span></span>
|<span data-ttu-id="1142a-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1142a-125">Header</span></span>|<span data-ttu-id="1142a-126">Значение</span><span class="sxs-lookup"><span data-stu-id="1142a-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1142a-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1142a-127">Authorization</span></span>|<span data-ttu-id="1142a-128">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1142a-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1142a-129">Accept</span><span class="sxs-lookup"><span data-stu-id="1142a-129">Accept</span></span>|<span data-ttu-id="1142a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="1142a-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1142a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1142a-131">Request body</span></span>
<span data-ttu-id="1142a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1142a-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1142a-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1142a-133">Response</span></span>
<span data-ttu-id="1142a-134">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1142a-134">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1142a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="1142a-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="1142a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="1142a-136">Request</span></span>
<span data-ttu-id="1142a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1142a-137">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="1142a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1142a-138">Response</span></span>
<span data-ttu-id="1142a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1142a-139">Here is an example of the response.</span></span> <span data-ttu-id="1142a-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="1142a-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1142a-141">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="1142a-141">Properties returned from an actual call vary according to context.</span></span>

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