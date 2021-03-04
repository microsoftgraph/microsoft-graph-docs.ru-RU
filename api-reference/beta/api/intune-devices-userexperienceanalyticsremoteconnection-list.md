---
title: Список userExperienceAnalyticsRemoteConnections
description: Список свойств и связей объектов userExperienceAnalyticsRemoteConnection.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7721ff94819c85e1fcb4fca4a86fc166e7e9a742
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447426"
---
# <a name="list-userexperienceanalyticsremoteconnections"></a><span data-ttu-id="9904c-103">Список userExperienceAnalyticsRemoteConnections</span><span class="sxs-lookup"><span data-stu-id="9904c-103">List userExperienceAnalyticsRemoteConnections</span></span>

<span data-ttu-id="9904c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9904c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9904c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9904c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9904c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9904c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9904c-107">Список свойств и связей [объектов userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)</span><span class="sxs-lookup"><span data-stu-id="9904c-107">List properties and relationships of the [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9904c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9904c-108">Prerequisites</span></span>
<span data-ttu-id="9904c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9904c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9904c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9904c-111">Permission type</span></span>|<span data-ttu-id="9904c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9904c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9904c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9904c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9904c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9904c-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9904c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9904c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9904c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9904c-116">Not supported.</span></span>|
|<span data-ttu-id="9904c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="9904c-117">Application</span></span>|<span data-ttu-id="9904c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9904c-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9904c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9904c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRemoteConnection
```

## <a name="request-headers"></a><span data-ttu-id="9904c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9904c-120">Request headers</span></span>
|<span data-ttu-id="9904c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9904c-121">Header</span></span>|<span data-ttu-id="9904c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9904c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9904c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9904c-123">Authorization</span></span>|<span data-ttu-id="9904c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9904c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9904c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9904c-125">Accept</span></span>|<span data-ttu-id="9904c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9904c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9904c-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9904c-127">Request body</span></span>
<span data-ttu-id="9904c-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9904c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9904c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="9904c-129">Response</span></span>
<span data-ttu-id="9904c-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9904c-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9904c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9904c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9904c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9904c-132">Request</span></span>
<span data-ttu-id="9904c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9904c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRemoteConnection
```

### <a name="response"></a><span data-ttu-id="9904c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="9904c-134">Response</span></span>
<span data-ttu-id="9904c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9904c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




