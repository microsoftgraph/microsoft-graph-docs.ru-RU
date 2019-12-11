---
title: Get detectedApp
description: Получение свойств и связей объекта detectedApp.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cc85b332ce3406383e7cd350f4f5bb608be36200
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945188"
---
# <a name="get-detectedapp"></a><span data-ttu-id="571bc-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="571bc-103">Get detectedApp</span></span>

> <span data-ttu-id="571bc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="571bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="571bc-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="571bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="571bc-106">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="571bc-106">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="571bc-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="571bc-107">Prerequisites</span></span>
<span data-ttu-id="571bc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571bc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="571bc-110">Permission type</span></span>|<span data-ttu-id="571bc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="571bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="571bc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="571bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="571bc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="571bc-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="571bc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="571bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="571bc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="571bc-115">Not supported.</span></span>|
|<span data-ttu-id="571bc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="571bc-116">Application</span></span>|<span data-ttu-id="571bc-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="571bc-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="571bc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="571bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="571bc-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="571bc-119">Optional query parameters</span></span>
<span data-ttu-id="571bc-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="571bc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="571bc-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="571bc-121">Request headers</span></span>
|<span data-ttu-id="571bc-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="571bc-122">Header</span></span>|<span data-ttu-id="571bc-123">Значение</span><span class="sxs-lookup"><span data-stu-id="571bc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="571bc-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="571bc-124">Authorization</span></span>|<span data-ttu-id="571bc-125">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="571bc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="571bc-126">Accept</span><span class="sxs-lookup"><span data-stu-id="571bc-126">Accept</span></span>|<span data-ttu-id="571bc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="571bc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="571bc-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="571bc-128">Request body</span></span>
<span data-ttu-id="571bc-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="571bc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="571bc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="571bc-130">Response</span></span>
<span data-ttu-id="571bc-131">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="571bc-131">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571bc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="571bc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="571bc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="571bc-133">Request</span></span>
<span data-ttu-id="571bc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="571bc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="571bc-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="571bc-135">Response</span></span>
<span data-ttu-id="571bc-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="571bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





