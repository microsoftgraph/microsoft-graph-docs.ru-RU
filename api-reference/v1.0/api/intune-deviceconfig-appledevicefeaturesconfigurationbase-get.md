---
title: Get appleDeviceFeaturesConfigurationBase
description: Чтение свойств и связей объекта appleDeviceFeaturesConfigurationBase.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b1f5368ae0ab2cb9c2863f29554658e1e7f98612
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819903"
---
# <a name="get-appledevicefeaturesconfigurationbase"></a><span data-ttu-id="57fed-103">Get appleDeviceFeaturesConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="57fed-103">Get appleDeviceFeaturesConfigurationBase</span></span>

> <span data-ttu-id="57fed-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="57fed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57fed-105">Чтение свойств и связей объекта [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="57fed-105">Read properties and relationships of the [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="57fed-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="57fed-106">Prerequisites</span></span>
<span data-ttu-id="57fed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57fed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57fed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="57fed-109">Permission type</span></span>|<span data-ttu-id="57fed-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="57fed-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57fed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="57fed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="57fed-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57fed-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57fed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="57fed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57fed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57fed-114">Not supported.</span></span>|
|<span data-ttu-id="57fed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="57fed-115">Application</span></span>|<span data-ttu-id="57fed-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57fed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57fed-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="57fed-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57fed-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="57fed-118">Optional query parameters</span></span>
<span data-ttu-id="57fed-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="57fed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="57fed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="57fed-120">Request headers</span></span>
|<span data-ttu-id="57fed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="57fed-121">Header</span></span>|<span data-ttu-id="57fed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="57fed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57fed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57fed-123">Authorization</span></span>|<span data-ttu-id="57fed-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="57fed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57fed-125">Accept</span><span class="sxs-lookup"><span data-stu-id="57fed-125">Accept</span></span>|<span data-ttu-id="57fed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57fed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57fed-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="57fed-127">Request body</span></span>
<span data-ttu-id="57fed-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="57fed-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57fed-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="57fed-129">Response</span></span>
<span data-ttu-id="57fed-130">При успешном выполнении этот метод возвращает код ответа `200 OK` и объект [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="57fed-130">If successful, this method returns a `200 OK` response code and [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57fed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="57fed-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="57fed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="57fed-132">Request</span></span>
<span data-ttu-id="57fed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="57fed-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="57fed-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="57fed-134">Response</span></span>
<span data-ttu-id="57fed-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="57fed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "value": {
    "@odata.type": "#microsoft.graph.appleDeviceFeaturesConfigurationBase",
    "id": "ca0bb5ff-b5ff-ca0b-ffb5-0bcaffb50bca",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7
  }
}
```



