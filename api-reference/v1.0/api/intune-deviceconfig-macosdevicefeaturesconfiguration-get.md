---
title: Получение объекта macOSDeviceFeaturesConfiguration
description: Чтение свойств и связей объекта macOSDeviceFeaturesConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a64e651abe1cbcbe64c27787a09dfee621325e4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990490"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="e5505-103">Получение объекта macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5505-103">Get macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="e5505-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e5505-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5505-105">Чтение свойств и связей объекта [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e5505-105">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5505-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e5505-106">Prerequisites</span></span>
<span data-ttu-id="e5505-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5505-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5505-109">Permission type</span></span>|<span data-ttu-id="e5505-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5505-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5505-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5505-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e5505-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e5505-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e5505-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5505-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5505-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5505-114">Not supported.</span></span>|
|<span data-ttu-id="e5505-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5505-115">Application</span></span>|<span data-ttu-id="e5505-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5505-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5505-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5505-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e5505-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e5505-118">Optional query parameters</span></span>
<span data-ttu-id="e5505-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e5505-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e5505-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5505-120">Request headers</span></span>
|<span data-ttu-id="e5505-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5505-121">Header</span></span>|<span data-ttu-id="e5505-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e5505-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5505-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5505-123">Authorization</span></span>|<span data-ttu-id="e5505-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e5505-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5505-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5505-125">Accept</span></span>|<span data-ttu-id="e5505-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5505-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5505-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e5505-127">Request body</span></span>
<span data-ttu-id="e5505-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5505-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5505-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5505-129">Response</span></span>
<span data-ttu-id="e5505-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и объект [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e5505-130">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5505-131">Пример</span><span class="sxs-lookup"><span data-stu-id="e5505-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5505-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5505-132">Request</span></span>
<span data-ttu-id="e5505-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5505-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e5505-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="e5505-134">Response</span></span>
<span data-ttu-id="e5505-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e5505-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



