---
title: Получение объекта deviceCategory
description: Чтение свойств и связей объекта deviceCategory.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5ad4c146eb4a5344b87becdf3e82ae76b0808153
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361513"
---
# <a name="get-devicecategory"></a><span data-ttu-id="2f925-103">Получение объекта deviceCategory</span><span class="sxs-lookup"><span data-stu-id="2f925-103">Get deviceCategory</span></span>

> <span data-ttu-id="2f925-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f925-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f925-105">Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).</span><span class="sxs-lookup"><span data-stu-id="2f925-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f925-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="2f925-106">Prerequisites</span></span>
<span data-ttu-id="2f925-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f925-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f925-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f925-109">Permission type</span></span>|<span data-ttu-id="2f925-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2f925-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f925-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f925-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2f925-112">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="2f925-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2f925-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f925-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="2f925-114">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="2f925-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="2f925-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f925-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2f925-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f925-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f925-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f925-117">Not supported.</span></span>|
|<span data-ttu-id="2f925-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f925-118">Application</span></span>|<span data-ttu-id="2f925-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f925-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f925-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f925-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2f925-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2f925-121">Optional query parameters</span></span>
<span data-ttu-id="2f925-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2f925-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2f925-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f925-123">Request headers</span></span>
|<span data-ttu-id="2f925-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f925-124">Header</span></span>|<span data-ttu-id="2f925-125">Значение</span><span class="sxs-lookup"><span data-stu-id="2f925-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f925-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f925-126">Authorization</span></span>|<span data-ttu-id="2f925-127">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f925-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f925-128">Accept</span><span class="sxs-lookup"><span data-stu-id="2f925-128">Accept</span></span>|<span data-ttu-id="2f925-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2f925-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f925-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f925-130">Request body</span></span>
<span data-ttu-id="2f925-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f925-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f925-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="2f925-132">Response</span></span>
<span data-ttu-id="2f925-133">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [deviceCategory](../resources/intune-shared-devicecategory.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f925-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f925-134">Пример</span><span class="sxs-lookup"><span data-stu-id="2f925-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f925-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f925-135">Request</span></span>
<span data-ttu-id="2f925-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f925-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="2f925-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f925-137">Response</span></span>
<span data-ttu-id="2f925-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2f925-138">Here is an example of the response.</span></span> <span data-ttu-id="2f925-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="2f925-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2f925-140">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="2f925-140">Properties returned from an actual call vary according to context.</span></span>

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




