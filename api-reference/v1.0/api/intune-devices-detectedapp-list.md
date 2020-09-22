---
title: Перечисление объектов detectedApp
description: Список свойств и связей объектов detectedApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f468d6d93710aba70821bf5117fe6c770cb7c7a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009599"
---
# <a name="list-detectedapps"></a><span data-ttu-id="b2aeb-103">Перечисление объектов detectedApp</span><span class="sxs-lookup"><span data-stu-id="b2aeb-103">List detectedApps</span></span>

<span data-ttu-id="b2aeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2aeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b2aeb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2aeb-106">Список свойств и связей объектов [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b2aeb-106">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b2aeb-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="b2aeb-107">Prerequisites</span></span>
<span data-ttu-id="b2aeb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2aeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2aeb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2aeb-110">Permission type</span></span>|<span data-ttu-id="b2aeb-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2aeb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2aeb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2aeb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2aeb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b2aeb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b2aeb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2aeb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2aeb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-115">Not supported.</span></span>|
|<span data-ttu-id="b2aeb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2aeb-116">Application</span></span>|<span data-ttu-id="b2aeb-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2aeb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2aeb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="b2aeb-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="b2aeb-119">Request headers</span></span>
|<span data-ttu-id="b2aeb-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2aeb-120">Header</span></span>|<span data-ttu-id="b2aeb-121">Значение</span><span class="sxs-lookup"><span data-stu-id="b2aeb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2aeb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2aeb-122">Authorization</span></span>|<span data-ttu-id="b2aeb-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2aeb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="b2aeb-124">Accept</span></span>|<span data-ttu-id="b2aeb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b2aeb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2aeb-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b2aeb-126">Request body</span></span>
<span data-ttu-id="b2aeb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2aeb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2aeb-128">Response</span></span>
<span data-ttu-id="b2aeb-129">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [detectedApp](../resources/intune-devices-detectedapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-129">If successful, this method returns a `200 OK` response code and a collection of [detectedApp](../resources/intune-devices-detectedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2aeb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b2aeb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2aeb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2aeb-131">Request</span></span>
<span data-ttu-id="b2aeb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
```

### <a name="response"></a><span data-ttu-id="b2aeb-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2aeb-133">Response</span></span>
<span data-ttu-id="b2aeb-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2aeb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.detectedApp",
      "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
      "displayName": "Display Name value",
      "version": "Version value",
      "sizeInByte": 10,
      "deviceCount": 11
    }
  ]
}
```









