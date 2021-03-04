---
title: summarizeDeviceRemoteConnection
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 23053d4e61ad3f60fc2a4a7d8090d5c692d2f0eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446735"
---
# <a name="summarizedeviceremoteconnection-function"></a><span data-ttu-id="9a8a8-103">summarizeDeviceRemoteConnection</span><span class="sxs-lookup"><span data-stu-id="9a8a8-103">summarizeDeviceRemoteConnection function</span></span>

<span data-ttu-id="9a8a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a8a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a8a8-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a8a8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a8a8-107">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a8a8-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9a8a8-108">Prerequisites</span></span>
<span data-ttu-id="9a8a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a8a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a8a8-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a8a8-111">Permission type</span></span>|<span data-ttu-id="9a8a8-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a8a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a8a8-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a8a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a8a8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8a8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9a8a8-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a8a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a8a8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-116">Not supported.</span></span>|
|<span data-ttu-id="9a8a8-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9a8a8-117">Application</span></span>|<span data-ttu-id="9a8a8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a8a8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a8a8-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a8a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="9a8a8-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9a8a8-120">Request headers</span></span>
|<span data-ttu-id="9a8a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9a8a8-121">Header</span></span>|<span data-ttu-id="9a8a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9a8a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a8a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a8a8-123">Authorization</span></span>|<span data-ttu-id="9a8a8-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a8a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9a8a8-125">Accept</span></span>|<span data-ttu-id="9a8a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a8a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a8a8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a8a8-127">Request body</span></span>
<span data-ttu-id="9a8a8-128">В URL-адресе запроса укажите перечисленные ниже параметры запроса и их значения.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9a8a8-129">В приведенной ниже таблице указаны параметры, которые можно использовать с этой функцией.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9a8a8-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a8a8-130">Property</span></span>|<span data-ttu-id="9a8a8-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9a8a8-131">Type</span></span>|<span data-ttu-id="9a8a8-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9a8a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a8a8-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="9a8a8-133">summarizeBy</span></span>|[<span data-ttu-id="9a8a8-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="9a8a8-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="9a8a8-135">Пока не задокументировано.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9a8a8-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a8a8-136">Response</span></span>
<span data-ttu-id="9a8a8-137">В случае успеха эта функция возвращает код отклика и `200 OK` [коллекцию userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a8a8-138">Пример</span><span class="sxs-lookup"><span data-stu-id="9a8a8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a8a8-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a8a8-139">Request</span></span>
<span data-ttu-id="9a8a8-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection/summarizeDeviceRemoteConnection(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9a8a8-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a8a8-141">Response</span></span>
<span data-ttu-id="9a8a8-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9a8a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
      "id": "9ecbcf80-cf80-9ecb-80cf-cb9e80cfcb9e",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "virtualNetwork": "Virtual Network value",
      "deviceCount": 11,
      "cloudPcRoundTripTime": 6.666666666666667,
      "cloudPcSignInTime": 5.666666666666667,
      "remoteSignInTime": 5.333333333333333,
      "coreBootTime": 4.0,
      "coreSignInTime": 4.666666666666667,
      "cloudPcFailurePercentage": 8.0
    }
  ]
}
```




