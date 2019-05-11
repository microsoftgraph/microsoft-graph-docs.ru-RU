---
title: Get detectedApp
description: Получение свойств и связей объекта detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd0308a2fb6bf7f785982b8b8008a767f06c5717
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33910025"
---
# <a name="get-detectedapp"></a><span data-ttu-id="c9506-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="c9506-103">Get detectedApp</span></span>

> <span data-ttu-id="c9506-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9506-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9506-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c9506-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9506-106">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c9506-106">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9506-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c9506-107">Prerequisites</span></span>
<span data-ttu-id="c9506-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9506-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9506-110">Permission type</span></span>|<span data-ttu-id="c9506-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9506-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9506-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9506-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9506-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9506-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c9506-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9506-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9506-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9506-115">Not supported.</span></span>|
|<span data-ttu-id="c9506-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9506-116">Application</span></span>|<span data-ttu-id="c9506-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9506-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9506-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9506-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9506-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c9506-119">Optional query parameters</span></span>
<span data-ttu-id="c9506-120">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c9506-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9506-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9506-121">Request headers</span></span>
|<span data-ttu-id="c9506-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9506-122">Header</span></span>|<span data-ttu-id="c9506-123">Значение</span><span class="sxs-lookup"><span data-stu-id="c9506-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9506-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9506-124">Authorization</span></span>|<span data-ttu-id="c9506-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9506-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9506-126">Accept</span><span class="sxs-lookup"><span data-stu-id="c9506-126">Accept</span></span>|<span data-ttu-id="c9506-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c9506-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9506-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9506-128">Request body</span></span>
<span data-ttu-id="c9506-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c9506-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9506-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="c9506-130">Response</span></span>
<span data-ttu-id="c9506-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c9506-131">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9506-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c9506-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9506-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9506-133">Request</span></span>
<span data-ttu-id="c9506-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9506-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="c9506-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9506-135">Response</span></span>
<span data-ttu-id="c9506-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9506-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.detectedApp",
    "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
    "displayName": "Display Name value",
    "version": "Version value",
    "sizeInByte": 10,
    "deviceCount": 11
  }
}
```




