---
title: Get detectedApp
description: Получение свойств и связей объекта detectedApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5569644cd0bb85a6213e0bb0bf930b162094eb57
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251435"
---
# <a name="get-detectedapp"></a><span data-ttu-id="60bb3-103">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="60bb3-103">Get detectedApp</span></span>

> <span data-ttu-id="60bb3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60bb3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60bb3-105">Получение свойств и связей объекта [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="60bb3-105">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60bb3-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="60bb3-106">Prerequisites</span></span>
<span data-ttu-id="60bb3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="60bb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60bb3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60bb3-109">Permission type</span></span>|<span data-ttu-id="60bb3-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="60bb3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60bb3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60bb3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="60bb3-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="60bb3-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="60bb3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60bb3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60bb3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60bb3-114">Not supported.</span></span>|
|<span data-ttu-id="60bb3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="60bb3-115">Application</span></span>|<span data-ttu-id="60bb3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60bb3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60bb3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60bb3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="60bb3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60bb3-118">Optional query parameters</span></span>
<span data-ttu-id="60bb3-119">Этот метод поддерживает [параметры запросов OData](https://docs.microsoft.com/en-us/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="60bb3-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60bb3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60bb3-120">Request headers</span></span>
|<span data-ttu-id="60bb3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60bb3-121">Header</span></span>|<span data-ttu-id="60bb3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="60bb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60bb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60bb3-123">Authorization</span></span>|<span data-ttu-id="60bb3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="60bb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60bb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="60bb3-125">Accept</span></span>|<span data-ttu-id="60bb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60bb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60bb3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60bb3-127">Request body</span></span>
<span data-ttu-id="60bb3-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60bb3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60bb3-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="60bb3-129">Response</span></span>
<span data-ttu-id="60bb3-130">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [detectedApp](../resources/intune-devices-detectedapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="60bb3-130">If successful, this method returns a `200 OK` response code and [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60bb3-131">Пример</span><span class="sxs-lookup"><span data-stu-id="60bb3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60bb3-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="60bb3-132">Request</span></span>
<span data-ttu-id="60bb3-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60bb3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
```

### <a name="response"></a><span data-ttu-id="60bb3-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="60bb3-134">Response</span></span>
<span data-ttu-id="60bb3-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="60bb3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



